## `drupal:9-php8.0-fpm-buster`

```console
$ docker pull drupal@sha256:1a4403f0a8eeb50a0467a4cfc52648f867899a875fbd1fe02a7f222293fe8ab3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:9-php8.0-fpm-buster` - linux; amd64

```console
$ docker pull drupal@sha256:c45f2c6a2400ebddaabd4fadbf9a179bcb692ac6bcb2b976754c4a8ac3203178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.3 MB (166309472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382d77854f098fde905a36ff7886e7ede11c7fe441c58ace0037566f0bf463b1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 07 Sep 2023 07:04:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 07 Sep 2023 07:05:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 07:05:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 07 Sep 2023 07:05:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 07 Sep 2023 07:05:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 07:05:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 07:05:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 07 Sep 2023 07:05:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 07 Sep 2023 07:05:03 GMT
ENV PHP_VERSION=8.0.30
# Thu, 07 Sep 2023 07:05:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 07 Sep 2023 07:05:03 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 07 Sep 2023 07:05:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Sep 2023 07:05:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Sep 2023 07:14:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Sep 2023 07:14:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 07 Sep 2023 07:14:39 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Sep 2023 07:14:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Sep 2023 07:14:39 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 07:14:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 07 Sep 2023 07:14:40 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Sep 2023 07:14:40 GMT
EXPOSE 9000
# Thu, 07 Sep 2023 07:14:40 GMT
CMD ["php-fpm"]
# Thu, 07 Sep 2023 23:47:59 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 23:47:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 Sep 2023 21:13:02 GMT
COPY file:e07dca2693c052eccdcb8ecf6a4ddfa6367b2f80335dac5c4ad082d553fdbda6 in /usr/local/bin/ 
# Fri, 15 Sep 2023 21:13:02 GMT
ENV DRUPAL_VERSION=9.5.10
# Fri, 15 Sep 2023 21:13:02 GMT
WORKDIR /opt/drupal
# Fri, 15 Sep 2023 21:13:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 15 Sep 2023 21:13:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae13a49b7b1fa8948b97a72ec6e48151a5a7703df58f481e83bbb72ecd4526e1`  
		Last Modified: Thu, 07 Sep 2023 07:30:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1e9c09cf55454a744cb48ef46c9b0dca23fa800aab4d556edcbbe86dcfc582`  
		Last Modified: Thu, 07 Sep 2023 07:30:34 GMT  
		Size: 76.7 MB (76691058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b4b1d57b71aee6b68bc9e2f31ca05d2c1903c9d0b84755265790dd5ff6681`  
		Last Modified: Thu, 07 Sep 2023 07:30:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fd9e8efd1b481065a5ac82e6dd9420c5112a261921cd142829f54db5f2df84`  
		Last Modified: Thu, 07 Sep 2023 07:30:23 GMT  
		Size: 11.1 MB (11144000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c449c53b3bf252092120f49db386cf0ea6e5565e47de5990eef1e645d953a318`  
		Last Modified: Thu, 07 Sep 2023 07:30:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03888dce23dd102fb2c36c2b6ff6691d5eab743a7631234a2b5cebcc7cbcd11`  
		Last Modified: Thu, 07 Sep 2023 07:31:05 GMT  
		Size: 25.5 MB (25465963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59d62c7a41b5d110e266d2d4ce1bb690f98a3898176b48d64f25b33707d5cbd`  
		Last Modified: Thu, 07 Sep 2023 07:31:02 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0ea7de831529d3d7692a787c663f7be8647bd600cd4c85d21c9ead97db1f2e`  
		Last Modified: Thu, 07 Sep 2023 07:31:02 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5aa51a0135cca330289bd51b1113c9084a403c98e63f819f924969f9ac12b`  
		Last Modified: Thu, 07 Sep 2023 07:31:02 GMT  
		Size: 8.7 KB (8717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80167c6a38642fdc582bbc0a178a80db775df92f00e8c5dc77d5518fa133ce28`  
		Last Modified: Fri, 08 Sep 2023 00:06:33 GMT  
		Size: 2.2 MB (2223735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e67ee74c527e8ed983fece6ccc71a0650d0a9ef470500d4c353cc8184aa3369`  
		Last Modified: Fri, 08 Sep 2023 00:06:33 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1c383cde9d2eda998a45a658e40525b08bd38afb56825f4d6eef21c4c9495`  
		Last Modified: Fri, 15 Sep 2023 21:34:22 GMT  
		Size: 704.4 KB (704422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78379ffce887d12896959a0af1267a08974854be362904aa13596746e618763d`  
		Last Modified: Fri, 15 Sep 2023 21:34:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19734f703336f258cd2995590ed399ca31b8fda2cd9bee8db042dbabb9bd7d0f`  
		Last Modified: Fri, 15 Sep 2023 21:34:27 GMT  
		Size: 22.9 MB (22880045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:26704058921b61814433594904bfc74eac72e9a22fcafe97b9a7a6815c397681
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141911650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bb2d4dc37b5872d6074f3d280bbe16db4b38299366578122548e8bf9d504d0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 18:38:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 07 Sep 2023 18:38:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 07 Sep 2023 18:39:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 18:39:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 07 Sep 2023 18:39:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 07 Sep 2023 18:39:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 18:39:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 18:39:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 07 Sep 2023 18:39:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 07 Sep 2023 18:39:24 GMT
ENV PHP_VERSION=8.0.30
# Thu, 07 Sep 2023 18:39:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 07 Sep 2023 18:39:25 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 07 Sep 2023 18:39:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Sep 2023 18:39:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Sep 2023 18:48:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Sep 2023 18:48:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 07 Sep 2023 18:48:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Sep 2023 18:48:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Sep 2023 18:48:26 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 18:48:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 07 Sep 2023 18:48:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Sep 2023 18:48:27 GMT
EXPOSE 9000
# Thu, 07 Sep 2023 18:48:27 GMT
CMD ["php-fpm"]
# Fri, 08 Sep 2023 04:29:53 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 04:29:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 Sep 2023 21:13:10 GMT
COPY file:e07dca2693c052eccdcb8ecf6a4ddfa6367b2f80335dac5c4ad082d553fdbda6 in /usr/local/bin/ 
# Fri, 15 Sep 2023 21:13:10 GMT
ENV DRUPAL_VERSION=9.5.10
# Fri, 15 Sep 2023 21:13:10 GMT
WORKDIR /opt/drupal
# Fri, 15 Sep 2023 21:13:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 15 Sep 2023 21:13:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed417f72a0d8c0020491eace2aef68fe5e017ce353baf87a7c0a0d523ff8384`  
		Last Modified: Thu, 07 Sep 2023 19:06:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31950e5c5fc44b2e387de59b3aac9a1a18544a5e070a1be579e612ed4e1741e6`  
		Last Modified: Thu, 07 Sep 2023 19:07:02 GMT  
		Size: 59.5 MB (59541512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df50a7162df832b2fadaa8a33cd31a2b5e2b34f8f6f9a342057e0bfe6652005`  
		Last Modified: Thu, 07 Sep 2023 19:06:45 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91826e2c9bc3d8b2268c495e76f8bd84c0a8d38aac18279ef58253561fda673`  
		Last Modified: Thu, 07 Sep 2023 19:06:44 GMT  
		Size: 11.1 MB (11142234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3903053ef58ddc252ad455ac161ad24a89574cc33cd519162f889189041cfbe1`  
		Last Modified: Thu, 07 Sep 2023 19:06:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7aa4c27c173abf8b2a19f1b43a232d62508ca1b4b744c31eb752b132de3127`  
		Last Modified: Thu, 07 Sep 2023 19:07:40 GMT  
		Size: 23.2 MB (23225444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5eb1398dd31adcb83e692f486861d2c5d6679a9c4e71bf5abd7a3f5afe268d6`  
		Last Modified: Thu, 07 Sep 2023 19:07:35 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e97dc4bff33e018d946808fbc580883e343a59181f8372d49e6aed49bbbeb0`  
		Last Modified: Thu, 07 Sep 2023 19:07:35 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb3ef1eb7bfedc06fb97b121e0a872848df740944ddf14ba8080f9e0904fdc`  
		Last Modified: Thu, 07 Sep 2023 19:07:35 GMT  
		Size: 8.7 KB (8719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34369f36d45d0c26ab92aece9bbb76b28b081fd245e65d61a60afc464833a4fa`  
		Last Modified: Fri, 08 Sep 2023 04:53:37 GMT  
		Size: 1.6 MB (1608988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e26a48c5a22ef1e69c52b081f78e770329b28f5c0629565262407aee3fea500`  
		Last Modified: Fri, 08 Sep 2023 04:53:37 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c11839523ae5f69f898a9ae232740518ba034087a2aab6ad09ad51a18cfea75`  
		Last Modified: Fri, 15 Sep 2023 21:41:48 GMT  
		Size: 704.4 KB (704418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1709aa6cadbc7038ceda941eaf5f9e81ab9f8eaf2626af7cef6960b4beec59f2`  
		Last Modified: Fri, 15 Sep 2023 21:41:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bb78a511cbc8923af08a08ffdbbaf2f6852514001b5d58c45525c2a5d39918`  
		Last Modified: Fri, 15 Sep 2023 21:42:04 GMT  
		Size: 22.9 MB (22880439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:1cefbc1d82096d41aefc179d48b8766b77a9994b98bc95ee4cd6b6eb78f69744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157860955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3732204c8b597254cb417574868687652b4a0371e9f528e9d738848ff04b6dd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:42 GMT
ADD file:22373577ebc4a88322b8e7e5a349667740deade289df65952593aa5fa355e161 in / 
# Wed, 20 Sep 2023 02:44:42 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:47:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 05:47:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 05:47:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:47:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 05:47:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 05:47:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:47:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:47:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:47:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 05:47:48 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 05:47:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 05:47:48 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 05:47:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 05:47:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:54:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 05:54:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:54:20 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 05:54:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 05:54:20 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 05:54:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 05:54:21 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 05:54:21 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 05:54:21 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 18:44:47 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:44:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 20 Sep 2023 18:44:48 GMT
COPY file:e07dca2693c052eccdcb8ecf6a4ddfa6367b2f80335dac5c4ad082d553fdbda6 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:44:48 GMT
ENV DRUPAL_VERSION=9.5.10
# Wed, 20 Sep 2023 18:44:48 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 18:45:07 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 20 Sep 2023 18:45:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:a5329dc26fe29288aabb62184c71ef06987bd81c95d7c43a48e38a0dfaa54ff8`  
		Last Modified: Wed, 20 Sep 2023 02:48:50 GMT  
		Size: 26.0 MB (25967816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b246114d1c77fb2a14434449a34b0e8761eb8579db67ea844bcd3b8b2080f7b5`  
		Last Modified: Wed, 20 Sep 2023 06:16:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f42380bd1e57d38a9a1bc857bece1bf51fe9157002f8e40e30f9edfd97dff`  
		Last Modified: Wed, 20 Sep 2023 06:16:42 GMT  
		Size: 70.4 MB (70362229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1529d01406312ce383fe74f2bc5676b908600571adc5a10ebc8c6f837ee38a`  
		Last Modified: Wed, 20 Sep 2023 06:16:35 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cfc38845c60155c60a352c98a73092fc654e765b8289c68a30227cf87a2ec`  
		Last Modified: Wed, 20 Sep 2023 06:16:34 GMT  
		Size: 11.1 MB (11142899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f7fcff1b070a8913a26420ca06a3763c11d2f58114bfc35fb6d3923d0178ae`  
		Last Modified: Wed, 20 Sep 2023 06:16:33 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10db98f60721805789588b33e051b008117babed49da2147c5fe398a12004476`  
		Last Modified: Wed, 20 Sep 2023 06:17:10 GMT  
		Size: 24.9 MB (24914009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e6184f89698c93a6609e05da4611b5e5dd91dfddaf0c50dd75aa780c3f27a`  
		Last Modified: Wed, 20 Sep 2023 06:17:08 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa66ed464e2b86ec845d1769db1a09ac7f98e58634f6fd1cb99f220939afe9b`  
		Last Modified: Wed, 20 Sep 2023 06:17:08 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44d4db9e3a635743dc712b77f56ee9dc21f7a1033701e77aa791e07df1275c2`  
		Last Modified: Wed, 20 Sep 2023 06:17:08 GMT  
		Size: 8.7 KB (8714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4194729afc049c943f6cee2940ac11d7e880bb6f51eee71cbfdfc8e0040b608`  
		Last Modified: Wed, 20 Sep 2023 19:01:08 GMT  
		Size: 1.9 MB (1876477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76f0296617cbdf48cc82d77af6f49f5a4fba2903b6b6f5b032d175d3cdd1453`  
		Last Modified: Wed, 20 Sep 2023 19:01:08 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144016a7ad835fa3641b7f2d5d1ce5409efb1375c8ca21b001c0bee7756316cd`  
		Last Modified: Wed, 20 Sep 2023 19:01:08 GMT  
		Size: 704.4 KB (704414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caeaea6efa3c456348f4afb982c623c4053262e8177f3b43ce444f6b87a1d65`  
		Last Modified: Wed, 20 Sep 2023 19:01:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d86cd19983e04ffb35bdd2435f16183db0b6467c5fcf7253acdf1a92d73a66`  
		Last Modified: Wed, 20 Sep 2023 19:01:12 GMT  
		Size: 22.9 MB (22880256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-buster` - linux; 386

```console
$ docker pull drupal@sha256:675dc3fc8607af2b996f1107729058acfeaac1a375337d11e7473b305d1f4ec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.0 MB (172036854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da16ae0b152621c776381bf7a58484c60b4019e7110e239492d39241bb992c97`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:41 GMT
ADD file:fb989660816f4cd43e34acc142a953475b8c7002d0827f2bf3f52df3f7792cbf in / 
# Wed, 20 Sep 2023 00:42:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 06:30:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 06:30:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 06:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 06:30:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 06:30:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 06:30:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:30:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:30:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 06:30:55 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 06:30:55 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 06:30:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 06:30:55 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 06:31:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 06:31:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:46:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 06:46:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:46:56 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 06:46:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 06:46:57 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:46:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 06:46:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 06:46:58 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 06:46:58 GMT
CMD ["php-fpm"]
# Thu, 21 Sep 2023 03:11:11 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:11:11 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Sep 2023 03:11:12 GMT
COPY file:e07dca2693c052eccdcb8ecf6a4ddfa6367b2f80335dac5c4ad082d553fdbda6 in /usr/local/bin/ 
# Thu, 21 Sep 2023 03:11:12 GMT
ENV DRUPAL_VERSION=9.5.10
# Thu, 21 Sep 2023 03:11:12 GMT
WORKDIR /opt/drupal
# Thu, 21 Sep 2023 03:11:27 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 21 Sep 2023 03:11:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d2583a509dfdf283554f9e60a045ae6823d40ee59a6bb9892e15839171b30970`  
		Last Modified: Wed, 20 Sep 2023 00:48:22 GMT  
		Size: 27.8 MB (27846922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e957484b5cac85a6080e6d3c04e08504754aea75df923ea9e2443b28ce29f97`  
		Last Modified: Wed, 20 Sep 2023 07:15:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5282a2ff79ffe102d2983dbdc3aae753caccd756b0afa0b7e4f1920f43a41a9d`  
		Last Modified: Wed, 20 Sep 2023 07:16:00 GMT  
		Size: 81.2 MB (81235090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c03d8322b1297d6a7523f660b5817670c569707c2395a345be66ebe3b857b68`  
		Last Modified: Wed, 20 Sep 2023 07:15:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c0c224adbf109874eb79b78cf3b6631748ef68ac10678328cc7285d61d2dc7`  
		Last Modified: Wed, 20 Sep 2023 07:15:41 GMT  
		Size: 11.1 MB (11143406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65ff38865308e8df02c6773c45cf4f04ee726a277283d1d648e448da19e59c4`  
		Last Modified: Wed, 20 Sep 2023 07:15:39 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee81c0d94d756a33d34745ddc1191190061c552b8c37509159a7d0792f0e7a`  
		Last Modified: Wed, 20 Sep 2023 07:16:36 GMT  
		Size: 25.9 MB (25921964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2493f600e6452ad604b4ebae5b1297ea48a49027224806522dbb91178e4a6e`  
		Last Modified: Wed, 20 Sep 2023 07:16:30 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205729eb534e310895f33f652905b81398d2695a1f1c4a6a47b357b28a559530`  
		Last Modified: Wed, 20 Sep 2023 07:16:30 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb3582613e47e8357cc0cdc0f1416487d44b4443ace345403066e6d9c1d892d`  
		Last Modified: Wed, 20 Sep 2023 07:16:30 GMT  
		Size: 8.7 KB (8718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4842e34acfb65c23454f89ebbffce4afbcc6caaad0f295f452e5c5c8e7d000`  
		Last Modified: Thu, 21 Sep 2023 03:30:07 GMT  
		Size: 2.3 MB (2292980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2762f3bf22afd402c403e7fdac3d3cf22f4417140e42a2c3b3a3766b58595a`  
		Last Modified: Thu, 21 Sep 2023 03:30:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d51aa42a4c2dd00d6f328964f351594bf35eb7d4eae934a1c0afdb76e0dd79d`  
		Last Modified: Thu, 21 Sep 2023 03:30:07 GMT  
		Size: 704.4 KB (704419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c6890f7494eddf181e099531cfef34a619367c043810ed415e17af0b1d94e`  
		Last Modified: Thu, 21 Sep 2023 03:30:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551e77aa7bd0a8649f35e983bd8b3792145aafe7c0664d641377b8ce4ddac06`  
		Last Modified: Thu, 21 Sep 2023 03:30:15 GMT  
		Size: 22.9 MB (22879209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
