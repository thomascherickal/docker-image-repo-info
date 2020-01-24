## `matomo:3-fpm`

```console
$ docker pull matomo@sha256:5659cbf72e2231696f72bd48c6825e122e8ff896a4de4e81ea0ef97077cd6ca9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `matomo:3-fpm` - linux; amd64

```console
$ docker pull matomo@sha256:767a472094c5d38308ff48806bbd189c05c07fcd642d1f92a43748bda0e043c7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161602839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0ccd51747b4b5916fff8b3118228ea3c06a040e04f70712350684cf106f0c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:51:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Dec 2019 20:51:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:51:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:51:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 20:51:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 28 Dec 2019 20:51:49 GMT
ENV PHP_VERSION=7.4.1
# Sat, 28 Dec 2019 20:51:49 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 20:51:50 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Sat, 28 Dec 2019 20:51:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 20:51:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 20:57:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 20:57:52 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sat, 28 Dec 2019 20:57:52 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 20:57:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 20:57:53 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 20:57:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 Dec 2019 20:57:54 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Dec 2019 20:57:54 GMT
EXPOSE 9000
# Sat, 28 Dec 2019 20:57:54 GMT
CMD ["php-fpm"]
# Thu, 16 Jan 2020 21:34:47 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 16 Jan 2020 21:36:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 21:36:04 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Jan 2020 21:36:05 GMT
ENV MATOMO_VERSION=3.13.1
# Thu, 16 Jan 2020 21:36:16 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 21:36:16 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 16 Jan 2020 21:36:17 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 16 Jan 2020 21:36:17 GMT
VOLUME [/var/www/html]
# Thu, 16 Jan 2020 21:36:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jan 2020 21:36:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde71bc845230432bf883ccbb431cd814e383bf03e78d30e81daffc7f343d810`  
		Last Modified: Sat, 28 Dec 2019 22:54:29 GMT  
		Size: 10.6 MB (10566979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5516e8ce42c85da8fd89f38d2c8d8d79d07269fe37a90d32080c55b6189d5bd7`  
		Last Modified: Sat, 28 Dec 2019 22:54:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604a9e51e1d88fb78d248c2c4426c4a85a823beef53306120a1f64a69c59d189`  
		Last Modified: Sat, 28 Dec 2019 22:54:33 GMT  
		Size: 28.5 MB (28521424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cc99a1fbdfeaf80ab83434e7f05f0e1116c425a7484e7711a5846880b777fe`  
		Last Modified: Sat, 28 Dec 2019 22:54:27 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b20909973e002e3265498d1a98f9700d1dbc75d3eef9d732c03d11b970b12b`  
		Last Modified: Sat, 28 Dec 2019 22:54:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a968bad60a038b1581d12847baf30e6648769861a8f2b916b52c285e634ca`  
		Last Modified: Sat, 28 Dec 2019 22:54:27 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137a3dbe04bcb2d38f1ff1b5ba666f58ef76bf4645e123871e58cf08468a7e5`  
		Last Modified: Thu, 16 Jan 2020 21:38:24 GMT  
		Size: 3.4 MB (3361793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10364673a658ff39bcb125e12981c0e1303744306040bee3372153f0179cb70`  
		Last Modified: Thu, 16 Jan 2020 21:38:23 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecc777615eda99bd12ef79b7f0da03091769ebab093d10d0dfeff4eeee93958`  
		Last Modified: Thu, 16 Jan 2020 21:38:27 GMT  
		Size: 15.4 MB (15396051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002138270903974f2ce6fb3b01a0409dfdd3d6c76f39ec649e91cb044a821557`  
		Last Modified: Thu, 16 Jan 2020 21:38:23 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c75c20751e384bf00e8262a71cb11a4757c02899bf0aeb241d1d75131fb7c2`  
		Last Modified: Thu, 16 Jan 2020 21:38:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:3-fpm` - linux; arm variant v5

```console
$ docker pull matomo@sha256:2b4f4e17f8274af64b3d06887e4aaed9550f8480e756d776ad64556a8f33a65e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139940769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:374f773e9c080714d8ab4419ca8423d8c51e26fc92eddb2f5f55e915e5842d0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:56:15 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Dec 2019 11:56:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:56:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:56:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 11:56:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 20:38:19 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 20:38:20 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 20:38:20 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 20:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 20:38:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:43:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 20:43:11 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:43:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 20:43:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 20:43:18 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 20:43:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Jan 2020 20:43:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 20:43:24 GMT
EXPOSE 9000
# Thu, 23 Jan 2020 20:43:25 GMT
CMD ["php-fpm"]
# Thu, 23 Jan 2020 23:12:01 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 23 Jan 2020 23:14:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jan 2020 23:14:31 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Jan 2020 23:14:31 GMT
ENV MATOMO_VERSION=3.13.1
# Thu, 23 Jan 2020 23:15:03 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jan 2020 23:15:06 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 23 Jan 2020 23:15:07 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 23 Jan 2020 23:15:09 GMT
VOLUME [/var/www/html]
# Thu, 23 Jan 2020 23:15:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:15:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd6af660d9e99000bef10669ba5fd8bbf71e5fc11c2ec4fd785ea3aeff19e24`  
		Last Modified: Thu, 23 Jan 2020 22:03:06 GMT  
		Size: 10.6 MB (10571031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d8ee7d040f220e74091c5b0b3378fc047d65c7fa56b2fc4c730c72c33522e`  
		Last Modified: Thu, 23 Jan 2020 22:03:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3170b82583f5d8da9ba971aff471ae17e4e2b94802d1e88bd4095006def88b9e`  
		Last Modified: Thu, 23 Jan 2020 22:03:11 GMT  
		Size: 27.2 MB (27151840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc38a5aeda47d37a709bf2f120249e5ed9e50d834f98c5b5c6c186fdecf3f0a3`  
		Last Modified: Thu, 23 Jan 2020 22:03:02 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec96ab1186beb3135acfc9c297d0d0a63133dcb15cb304adf899b8d2220ab6c`  
		Last Modified: Thu, 23 Jan 2020 22:03:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d5a5c2ff6cb1f7b8cb01b5f3b8d0e5cec081e8a773407ae1d2e200d03560d4`  
		Last Modified: Thu, 23 Jan 2020 22:03:02 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9262fd16e30a4813d1766194f3474705f787330033fd8357f36209f6cef82732`  
		Last Modified: Thu, 23 Jan 2020 23:16:04 GMT  
		Size: 3.2 MB (3181471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da41f7891959d67b52625899a177887a73472e73683aaa9cdb68a352bddc913`  
		Last Modified: Thu, 23 Jan 2020 23:16:03 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f18a0c9045b92c79b49ea28914fc032801af74c10a420828dc194fc37fe3a0`  
		Last Modified: Thu, 23 Jan 2020 23:16:10 GMT  
		Size: 15.4 MB (15394781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7a704d3faf8b0d900c6a1a60f2b58acd350497db6c68e18497342688b8e690`  
		Last Modified: Thu, 23 Jan 2020 23:16:03 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52b3924899d9aa007e80526005225ce1b3f3ac5666a9fd44a8f3ef7dea629a2`  
		Last Modified: Thu, 23 Jan 2020 23:16:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:3-fpm` - linux; arm variant v7

```console
$ docker pull matomo@sha256:26abf4859357a8277450ec2fb1d24839d80ed7515207cf3b81507ee924b19f9d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137397728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:218261aea682cca8d42a283345a03091b619415202ee012aea23df873b016610`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:51:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Dec 2019 15:51:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:51:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:51:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:51:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 21:22:37 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 21:22:38 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:22:39 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 21:22:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:22:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:26:17 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:26:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:26:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:26:23 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:26:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Jan 2020 21:26:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jan 2020 21:26:29 GMT
EXPOSE 9000
# Thu, 23 Jan 2020 21:26:29 GMT
CMD ["php-fpm"]
# Fri, 24 Jan 2020 06:28:29 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 24 Jan 2020 06:30:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 06:30:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 06:30:46 GMT
ENV MATOMO_VERSION=3.13.1
# Fri, 24 Jan 2020 06:31:20 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 06:31:24 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 24 Jan 2020 06:31:24 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 24 Jan 2020 06:31:25 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 06:31:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:31:26 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b687d8d7383a9f62078b9ecdf892f55bc55bf83cf2a4e8df17eb9c09ca516`  
		Last Modified: Thu, 23 Jan 2020 23:40:47 GMT  
		Size: 10.6 MB (10571111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8165153535b7b8f8ad4085dbd79237cf045fc9bd2bdd55f99e6797b1fe88ec44`  
		Last Modified: Thu, 23 Jan 2020 23:40:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ba716e2fd2135878ea266437e3bfe177747a965c207c3ba7414b16c4afb58f`  
		Last Modified: Thu, 23 Jan 2020 23:40:48 GMT  
		Size: 26.2 MB (26170147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84342661b0691498b9bc29bf82f7aa3604d0700eb9bd4e7115c32f0efb022be`  
		Last Modified: Thu, 23 Jan 2020 23:40:40 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528d0cbd761e58e6da8022837859dbfd19db51ba4cf630d837ea0cffc74bd3e`  
		Last Modified: Thu, 23 Jan 2020 23:40:39 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987652c3ae330e8519e45c2968cd3f4d68a121872f70d67daea8efb4e7287374`  
		Last Modified: Thu, 23 Jan 2020 23:40:40 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190851826bde7084023a1e44b60adf291239c50ddccead87fcfdeebc07c9db69`  
		Last Modified: Fri, 24 Jan 2020 06:34:55 GMT  
		Size: 3.0 MB (3048714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fd384f5e3aa67d89a0730fd1208584b1dc3ef0ef2a1b670d2043009a194e4a`  
		Last Modified: Fri, 24 Jan 2020 06:34:54 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f6927d28592f7499bc27c4247a802078c7b49f36bbc003e44f87c76a7ff800`  
		Last Modified: Fri, 24 Jan 2020 06:35:01 GMT  
		Size: 15.4 MB (15394931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff3c69031ad095b6837c3f54521dd73fc45dc4d724d6804eb3e988fe4f1d541`  
		Last Modified: Fri, 24 Jan 2020 06:34:54 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f43ead245c97fe3918c425af6638ab4645caf05b96c9138e20bf6a0ab3daad`  
		Last Modified: Fri, 24 Jan 2020 06:34:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:3-fpm` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:613325ae2d8d7f6b61f73da7327f4dedb1de04315db0d64d0723a5487297b82f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153748229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a114f39c58c6c9303c0f223b6f99ac083b9a2a9abca500163ace46d4081d0a5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:43:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Dec 2019 14:44:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:44:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:44:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 14:44:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Jan 2020 00:00:35 GMT
ENV PHP_VERSION=7.4.2
# Fri, 24 Jan 2020 00:00:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 00:00:37 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Fri, 24 Jan 2020 00:00:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jan 2020 00:00:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 00:04:47 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:04:49 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 00:04:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 00:04:51 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 00:04:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 24 Jan 2020 00:04:54 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Jan 2020 00:04:56 GMT
EXPOSE 9000
# Fri, 24 Jan 2020 00:04:57 GMT
CMD ["php-fpm"]
# Fri, 24 Jan 2020 04:26:04 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 24 Jan 2020 04:28:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 04:28:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 04:28:08 GMT
ENV MATOMO_VERSION=3.13.1
# Fri, 24 Jan 2020 04:28:33 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 04:28:35 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 24 Jan 2020 04:28:36 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 24 Jan 2020 04:28:37 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 04:28:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 04:28:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a31ea7708bcc36cc2941588ea7167c09de8d5f992d42d5989c5668220f5cf8`  
		Last Modified: Fri, 24 Jan 2020 02:36:55 GMT  
		Size: 10.6 MB (10571859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae3d6b3e9e71aae42eadc8bde947a7b3b2c3349444df100b4f1b0a495936359`  
		Last Modified: Fri, 24 Jan 2020 02:36:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de01132f62cf1a207196d3acce3357273ee7ec9161e69a805618e3493cacd6f4`  
		Last Modified: Fri, 24 Jan 2020 02:36:57 GMT  
		Size: 28.3 MB (28276553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1ac2e9f2d0d6b9d2944380c403f244153bf546273af0b34d59af7c24fc8532`  
		Last Modified: Fri, 24 Jan 2020 02:36:49 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a6b5b0c6850ede6043a0b682fae318a28d53b0475912296814eb1e55c55de0`  
		Last Modified: Fri, 24 Jan 2020 02:36:50 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583dfc03518d0a7cd7910fcddc528c8c09eec261e8f29e4782efffb69883500f`  
		Last Modified: Fri, 24 Jan 2020 02:36:50 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba3919ea36bfd38f916b232e55d15205584a3fc984b4b32d69fbd96c2c8da2`  
		Last Modified: Fri, 24 Jan 2020 04:32:11 GMT  
		Size: 3.3 MB (3305674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43abd342e9ed9e4759ecbf38fd662cf8d87ca58fa173636c13ea1f4006d36f13`  
		Last Modified: Fri, 24 Jan 2020 04:32:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404cf8a5d6addca57c17b10670dc8be7d47cfe72ad7587dc6cc647a65eb62ee`  
		Last Modified: Fri, 24 Jan 2020 04:32:21 GMT  
		Size: 15.4 MB (15395437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd816e4889df9c6ce3101d93a7b500c1cc883afd6ae1a040f6b98e0ed5807ceb`  
		Last Modified: Fri, 24 Jan 2020 04:32:10 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ade7bc60dc6309c15d811e81bd54ffe7f8078355d6d02f29d1e1ae65b78361`  
		Last Modified: Fri, 24 Jan 2020 04:32:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:3-fpm` - linux; 386

```console
$ docker pull matomo@sha256:a4af9ba5d748a5481532bc979400bf6f351620d4f201bbb43c308b798cd522c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167419173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d033bc00fb0b55914cc03ac2229a65c8174aea6d8da33a09549b69fce6ef26c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 17:02:05 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Dec 2019 17:02:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 17:02:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 17:02:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 17:02:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 28 Dec 2019 17:02:06 GMT
ENV PHP_VERSION=7.4.1
# Sat, 28 Dec 2019 17:02:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 17:02:06 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Sat, 28 Dec 2019 17:02:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 17:02:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:10:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 17:10:05 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:10:06 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 17:10:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 17:10:06 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 17:10:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 Dec 2019 17:10:07 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Dec 2019 17:10:08 GMT
EXPOSE 9000
# Sat, 28 Dec 2019 17:10:08 GMT
CMD ["php-fpm"]
# Thu, 16 Jan 2020 21:40:29 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 16 Jan 2020 21:41:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 21:41:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Jan 2020 21:41:58 GMT
ENV MATOMO_VERSION=3.13.1
# Thu, 16 Jan 2020 21:42:11 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 21:42:12 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 16 Jan 2020 21:42:12 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 16 Jan 2020 21:42:12 GMT
VOLUME [/var/www/html]
# Thu, 16 Jan 2020 21:42:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jan 2020 21:42:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5a919dbab8e76ea3c1d71a307d23a2327aa2a2c7a91b22a484139c2a5c01ae`  
		Last Modified: Sat, 28 Dec 2019 19:33:24 GMT  
		Size: 10.6 MB (10566314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f82c1d79942ac219c246e8ffa479027726b5bf8e7d070de05926184ffa1aaf`  
		Last Modified: Sat, 28 Dec 2019 19:33:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7f348159fd84e253361ddec67bdacba524700a3187e80bbd05b3e30e4afcfe`  
		Last Modified: Sat, 28 Dec 2019 19:33:30 GMT  
		Size: 29.1 MB (29107093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8b0a9d1bf273d766da99dc902cfa5dd446a67c29455bbdb631b274b9a61d2b`  
		Last Modified: Sat, 28 Dec 2019 19:33:22 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6322e81fded07d654128b912413e9eb38a00c0a52131a02b748e6a88da7064b`  
		Last Modified: Sat, 28 Dec 2019 19:33:22 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed5b51247c2a45836c947680410f70610ed71e66b09dda70d99fe56355f534e`  
		Last Modified: Sat, 28 Dec 2019 19:33:22 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e2562bee39efaea8b997e26cf335849c49c4a3bb822b42aa1f9c3130f2ed44`  
		Last Modified: Thu, 16 Jan 2020 21:44:33 GMT  
		Size: 3.4 MB (3390956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eac2a44267ea0ecbfdf3579bc4887ef6c61dcbe8fcaf1ae1be7cf07ce3cc9f`  
		Last Modified: Thu, 16 Jan 2020 21:44:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4c6893d37da31903d752df7ea5c6a0b1f5dc307db9581cacdc9374bcbdeb3a`  
		Last Modified: Thu, 16 Jan 2020 21:44:37 GMT  
		Size: 15.4 MB (15395594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6d3b0ce82c38e1b13bf04cc0aeb4bb7090f09d92077547dbba249af84eea8`  
		Last Modified: Thu, 16 Jan 2020 21:44:32 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c302b93157675aa96a64b7abe9983f13c961cdd9704f423b67400feee6747b0d`  
		Last Modified: Thu, 16 Jan 2020 21:44:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:3-fpm` - linux; ppc64le

```console
$ docker pull matomo@sha256:160aba3a9fe59ae37d3f8b6fe4d1dd0e19b81458b242a95de760721d8affb39c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172541007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad984ad10fa9661477804b2274ab33b90dcc74b3e0e4d97e24e16a225fbf4fcf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:23:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Dec 2019 18:23:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:23:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:24:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:24:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 28 Dec 2019 18:24:06 GMT
ENV PHP_VERSION=7.4.1
# Sat, 28 Dec 2019 18:24:09 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:24:11 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Sat, 28 Dec 2019 18:24:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:24:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:28:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:28:38 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:28:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:28:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:28:47 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:28:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 Dec 2019 18:28:54 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Dec 2019 18:28:56 GMT
EXPOSE 9000
# Sat, 28 Dec 2019 18:29:01 GMT
CMD ["php-fpm"]
# Thu, 16 Jan 2020 21:23:22 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 16 Jan 2020 21:25:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 21:26:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Jan 2020 21:26:02 GMT
ENV MATOMO_VERSION=3.13.1
# Thu, 16 Jan 2020 21:27:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 21:27:39 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 16 Jan 2020 21:27:41 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 16 Jan 2020 21:27:49 GMT
VOLUME [/var/www/html]
# Thu, 16 Jan 2020 21:27:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jan 2020 21:27:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc925df6a87c7db5d2b780b49a27b8e982cd41a30dd42a8fef2d0d7a861ef0`  
		Last Modified: Sat, 28 Dec 2019 20:13:56 GMT  
		Size: 10.6 MB (10566744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a277e12905c6123168c319119e6f6ce6f2de820a58e5a1c25ebdbf6b70bb14c6`  
		Last Modified: Sat, 28 Dec 2019 20:13:51 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9203de1d5edcf641aad320681a2509e056a309c949aa02bdb83d587ad44b5e24`  
		Last Modified: Sat, 28 Dec 2019 20:14:02 GMT  
		Size: 30.2 MB (30206658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8318f94b7b20d83b4f1645b95179350a8d3b78b1994028ccf02cd8f2994a230f`  
		Last Modified: Sat, 28 Dec 2019 20:13:51 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18854ae1587090aa5fdabc26abb045c3041402966f83b69532ab7b1019c544d9`  
		Last Modified: Sat, 28 Dec 2019 20:13:51 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965a8048328e47dc2b820c5d49c1632329483f043e1765df8585d7314eceb55a`  
		Last Modified: Sat, 28 Dec 2019 20:13:51 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6197ed2a2b98cebaa087cb5fd9079bc5a9a318c6da96658ecf552febec87187c`  
		Last Modified: Thu, 16 Jan 2020 21:32:37 GMT  
		Size: 3.6 MB (3581500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475f711164369e809a57c52a74a521c88b297d970ffcc7ba520a2de1702c245f`  
		Last Modified: Thu, 16 Jan 2020 21:32:36 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667c3ab45bacb3e6de2864a0835d7a5ba95684b4a33790c4e476f37c36848699`  
		Last Modified: Thu, 16 Jan 2020 21:32:41 GMT  
		Size: 15.4 MB (15396334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64cdc8a2ba2705782fdf14730933457940c7981adffb5bc9491b67066a717152`  
		Last Modified: Thu, 16 Jan 2020 21:32:36 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce38a97d05af18f3c40648384e255b966048e012ffbbaf5fd21973caa2b6ce14`  
		Last Modified: Thu, 16 Jan 2020 21:32:36 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
