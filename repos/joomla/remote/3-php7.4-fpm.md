## `joomla:3-php7.4-fpm`

```console
$ docker pull joomla@sha256:5edfc5b9a8c7e93e27b72a15ffcfecd275fe6291a1c2f87ae175aaeb61f67d67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `joomla:3-php7.4-fpm` - linux; amd64

```console
$ docker pull joomla@sha256:4f7ade585971da3cf60b262ad1d42e44cfd1afe2e29bc13cbbe8c262439817ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155924488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed13543a5e154e7d2b46a1882dcf461febcb171d6e276387d4b1125a39783bf6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:26:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 01 Feb 2020 19:26:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 01 Feb 2020 19:26:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:26:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 01 Feb 2020 19:26:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 01 Feb 2020 19:40:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 01 Feb 2020 19:40:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 01 Feb 2020 19:40:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 01 Feb 2020 19:40:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 01 Feb 2020 19:40:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 Feb 2020 19:40:30 GMT
ENV PHP_VERSION=7.4.2
# Sat, 01 Feb 2020 19:40:30 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Sat, 01 Feb 2020 19:40:31 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Sat, 01 Feb 2020 19:40:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 01 Feb 2020 19:40:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:48:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 01 Feb 2020 19:48:46 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:48:47 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 Feb 2020 19:48:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 Feb 2020 19:48:48 GMT
WORKDIR /var/www/html
# Sat, 01 Feb 2020 19:48:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 Feb 2020 19:48:49 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 Feb 2020 19:48:49 GMT
EXPOSE 9000
# Sat, 01 Feb 2020 19:48:49 GMT
CMD ["php-fpm"]
# Sun, 02 Feb 2020 11:44:30 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Sun, 02 Feb 2020 11:44:30 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 02 Feb 2020 11:46:06 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:46:07 GMT
VOLUME [/var/www/html]
# Sun, 02 Feb 2020 11:46:07 GMT
ENV JOOMLA_VERSION=3.9.15
# Sun, 02 Feb 2020 11:46:07 GMT
ENV JOOMLA_SHA512=d68e32de6cfe9af92ff7f7991c9253a4487832e55e32e6f74f2b4d592a4777f3b4d8bd74dcd0b10d4262c5e39bdad1e9f7698dedb2ef2989dbc06aa7ab2f6c69
# Sun, 02 Feb 2020 11:46:11 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 02 Feb 2020 11:46:12 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Sun, 02 Feb 2020 11:46:12 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 02 Feb 2020 11:46:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 02 Feb 2020 11:46:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3224e2c3a8935eadbb2b4ae8f162c5cdda9e4b5693f763d7c7fa1c4e0288374`  
		Last Modified: Sat, 01 Feb 2020 21:46:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7a066df88f078e73668ecda25e6f74ddb03c4b542565e0e8cb675fa4e25631`  
		Last Modified: Sat, 01 Feb 2020 21:47:06 GMT  
		Size: 76.7 MB (76652069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdf741d72a992e97109c02ec1f5f583127a47b1c4c054a351b96a5f259ca1ab`  
		Last Modified: Sat, 01 Feb 2020 21:46:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0096578ff21cb156c142789cfcb3e12462855b8d2377b100aace4cb2dfcebdfc`  
		Last Modified: Sat, 01 Feb 2020 21:47:38 GMT  
		Size: 10.6 MB (10573031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b9a3846c51f5bee5b773bea6819e1278e00879bd9531f4fdc6dbd3636ea0d7`  
		Last Modified: Sat, 01 Feb 2020 21:47:37 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8df69c5cfa70bfa68ccfb2159a3b83d49efaf26d32622eb7ec40e5a80e53c`  
		Last Modified: Sat, 01 Feb 2020 21:47:44 GMT  
		Size: 28.5 MB (28522696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba16a18226804ba5bf5e931c45f506f308a4c5fd466cc3ea770da0c6ffe0c80b`  
		Last Modified: Sat, 01 Feb 2020 21:47:36 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c137b651214d4f9fe1b92655aee7de3f4ccee8eaf232e23a7c30bdb0a9180fae`  
		Last Modified: Sat, 01 Feb 2020 21:47:36 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2738b6c9bea0dbc8561c051f828efb73cf6c7291a299e1573ef29426a979cd6`  
		Last Modified: Sat, 01 Feb 2020 21:47:36 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1779e0a68b1a7880c6ccf0f6d196d050ab65902fb7de5c8fbc14fe90bef849d`  
		Last Modified: Sun, 02 Feb 2020 11:48:33 GMT  
		Size: 3.4 MB (3418847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b79f5ffa0ac1e0198eee3328f14fa9b78301a01ed9e735f673e0efda76e14d`  
		Last Modified: Sun, 02 Feb 2020 11:48:38 GMT  
		Size: 9.7 MB (9651972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6254f764894f1c437f31d1da58df2467b89c53aad685c9e348dbee6a8561`  
		Last Modified: Sun, 02 Feb 2020 11:48:32 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42d4760014ccac6483c407b4fd94c477b795e6b2dddacb7ce74f1f685df28b5`  
		Last Modified: Sun, 02 Feb 2020 11:48:32 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.4-fpm` - linux; arm variant v5

```console
$ docker pull joomla@sha256:df73518a6479439dc2feeba54d638f6cc1b1ac2dd0c322cd30685d3c87fc4225
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134266971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dcebb55ae24f2064a4b9bf11a3d9f85b1975806e4f87f75edea2500fa826e78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 20:53:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 01 Feb 2020 20:53:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 01 Feb 2020 20:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 20:54:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 01 Feb 2020 20:54:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 01 Feb 2020 21:02:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 01 Feb 2020 21:02:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 01 Feb 2020 21:02:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 01 Feb 2020 21:02:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 01 Feb 2020 21:02:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 Feb 2020 21:02:34 GMT
ENV PHP_VERSION=7.4.2
# Sat, 01 Feb 2020 21:02:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Sat, 01 Feb 2020 21:02:36 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Sat, 01 Feb 2020 21:02:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 01 Feb 2020 21:02:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:06:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 01 Feb 2020 21:06:10 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:06:12 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 Feb 2020 21:06:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 Feb 2020 21:06:14 GMT
WORKDIR /var/www/html
# Sat, 01 Feb 2020 21:06:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 Feb 2020 21:06:17 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 Feb 2020 21:06:17 GMT
EXPOSE 9000
# Sat, 01 Feb 2020 21:06:18 GMT
CMD ["php-fpm"]
# Sun, 02 Feb 2020 07:07:39 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Sun, 02 Feb 2020 07:07:40 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 02 Feb 2020 07:10:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 07:10:45 GMT
VOLUME [/var/www/html]
# Sun, 02 Feb 2020 07:10:49 GMT
ENV JOOMLA_VERSION=3.9.15
# Sun, 02 Feb 2020 07:10:50 GMT
ENV JOOMLA_SHA512=d68e32de6cfe9af92ff7f7991c9253a4487832e55e32e6f74f2b4d592a4777f3b4d8bd74dcd0b10d4262c5e39bdad1e9f7698dedb2ef2989dbc06aa7ab2f6c69
# Sun, 02 Feb 2020 07:11:01 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 02 Feb 2020 07:11:02 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Sun, 02 Feb 2020 07:11:03 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 02 Feb 2020 07:11:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 02 Feb 2020 07:11:05 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c45ccccae36b11824d60e44524af7b6fa50071e3d611d84cb304dd77defab8`  
		Last Modified: Sat, 01 Feb 2020 22:23:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bb0996b6fdaded26517b7c76776a1a9c8884099f10dedce0542539497f118b`  
		Last Modified: Sat, 01 Feb 2020 22:23:37 GMT  
		Size: 58.8 MB (58799601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd04cf71e89913a06b80581e3e995075f83ad72367a777cf4c4eab806021fe5`  
		Last Modified: Sat, 01 Feb 2020 22:23:16 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1880f0deeb40c38e461fe63063e7aa718c89612b79545cd487437f8d8099b5`  
		Last Modified: Sat, 01 Feb 2020 22:24:29 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacfa0726c87bd2c56f2d2fa414f55db3d42977de34ed2381d5f3a753234012a`  
		Last Modified: Sat, 01 Feb 2020 22:24:26 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9555884c3a2456b0223a49d045cedfb97a0bc355ea563633446dcd1b827dc0`  
		Last Modified: Sat, 01 Feb 2020 22:24:35 GMT  
		Size: 27.2 MB (27151833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4948631a87a5d960969a56611f5cdc7102b432859c38b2b8f0760d9c581b8d80`  
		Last Modified: Sat, 01 Feb 2020 22:24:27 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5010e1d2b6e31436a317094236d33eb62373302337ff2130c9c57a0d1e0c6363`  
		Last Modified: Sat, 01 Feb 2020 22:24:27 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4f65df82e0845f2c2bf4e205fcde6d4e117d840d1d742fc2d529e0a7b6c13`  
		Last Modified: Sat, 01 Feb 2020 22:24:27 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd62f1e8a95be1f3cfe93c0e7b4053b5f78fe4c45719988146bef08558f83929`  
		Last Modified: Sun, 02 Feb 2020 07:14:06 GMT  
		Size: 3.2 MB (3249219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faf2a6e47c416d8caabbdc3f4fd9b34484ab69e3154c6c598ecf3c8d9c3b267`  
		Last Modified: Sun, 02 Feb 2020 07:14:10 GMT  
		Size: 9.7 MB (9651957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709ff640b4f3727949677653c828c8b4135b98ea02e493b72bba0abdbe6821d9`  
		Last Modified: Sun, 02 Feb 2020 07:14:05 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d035b520b34ba34f728031df12872bf227555f6a41f5fdb116a73ecc1d561`  
		Last Modified: Sun, 02 Feb 2020 07:14:05 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.4-fpm` - linux; arm variant v7

```console
$ docker pull joomla@sha256:e010d4d591158ed87f9b0c9a6ce71b2f33964182187b0b3642f870c68cf86a40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131763583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2564f74d42ef9d802f38cdf4d4d35f3e044dd24549ec666c60a091c73fb4e855`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:58:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 02 Feb 2020 00:58:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 02 Feb 2020 00:59:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:59:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 02 Feb 2020 00:59:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 02 Feb 2020 01:07:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sun, 02 Feb 2020 01:07:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 01:07:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 01:07:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sun, 02 Feb 2020 01:07:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sun, 02 Feb 2020 01:07:42 GMT
ENV PHP_VERSION=7.4.2
# Sun, 02 Feb 2020 01:07:43 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Sun, 02 Feb 2020 01:07:44 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Sun, 02 Feb 2020 01:07:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 01:08:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 02 Feb 2020 01:11:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sun, 02 Feb 2020 01:11:17 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sun, 02 Feb 2020 01:11:19 GMT
RUN docker-php-ext-enable sodium
# Sun, 02 Feb 2020 01:11:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 02 Feb 2020 01:11:21 GMT
WORKDIR /var/www/html
# Sun, 02 Feb 2020 01:11:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sun, 02 Feb 2020 01:11:24 GMT
STOPSIGNAL SIGQUIT
# Sun, 02 Feb 2020 01:11:25 GMT
EXPOSE 9000
# Sun, 02 Feb 2020 01:11:25 GMT
CMD ["php-fpm"]
# Sun, 02 Feb 2020 17:21:57 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Sun, 02 Feb 2020 17:21:58 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 02 Feb 2020 17:24:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 17:24:24 GMT
VOLUME [/var/www/html]
# Sun, 02 Feb 2020 17:24:24 GMT
ENV JOOMLA_VERSION=3.9.15
# Sun, 02 Feb 2020 17:24:25 GMT
ENV JOOMLA_SHA512=d68e32de6cfe9af92ff7f7991c9253a4487832e55e32e6f74f2b4d592a4777f3b4d8bd74dcd0b10d4262c5e39bdad1e9f7698dedb2ef2989dbc06aa7ab2f6c69
# Sun, 02 Feb 2020 17:24:35 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 02 Feb 2020 17:24:37 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Sun, 02 Feb 2020 17:24:38 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 02 Feb 2020 17:24:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 02 Feb 2020 17:24:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37cb050f89036596ba7c3e4ddbe118156973fe8b59516e353a42ac97a3f6ba5`  
		Last Modified: Sun, 02 Feb 2020 02:28:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd60b6434b4a4eac9a8103900797e1a4260baf12d401a112911179fe3c37e00`  
		Last Modified: Sun, 02 Feb 2020 02:29:01 GMT  
		Size: 59.5 MB (59500876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a07b40ddbc553f32319192f74a79015c5c90e56e523b22f6ad70245aa8411ff`  
		Last Modified: Sun, 02 Feb 2020 02:28:40 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2f849b7a97ead7a5f22ff873cc8ec5785105da9e949940a2f000a855116c05`  
		Last Modified: Sun, 02 Feb 2020 02:29:55 GMT  
		Size: 10.6 MB (10570952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cddf1a6805952f777af4a7252ac84d0d70b456383a5e18cda973da9cfe1b67f`  
		Last Modified: Sun, 02 Feb 2020 02:29:52 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95e34cc6b2ec0c1b0dfbebeed005d2b44ec661ae9888865ca94f05334ab9915`  
		Last Modified: Sun, 02 Feb 2020 02:30:00 GMT  
		Size: 26.2 MB (26170079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d809d453e4107507953bc5e127157b661c4fe96f2aa3403a8085676b37c31516`  
		Last Modified: Sun, 02 Feb 2020 02:29:52 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4c79dbf45508447d978d6e71d2a21fa0deb824c15f6ee37d56037a81ac1c0f`  
		Last Modified: Sun, 02 Feb 2020 02:29:52 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c80bdf10f33c793287f803a960036cec2a0777ce0bdeb25191d3847c4b8350`  
		Last Modified: Sun, 02 Feb 2020 02:29:52 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9255264411a5a126d276395d280b3c94a30c7cd1f6a92f032948cb291e8ed`  
		Last Modified: Sun, 02 Feb 2020 17:28:06 GMT  
		Size: 3.2 MB (3156915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77de35b0fb6ad5a8ea22935f9910a9dab1dea9148ccf57894504c66fc9ec5fe7`  
		Last Modified: Sun, 02 Feb 2020 17:28:10 GMT  
		Size: 9.7 MB (9651961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a14a24adae25388169aff172c22c41c3d1e2d705ef7905b7413d2d47a1a42bd`  
		Last Modified: Sun, 02 Feb 2020 17:28:05 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9bbae3a1af8433183ac2c6fb444ad8a6288dfef50e7f99077bebcacbe9de56`  
		Last Modified: Sun, 02 Feb 2020 17:28:04 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.4-fpm` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:5cb9aa59dd32b69310baede38e53232b22a7e053db4445a7dfe0ed714d577004
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148062521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a981fb1e26fc0434b874ee60126b089bb227c12b15aa2a21c3f06c3f535807d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:04:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 02 Feb 2020 08:04:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 02 Feb 2020 08:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:05:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 02 Feb 2020 08:05:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 02 Feb 2020 08:13:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sun, 02 Feb 2020 08:13:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 08:13:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 08:13:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sun, 02 Feb 2020 08:13:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sun, 02 Feb 2020 08:13:59 GMT
ENV PHP_VERSION=7.4.2
# Sun, 02 Feb 2020 08:13:59 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Sun, 02 Feb 2020 08:14:00 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Sun, 02 Feb 2020 08:14:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 08:14:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:17:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sun, 02 Feb 2020 08:17:29 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:17:31 GMT
RUN docker-php-ext-enable sodium
# Sun, 02 Feb 2020 08:17:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 02 Feb 2020 08:17:32 GMT
WORKDIR /var/www/html
# Sun, 02 Feb 2020 08:17:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sun, 02 Feb 2020 08:17:35 GMT
STOPSIGNAL SIGQUIT
# Sun, 02 Feb 2020 08:17:35 GMT
EXPOSE 9000
# Sun, 02 Feb 2020 08:17:36 GMT
CMD ["php-fpm"]
# Sun, 02 Feb 2020 18:05:46 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Sun, 02 Feb 2020 18:05:47 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 02 Feb 2020 18:08:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 18:08:32 GMT
VOLUME [/var/www/html]
# Sun, 02 Feb 2020 18:08:32 GMT
ENV JOOMLA_VERSION=3.9.15
# Sun, 02 Feb 2020 18:08:33 GMT
ENV JOOMLA_SHA512=d68e32de6cfe9af92ff7f7991c9253a4487832e55e32e6f74f2b4d592a4777f3b4d8bd74dcd0b10d4262c5e39bdad1e9f7698dedb2ef2989dbc06aa7ab2f6c69
# Sun, 02 Feb 2020 18:08:41 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 02 Feb 2020 18:08:42 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Sun, 02 Feb 2020 18:08:43 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 02 Feb 2020 18:08:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 02 Feb 2020 18:08:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ef482177c11080f835ff485ad054b5897ed5bc3778a7a2ebe68b655a930e06`  
		Last Modified: Sun, 02 Feb 2020 09:33:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff48b131cc3e3c219ce42e8dd4b8f558c3f2b70b6b5a533ec8ec378a8244a5df`  
		Last Modified: Sun, 02 Feb 2020 09:34:15 GMT  
		Size: 70.3 MB (70334393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38b85eef9c7a9d92bcece36db91d11c75af83cbce73aef5e34bf5c9d3bfddc0`  
		Last Modified: Sun, 02 Feb 2020 09:33:55 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360e93995a3b0c60807c4dd141891f4c439c206db3b977788e8dc75f5b435c0`  
		Last Modified: Sun, 02 Feb 2020 09:35:04 GMT  
		Size: 10.6 MB (10571814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cf79f39bec65076d2626a0c65f63ba095acf1261fb473fa9a736ffd18f203d`  
		Last Modified: Sun, 02 Feb 2020 09:35:01 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8400693fdcd11fd81aaa9cbbc60dbe290b8239395e3ff05e2b267176850342ae`  
		Last Modified: Sun, 02 Feb 2020 09:35:10 GMT  
		Size: 28.3 MB (28276504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37006c08410519cbbeb460c94f6be1465a09f009c28d182d0c864938ca6f2557`  
		Last Modified: Sun, 02 Feb 2020 09:35:01 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0acfa60e5bb8d2fba15f7f8b934d65ad6ab711ef2c1d465f6d030a2b432e92`  
		Last Modified: Sun, 02 Feb 2020 09:35:01 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be415e5ba0ab77cf1a3c50796ef1643bae27e456de705a7909ae4c61307a299`  
		Last Modified: Sun, 02 Feb 2020 09:35:01 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a16f782de506a525f0a9a64fdb497fcbcbc43598c5e231d89010b34b8dca271`  
		Last Modified: Sun, 02 Feb 2020 18:12:12 GMT  
		Size: 3.4 MB (3363536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d275bfed01b9a56aeec35ca23e11be2b9a0ea0f8884aa53104b8e90854ea9e`  
		Last Modified: Sun, 02 Feb 2020 18:12:16 GMT  
		Size: 9.7 MB (9651961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b61faa9f021751e52bf698d1fa902a783bc437cb99dfc337c8888c7849da989`  
		Last Modified: Sun, 02 Feb 2020 18:12:11 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ef2db1185f8ba10d45c7aa3eacdc4e5f27e6648d1a893de3e9d531d5f13d12`  
		Last Modified: Sun, 02 Feb 2020 18:12:11 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.4-fpm` - linux; 386

```console
$ docker pull joomla@sha256:3fecebdc8bddaaf78263d35a5c98a171f3942c1190486e253ace820e86e293d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.7 MB (161734261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5176a9efc86a4c1f612e25465b43c29077a5d37613da77d7e6fac0f0f1234736`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:33:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 02 Feb 2020 01:33:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 02 Feb 2020 01:33:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:33:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 02 Feb 2020 01:33:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 02 Feb 2020 01:48:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sun, 02 Feb 2020 01:48:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 01:48:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 01:48:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sun, 02 Feb 2020 01:48:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sun, 02 Feb 2020 01:48:50 GMT
ENV PHP_VERSION=7.4.2
# Sun, 02 Feb 2020 01:48:50 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Sun, 02 Feb 2020 01:48:50 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Sun, 02 Feb 2020 01:49:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 01:49:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 02 Feb 2020 01:56:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sun, 02 Feb 2020 01:56:57 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sun, 02 Feb 2020 01:56:59 GMT
RUN docker-php-ext-enable sodium
# Sun, 02 Feb 2020 01:56:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 02 Feb 2020 01:56:59 GMT
WORKDIR /var/www/html
# Sun, 02 Feb 2020 01:57:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sun, 02 Feb 2020 01:57:01 GMT
STOPSIGNAL SIGQUIT
# Sun, 02 Feb 2020 01:57:02 GMT
EXPOSE 9000
# Sun, 02 Feb 2020 01:57:02 GMT
CMD ["php-fpm"]
# Sun, 02 Feb 2020 11:48:45 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Sun, 02 Feb 2020 11:48:45 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 02 Feb 2020 11:50:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:50:33 GMT
VOLUME [/var/www/html]
# Sun, 02 Feb 2020 11:50:33 GMT
ENV JOOMLA_VERSION=3.9.15
# Sun, 02 Feb 2020 11:50:33 GMT
ENV JOOMLA_SHA512=d68e32de6cfe9af92ff7f7991c9253a4487832e55e32e6f74f2b4d592a4777f3b4d8bd74dcd0b10d4262c5e39bdad1e9f7698dedb2ef2989dbc06aa7ab2f6c69
# Sun, 02 Feb 2020 11:50:39 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 02 Feb 2020 11:50:40 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Sun, 02 Feb 2020 11:50:40 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 02 Feb 2020 11:50:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 02 Feb 2020 11:50:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0193cddf0dacef353a98632490e6784d5095e706edcb983fcee6ec51374d4e`  
		Last Modified: Sun, 02 Feb 2020 04:18:24 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f1ce80033990dddefaab407e414c32c56e517edc78604a6fc39c2acd3b7b59`  
		Last Modified: Sun, 02 Feb 2020 04:18:52 GMT  
		Size: 81.2 MB (81198555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d6c8fa8b704d1717c63218688cdf03db3ffac7714f4e5590adf18ff5b6b039`  
		Last Modified: Sun, 02 Feb 2020 04:18:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903ab0763f0e845af5053b9ac5cc4edaa51fa1d1cedd41052230050d9fc30768`  
		Last Modified: Sun, 02 Feb 2020 04:19:51 GMT  
		Size: 10.6 MB (10572234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f43b643e00c7cdb850962c8e7171074d70dbeb8e6ec19e30ca629dd913d2a28`  
		Last Modified: Sun, 02 Feb 2020 04:19:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496f1dbcb479b9a5070e21e60d22747fffe800c7940cb3fc11e58f36e4410320`  
		Last Modified: Sun, 02 Feb 2020 04:20:02 GMT  
		Size: 29.1 MB (29114998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2c8611e5afdfc8c7d1f55821305516487497eef8ad8f9f51b12de139a95b1`  
		Last Modified: Sun, 02 Feb 2020 04:19:47 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c85a0e8a3d5f331e8083f4058b18a7310fcd6f822637f0efdab65cf531c9981`  
		Last Modified: Sun, 02 Feb 2020 04:19:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c4a4bb198824066d4f29318bf4916de26eec1830b92b665accf4bd0a8711d7`  
		Last Modified: Sun, 02 Feb 2020 04:19:47 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca3a14746b8a17585e5af86248f6ebf3cab33bb6a22a9f2a78c83ac2cae9691`  
		Last Modified: Sun, 02 Feb 2020 11:52:56 GMT  
		Size: 3.4 MB (3435849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd754a9f9d6a36445a28e840398c190b61f2ebc6a1831813c558a404882d1059`  
		Last Modified: Sun, 02 Feb 2020 11:53:01 GMT  
		Size: 9.7 MB (9651961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9329ad45428c78c9141bf63f72d4e32c3bbf3d67ef3f5f5d28134be9e1038640`  
		Last Modified: Sun, 02 Feb 2020 11:52:55 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d9537058d9f6601122312aab841279eb7ebd4b3bec3b8d5f7bd48c258d5e1c`  
		Last Modified: Sun, 02 Feb 2020 11:52:55 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.4-fpm` - linux; ppc64le

```console
$ docker pull joomla@sha256:cd3e23fbd98fa62c4340b107d63781b3bb983ca3f54df267733f649dc423d7e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.8 MB (166820948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:674b8f8f62e25048e196e0946ea2b231d25a25998a60c42caefd811dfa8f2dd5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:56:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 02 Feb 2020 08:56:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 02 Feb 2020 08:58:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 02 Feb 2020 08:58:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 02 Feb 2020 09:11:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sun, 02 Feb 2020 09:11:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 09:11:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 02 Feb 2020 09:11:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sun, 02 Feb 2020 09:11:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sun, 02 Feb 2020 09:11:47 GMT
ENV PHP_VERSION=7.4.2
# Sun, 02 Feb 2020 09:11:52 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Sun, 02 Feb 2020 09:11:57 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Sun, 02 Feb 2020 09:13:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:13:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:17:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sun, 02 Feb 2020 09:17:21 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:17:25 GMT
RUN docker-php-ext-enable sodium
# Sun, 02 Feb 2020 09:17:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 02 Feb 2020 09:17:33 GMT
WORKDIR /var/www/html
# Sun, 02 Feb 2020 09:17:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sun, 02 Feb 2020 09:17:44 GMT
STOPSIGNAL SIGQUIT
# Sun, 02 Feb 2020 09:17:46 GMT
EXPOSE 9000
# Sun, 02 Feb 2020 09:17:47 GMT
CMD ["php-fpm"]
# Sun, 02 Feb 2020 19:28:10 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Sun, 02 Feb 2020 19:28:14 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 02 Feb 2020 19:30:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 19:30:46 GMT
VOLUME [/var/www/html]
# Sun, 02 Feb 2020 19:30:48 GMT
ENV JOOMLA_VERSION=3.9.15
# Sun, 02 Feb 2020 19:30:53 GMT
ENV JOOMLA_SHA512=d68e32de6cfe9af92ff7f7991c9253a4487832e55e32e6f74f2b4d592a4777f3b4d8bd74dcd0b10d4262c5e39bdad1e9f7698dedb2ef2989dbc06aa7ab2f6c69
# Sun, 02 Feb 2020 19:31:07 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 02 Feb 2020 19:31:09 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Sun, 02 Feb 2020 19:31:10 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 02 Feb 2020 19:31:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 02 Feb 2020 19:31:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966ccdc0aecd2b2408b79193c2e5da4621b70dd05cb33f690a6085cbd68d828`  
		Last Modified: Sun, 02 Feb 2020 11:04:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80918ab44a55db4cf3524614dbdcea0931538e382d9c436c05ef5c2052a79993`  
		Last Modified: Sun, 02 Feb 2020 11:05:22 GMT  
		Size: 82.3 MB (82259405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2941531c52c5a3060bb214f05618924812516ae9a5686b18eb72ecfb2d072f1`  
		Last Modified: Sun, 02 Feb 2020 11:04:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d36ec41a0458549a73f0e10be367773919bf9e11b43ad2a5d63b751b668fd4`  
		Last Modified: Sun, 02 Feb 2020 11:07:30 GMT  
		Size: 10.6 MB (10572751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f867385d53d1c8b646084c2c0a8cb7b4130781ba249e5cacc73932691c3d147`  
		Last Modified: Sun, 02 Feb 2020 11:07:23 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2a96d4f74e5d9c38b4f0ac4c4735dfd909228aa6d90f4024d4e7eff4c03d7b`  
		Last Modified: Sun, 02 Feb 2020 11:07:35 GMT  
		Size: 30.2 MB (30213259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b68e0d42306a6d04fc6c58a873513dec2659061e1cc88fcb50cb93b0de7312`  
		Last Modified: Sun, 02 Feb 2020 11:07:23 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833359402e10b4b44a907952c4697ede48a2a98c4aa97b2c4ea93559ef1c5f7`  
		Last Modified: Sun, 02 Feb 2020 11:07:23 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfed84b14c6ea09e291444047be2893924c5bfa39c0a93781a1fb83fadf3764`  
		Last Modified: Sun, 02 Feb 2020 11:07:23 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b562e18cf217db77b0a0c91312ae8f698613e2bd37199690da4f5fa7232c9bc`  
		Last Modified: Sun, 02 Feb 2020 19:35:31 GMT  
		Size: 3.6 MB (3592211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6267ae3647d5a89ca095000bc49a16b9e6c3af10adf661fa839e3de4ab7a0801`  
		Last Modified: Sun, 02 Feb 2020 19:35:34 GMT  
		Size: 9.7 MB (9651964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8122423321719854cf57e8fc388d19b76b8ecc52cff33166f9771a5a173b8d0`  
		Last Modified: Sun, 02 Feb 2020 19:35:29 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac30b0e2a134fc04387b80bcd44ee78567289f030d4f4dff1e220d11e0d711b`  
		Last Modified: Sun, 02 Feb 2020 19:35:29 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
