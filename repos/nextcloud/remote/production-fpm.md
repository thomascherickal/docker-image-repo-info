## `nextcloud:production-fpm`

```console
$ docker pull nextcloud@sha256:1de897f150d56a47902acdcf1ec8bd88dda57f157c34aafb439c3937d67133f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `nextcloud:production-fpm` - linux; amd64

```console
$ docker pull nextcloud@sha256:bc725dd9728726800651c10c2ce3140b46b93b75e315333dde347e0e59f63f56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.5 MB (276518478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71e29227b3144628285950f76fd72fea893b5b6c4b20a362ee52553da3a067e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:55:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 18:55:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 18:55:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:55:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 18:55:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 19:14:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 19:14:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 19:14:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 19:14:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 19:42:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 19:42:28 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 19:42:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 19:42:29 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 19:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 19:42:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 19:50:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 19:50:23 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 19:50:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 19:50:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 19:50:26 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 19:50:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 19:50:28 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 19:50:28 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 19:50:29 GMT
CMD ["php-fpm"]
# Wed, 10 Feb 2021 09:16:41 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 22:14:57 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 22:14:58 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 22:17:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 22:17:52 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 22:17:52 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 22:22:04 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 22:22:40 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 22:22:41 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 22:22:42 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 22:22:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 22:22:42 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48991d6909cf720506106468cbe52f0eec8e1c809d7684429ffca6503fcebf1`  
		Last Modified: Tue, 09 Feb 2021 20:43:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935e2abd2c2c402808fff904dbd8a4a40328ef5be78063cae8fa3b780383e266`  
		Last Modified: Tue, 09 Feb 2021 20:43:27 GMT  
		Size: 76.7 MB (76677231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ccf45ccdb967c3157f2b65cb4fd4f821bb329dc5cbb0192423518ab73ceae6`  
		Last Modified: Tue, 09 Feb 2021 20:43:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca77472e81fb836f3d8f6b522a8ac515c1fd3aa74b6380c1dcaa879b15b58419`  
		Last Modified: Tue, 09 Feb 2021 20:45:26 GMT  
		Size: 10.7 MB (10653097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53f6cf96a486872bfc8480fbe3e8d34eaee06b6b6f8ebe89222a40c971b1b31`  
		Last Modified: Tue, 09 Feb 2021 20:45:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffe6e27dddcf013411e3339c2e6253d8569095d99a1d789ae6fc5c7d590e45e`  
		Last Modified: Tue, 09 Feb 2021 20:45:30 GMT  
		Size: 28.6 MB (28569574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f028ee70866e3615631ca01dc98c62ae9584742a18fc5b24189ef4709632c`  
		Last Modified: Tue, 09 Feb 2021 20:45:24 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0fa1ec27ac062ac250770696f2d291c9578280e031e679ca4e4a01969610a2`  
		Last Modified: Tue, 09 Feb 2021 20:45:24 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f590763005b14d428a484db3d2fdb8a2eed3254ac5818eda6cb5ea718c70bb76`  
		Last Modified: Tue, 09 Feb 2021 20:45:24 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0571229d9cee5ee1e468d72e7f9734a5fe14464592c7c8e5ac73da1d1b10f1ad`  
		Last Modified: Wed, 10 Feb 2021 09:28:59 GMT  
		Size: 1.6 MB (1635819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927bad147e4e79b95f9c2b9d1a16686c33c37b3ec5dd1746a94bed12eeb151b2`  
		Last Modified: Fri, 19 Feb 2021 22:30:27 GMT  
		Size: 16.5 MB (16530552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6efe8b417056d406fc1a752983fbc1cec9514302a4dd1ceab935ea4a0ccaa0`  
		Last Modified: Fri, 19 Feb 2021 22:30:22 GMT  
		Size: 565.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225a2e850453c1f22dff556b9289d1b1804a9677b4933b45cb9d1c550bc25f06`  
		Last Modified: Fri, 19 Feb 2021 22:34:10 GMT  
		Size: 115.3 MB (115340171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0f894ecf5cdbff84d6be0a976efafd08870ef1982c5e588f3bded7d7c66452`  
		Last Modified: Fri, 19 Feb 2021 22:33:42 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2a017776fc73b4e7e0c05d183ae4d909ad1923bd67fc8e12e959e9c6511ab`  
		Last Modified: Fri, 19 Feb 2021 22:33:42 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:a311309e036156eccaf7266173c2b9ea9233d3c175298d9f90461a341b781baa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.5 MB (253515999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae41f072245fb232fef2e554391217a21964f9aafc15b169979d12268c05eef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:40:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 09:40:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 09:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 09:41:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 09:50:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 09:50:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 09:50:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 09:50:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 10:05:52 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 10:05:53 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 10:05:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 10:05:54 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 10:06:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 10:06:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 10:09:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 10:09:36 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 10:09:38 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 10:09:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 10:09:39 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 10:09:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 10:09:42 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 10:09:43 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 10:09:44 GMT
CMD ["php-fpm"]
# Tue, 09 Feb 2021 16:13:16 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 19:56:03 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 19:56:04 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:01:26 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:01:29 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:01:29 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:07:55 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:09:10 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:09:16 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:09:19 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:09:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:09:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479d20320ef94e865807f24ef2b2ed4435c3b8f9a45286e13b963422bb31030e`  
		Last Modified: Tue, 09 Feb 2021 10:48:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f378ecd0ed69d12360ccc0800e83b3d3d66ca888dacb74bb21b13599b0c51903`  
		Last Modified: Tue, 09 Feb 2021 10:49:14 GMT  
		Size: 58.8 MB (58814766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fba887c8789cfa67533944f9e7d2e966cf5d283331b7a74d9c4a4ba2b0fe83`  
		Last Modified: Tue, 09 Feb 2021 10:48:55 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f01ab417c99149dda135c436487b29d448620dc0ffe8d3cf29b096d6023417d`  
		Last Modified: Tue, 09 Feb 2021 10:51:46 GMT  
		Size: 10.7 MB (10651424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d595da9cd1d7c0687afa55fd7284a8fbfdc1441eda6e6faaaab1ba3d2ae83d`  
		Last Modified: Tue, 09 Feb 2021 10:51:43 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9fcb249e9bb77200b5420aa546bc2fd4cad18cef51bf3cc7cc3a3b8a3dc92b`  
		Last Modified: Tue, 09 Feb 2021 10:51:51 GMT  
		Size: 27.2 MB (27184784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071cbb62120801280aea79aeb1898944270d0aecc3a99ed6b9c41616128ce6c3`  
		Last Modified: Tue, 09 Feb 2021 10:51:43 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f71ffc9d32a0a08b50f990d7f9a327c9e615ff584073825d87b1260423c89d`  
		Last Modified: Tue, 09 Feb 2021 10:51:43 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace84cc4b78c8654a0a3ee47642598819b26759e3c61a9cd001789d8381b6e2c`  
		Last Modified: Tue, 09 Feb 2021 10:51:44 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98794d3a2cac6b4975eba2337180efc29b442e7fdcbec479cfb71710bfbef6c4`  
		Last Modified: Tue, 09 Feb 2021 16:29:05 GMT  
		Size: 1.6 MB (1573604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eb395bd7a13c65aebcd091a42f04bf0d587815dd1358fd05741b4c352751f5`  
		Last Modified: Fri, 19 Feb 2021 20:17:59 GMT  
		Size: 15.1 MB (15096745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80380e8009e99792e26b55fe94a05e6115a474c074a2c3fc54ed96efe9f9556`  
		Last Modified: Fri, 19 Feb 2021 20:17:53 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5899b436ac53449945e37b946eda5a64f3e7ef110a04c43df63d3f272b0fdbb2`  
		Last Modified: Fri, 19 Feb 2021 20:22:09 GMT  
		Size: 115.3 MB (115338427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acef2a218e1313c451c3cf27ff4f48da614f4ef4ae8c01426e76b1d217eb4ad`  
		Last Modified: Fri, 19 Feb 2021 20:21:28 GMT  
		Size: 2.5 KB (2530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ff6aa076c7d4048a5701c543b91fabfd8c0a84943407af3e778c6481401a88`  
		Last Modified: Fri, 19 Feb 2021 20:21:29 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:1d76a67f2577319a59b3bc44658addeef55d8f88fb71432ce636f8994c1da219
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249883455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d8b505ba4514f528989cd22cd6122017abbc67e224b22db3b6b4e322679be6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:54:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 11:54:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 11:55:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:55:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 11:55:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 12:03:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 12:03:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 12:03:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 12:03:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 12:17:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 12:17:03 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 12:17:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 12:17:05 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 12:17:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 12:17:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 12:20:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 12:20:15 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 12:20:17 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 12:20:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 12:20:19 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 12:20:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 12:20:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 12:20:22 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 12:20:23 GMT
CMD ["php-fpm"]
# Wed, 10 Feb 2021 04:23:16 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 20:58:07 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:58:07 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 21:02:50 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 21:02:54 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 21:02:59 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 21:10:39 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 21:11:41 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 21:11:48 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 21:11:50 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 21:11:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 21:11:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4e7c5500d514905861de5fd68ba2321eb5866e64f8b6689c3ea8129a68b4a2`  
		Last Modified: Tue, 09 Feb 2021 13:00:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30745314a6fe3cad64125db918cc09eadf8b13a570ca225f34f3e36e9fb6110`  
		Last Modified: Tue, 09 Feb 2021 13:01:01 GMT  
		Size: 59.5 MB (59513280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0061ef8da45b5a1732d5c93658be4ee8d9088db791f661832ceabe441b54544b`  
		Last Modified: Tue, 09 Feb 2021 13:00:44 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa0b49a503a6337116d800c6a83ab5f04dcd0fe009fdd2acb1aefbc71fb1253`  
		Last Modified: Tue, 09 Feb 2021 13:03:44 GMT  
		Size: 10.7 MB (10651455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407613ee142f5b2d930ffa81fc96281e99d53975f2b61e17a0334111e723bc25`  
		Last Modified: Tue, 09 Feb 2021 13:03:41 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb21bd56fccfbbf848f7a7227de2dbeed58a060558aa124fcf7392c85e5dbf7`  
		Last Modified: Tue, 09 Feb 2021 13:03:49 GMT  
		Size: 26.2 MB (26197629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c304ad9132ba47a294b555c9d238d01967e08bf10a10b6b909d4397f2722e8`  
		Last Modified: Tue, 09 Feb 2021 13:03:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04fa74e0d70c914303cd732e14bf14873d0aec2706007a9408f984807ce90e6`  
		Last Modified: Tue, 09 Feb 2021 13:03:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086199433eb100a1f520de3c6408427249d6cc2641bf286d14d27e2cedbd71`  
		Last Modified: Tue, 09 Feb 2021 13:03:40 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fc051bb1f810199dab2712264bce7a8035b849e027c3365e9b0799c6d9de9`  
		Last Modified: Wed, 10 Feb 2021 04:44:23 GMT  
		Size: 1.4 MB (1425658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139364cc96c8b122198b7c3f64019af0949516d1d5d45448a4ec17b89f6a8c75`  
		Last Modified: Fri, 19 Feb 2021 21:23:16 GMT  
		Size: 14.0 MB (14036698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc77b02581c33120b6da69453502f5e286845834abfc90f8e0ae64e74ab3f4a`  
		Last Modified: Fri, 19 Feb 2021 21:23:12 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505b66abc91c6a9f5b363d78bfa5074e69abeace6f8609fe0009206573583a39`  
		Last Modified: Fri, 19 Feb 2021 21:28:41 GMT  
		Size: 115.3 MB (115338387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1f50ce494d4bce475245e8074c67da87254b65d100ef82ac3dc4f14abb7000`  
		Last Modified: Fri, 19 Feb 2021 21:28:02 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9c6259de0e99b65d130fb85351deafcf1112b334c8d4575529cad161f9899e`  
		Last Modified: Fri, 19 Feb 2021 21:28:01 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:45c31c0afdcfe9289f0347616f7946ad0fc6cbef99cfdcf5269da112e817fbf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.0 MB (267023851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c44a6ab5261fe31d81e64b841bcb23f31814c5396f7de3ae8cb26ae55c74376`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 13:24:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 13:24:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 13:24:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 13:24:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 13:24:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 13:33:51 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 13:33:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:33:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:33:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 13:49:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 13:49:43 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 13:49:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 13:49:46 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 13:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 13:50:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 13:53:41 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:53:48 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 13:53:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 13:53:50 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 13:53:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 13:53:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 13:53:54 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 13:53:54 GMT
CMD ["php-fpm"]
# Wed, 10 Feb 2021 06:06:02 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 20:39:14 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:39:15 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:43:49 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:43:53 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:43:53 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:50:22 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:51:16 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:51:20 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:51:23 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:51:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:51:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445693bd43e8246a8c166233392b33143f7f5e396c480f74538e5738fb6bd6e`  
		Last Modified: Tue, 09 Feb 2021 14:35:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb0363d084b9a838de3a1ef92a69c34131d0be020cc0474098ea80a07e16b6d`  
		Last Modified: Tue, 09 Feb 2021 14:35:38 GMT  
		Size: 70.4 MB (70355003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87c2495950546c2e82fc496d7c39837a517f3f3095fb87598d1731d0529f907`  
		Last Modified: Tue, 09 Feb 2021 14:35:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1adb288e98c22c27ceab533f4e3971f840884be129e126e644963f9673c797`  
		Last Modified: Tue, 09 Feb 2021 14:38:35 GMT  
		Size: 10.7 MB (10652061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e88e34d21f95da42fe9e3fb71c4040ae0237ceeeae8fc504be0bed90c2f01f6`  
		Last Modified: Tue, 09 Feb 2021 14:38:33 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc06f014cf9aa42afd5ade8070004c7898118541b28b4d2d7028abf07907ea65`  
		Last Modified: Tue, 09 Feb 2021 14:38:41 GMT  
		Size: 28.3 MB (28334008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e87070ee2fafa7ea2e9244d2a532f834f9a72eddbde3a6c8abccdcd6bab687`  
		Last Modified: Tue, 09 Feb 2021 14:38:33 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0b37e16f2e15c7d9c527d7c171e054dc7b4e90b1c1689cff4e78876dcb176`  
		Last Modified: Tue, 09 Feb 2021 14:38:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2142f69ef7db285e1d4bad90ca16a95bd76f684ac6a895ec5965d72bc0b427`  
		Last Modified: Tue, 09 Feb 2021 14:38:33 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d39293833bf213f25773430ed08caf6a657a957ec4703b2f3cacb10b6065482`  
		Last Modified: Wed, 10 Feb 2021 06:26:31 GMT  
		Size: 1.6 MB (1602407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62db4ca10ab0a84da317d46e725eea1fb21252995c6774d17489ab2cda42a395`  
		Last Modified: Fri, 19 Feb 2021 21:02:24 GMT  
		Size: 14.9 MB (14872600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f87f068b2b0238d91d755b8ce54eee9443be0e7ed7b36df53906268b04741`  
		Last Modified: Fri, 19 Feb 2021 21:02:20 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5624e5577a89e631639548b7102e0a9bb67488edc95fa1d57f2056944cda394`  
		Last Modified: Fri, 19 Feb 2021 21:07:07 GMT  
		Size: 115.3 MB (115339365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a077ba182bb0b64fd92be75e078ef69c34c4ac8499da72c90c0f0feccf310e6`  
		Last Modified: Fri, 19 Feb 2021 21:06:40 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccf5857ee231027f30a56fa18ef935a53829bd1302c1b371094257c46174569`  
		Last Modified: Fri, 19 Feb 2021 21:06:38 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; 386

```console
$ docker pull nextcloud@sha256:f79f307f4f412946fa9152b4025583ad0a2beb93d153e9bd5a232a37badf492f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.7 MB (281664122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d0eb02f0c8762fb73c13c7b6803d1d436b842e913542b67b900529105b87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 12:55:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 12:55:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 12:55:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 12:55:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 12:55:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 13:13:15 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 13:13:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:13:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:13:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 13:42:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 13:42:48 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 13:42:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 13:42:49 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 13:43:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 13:43:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:51:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 13:51:45 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:51:47 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 13:51:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 13:51:47 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 13:51:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 13:51:49 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 13:51:49 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 13:51:50 GMT
CMD ["php-fpm"]
# Tue, 09 Feb 2021 22:35:02 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 21:39:07 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 21:39:07 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 21:42:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 21:42:52 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 21:42:52 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 21:49:28 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 21:50:27 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 21:50:28 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 21:50:30 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 21:50:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 21:50:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273ebd73efe18fbe0a9fb3fa3727a6f72bd5edef4eec32f0cdfd91723b6c877`  
		Last Modified: Tue, 09 Feb 2021 15:05:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07347a055a7dbbfecfcbf26edf69115228d399f8c70e5ce9fe2575ac94c9b0c`  
		Last Modified: Tue, 09 Feb 2021 15:06:30 GMT  
		Size: 81.2 MB (81216990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71658904aa5572b07669df7ce20edd1cdbad61f48cd009aff53e9dd64cc748b3`  
		Last Modified: Tue, 09 Feb 2021 15:05:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4674ce3e3824e9bc11353f16fcdfb8060ce07f6c557b76cb9b06f20c47dae66`  
		Last Modified: Tue, 09 Feb 2021 15:09:26 GMT  
		Size: 10.7 MB (10652274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282cf3122b0933484a04cc9c6ec1bacaea592786d537705d50bfc2670cfaa60e`  
		Last Modified: Tue, 09 Feb 2021 15:09:23 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6166dbce770ae39e1344460ad143f73eaf68a6b72681ae0a1f29ef5cb1ac3c2`  
		Last Modified: Tue, 09 Feb 2021 15:09:37 GMT  
		Size: 29.2 MB (29150021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce0058a2b5744bb286b70452fe7b738ae603c0ac7c7c3bfd91138566f0da681`  
		Last Modified: Tue, 09 Feb 2021 15:09:23 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b24060eef390482adf45ece5d6b2f6c6f43f9489f93699a5273a38de8a8541`  
		Last Modified: Tue, 09 Feb 2021 15:09:23 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5660f4558217653866b25531bbc9eaed50c66106a1a5599d9a7ca27bd7b9b140`  
		Last Modified: Tue, 09 Feb 2021 15:09:23 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad01fffce00b843697ed0c6fcf41229dd79dd6841c1f8dce301514501cf130b`  
		Last Modified: Tue, 09 Feb 2021 22:54:14 GMT  
		Size: 1.7 MB (1659767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cf72bad4cbcf38779c5efa5b08723de500d8cc72fb16ff7e13fb3d1dba5bde`  
		Last Modified: Fri, 19 Feb 2021 22:01:43 GMT  
		Size: 15.9 MB (15875974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfdd72d2b9d0f8410f234fc2d19b51ea1b1f4d14e01c7300efb5e9be022d517`  
		Last Modified: Fri, 19 Feb 2021 22:01:33 GMT  
		Size: 564.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a56f9e65e9108be34f135207da3fa4e5e34ca71e13e3c45209c4312693777f4`  
		Last Modified: Fri, 19 Feb 2021 22:07:19 GMT  
		Size: 115.3 MB (115339483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643fc5485e7622ea4d121679d22137afe2ca4e2b15182dd27f6e95fe92141a4`  
		Last Modified: Fri, 19 Feb 2021 22:06:45 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f80dcef5dda1a47d3599a0fb6640f3b33febd6d913a063450a90e38203ee7b`  
		Last Modified: Fri, 19 Feb 2021 22:06:45 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; mips64le

```console
$ docker pull nextcloud@sha256:d3e05269fb1506906a3804cee3934cdd893ff4d4dd91fa295fb495346e3f232b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.8 MB (257797325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e2cc27e3b7727e2695f1f5a9174cc890784b2f99158959742425aa202330ac9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:38:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 04:38:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 04:39:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:39:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 04:39:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 05:05:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 05:05:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 05:05:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 05:05:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 05:48:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 05:48:49 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 05:48:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 05:48:50 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 05:49:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 05:49:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:01:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 06:01:54 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:01:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 06:01:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 06:01:56 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 06:01:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 06:01:58 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 06:01:59 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 06:01:59 GMT
CMD ["php-fpm"]
# Tue, 09 Feb 2021 19:58:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 20:17:36 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:17:36 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:25:22 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:25:24 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:25:25 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:32:22 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:34:02 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:34:05 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:34:06 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:34:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:34:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:dfb81134097d874e01b495d1fba82e384056d0a3a45f01a69a2e86ae82af1e96`  
		Last Modified: Tue, 09 Feb 2021 03:15:55 GMT  
		Size: 25.8 MB (25764640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ea2980e9d1424f17765223b637d6e3f527c0ab3e3b3c293e4ab6d46df86bb6`  
		Last Modified: Tue, 09 Feb 2021 07:01:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fd49341687ab8ff8e018c1339c00f4b14d980dcff74a90982425c92fb4d468`  
		Last Modified: Tue, 09 Feb 2021 07:02:38 GMT  
		Size: 61.4 MB (61402881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385772c6452fb0c29341d9195703f25fc85945134be55c6dfe8b39f7825c9cf`  
		Last Modified: Tue, 09 Feb 2021 07:01:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fd37cb33d4d671be245456014ae832e083403fb8142c8038ff3b3a8a41d04`  
		Last Modified: Tue, 09 Feb 2021 07:07:41 GMT  
		Size: 10.7 MB (10650796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103b1f44f0959315aede9ae1329156e090f84952bce3fc17d79258ac2998487`  
		Last Modified: Tue, 09 Feb 2021 07:07:36 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4affa4d311f9eab19b574358573581c1575976bb4361ca8bf5b3c3977594cfb`  
		Last Modified: Tue, 09 Feb 2021 07:07:55 GMT  
		Size: 27.9 MB (27947294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46a481ed96aa7d0683f668a038c6d1e2050dc98bbf3700b8f446cc5a7d828ad`  
		Last Modified: Tue, 09 Feb 2021 07:07:35 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0100091b1ba6cfc7afb1c4a02b615092878038e09f1e0cb6cd284a20dcbc6e2`  
		Last Modified: Tue, 09 Feb 2021 07:07:35 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1560c9a0434bb7e3dc599e32c4b7bcb782452ada53bda164e02474215bc44ef8`  
		Last Modified: Tue, 09 Feb 2021 07:07:35 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3257a32e6c942e7031b1673ce826338fe3517dc386ab1614d8edcf55d02eca1`  
		Last Modified: Tue, 09 Feb 2021 20:18:22 GMT  
		Size: 1.7 MB (1740129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827aee4f453eb6086b6ec202e5c32a7a41b7dd4ad8f9d13e271c0ee841c222e`  
		Last Modified: Fri, 19 Feb 2021 20:45:07 GMT  
		Size: 14.9 MB (14936522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef56ae30c55a173d672a7c1da0bf662404463d90731616bc7ccca4259f41853`  
		Last Modified: Fri, 19 Feb 2021 20:44:55 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7c7136e16b2de182f0a1c5f674dae42d263ca76b203dc31729684de2b04409`  
		Last Modified: Fri, 19 Feb 2021 20:52:53 GMT  
		Size: 115.3 MB (115338183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f5d5b43ae6cac712f1e96290819f3ee5138b3eaea4b51c1dbae780a6e41552`  
		Last Modified: Fri, 19 Feb 2021 20:51:36 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c68a4f60b77ef468be2acbcb814d08c14c34d714fd36f58f973fbfa801217be`  
		Last Modified: Fri, 19 Feb 2021 20:51:37 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:266473363618940d0f2d1e5514f0ee1756e3036e44f2b3e612e439cba3ff7321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287665937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd51c009adcb30c63cbde095b889d3c250767a5d10c763c471807a2e520ff0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 15:49:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 15:49:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 15:54:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 15:54:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 15:54:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 16:18:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 16:19:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 16:19:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 16:19:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 16:51:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 16:51:28 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 16:51:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 16:51:40 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 16:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 16:53:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 16:58:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 16:58:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 16:59:02 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 16:59:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 16:59:16 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 16:59:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 16:59:41 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 16:59:48 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 16:59:54 GMT
CMD ["php-fpm"]
# Wed, 10 Feb 2021 12:08:49 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 21:31:11 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 21:31:15 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 21:49:45 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 21:49:51 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 21:49:57 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 22:11:55 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 22:15:37 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 22:15:47 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 22:15:56 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 22:16:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 22:16:09 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08ed6cfbd4e7b8f4f2d892c01b1976ced072938787d146fc0a55690e9883a74`  
		Last Modified: Tue, 09 Feb 2021 17:52:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cc4083d6613c902035d3b0dd1bb317f5bb699313bcd6e687ec17347192cdaa`  
		Last Modified: Tue, 09 Feb 2021 17:53:19 GMT  
		Size: 82.3 MB (82290490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d61a25f1b4f9da6f8c429b980f08dd7c19f7c6353704da136afc7e59343620`  
		Last Modified: Tue, 09 Feb 2021 17:52:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b19d6f07388b67c4e2b25252fe5e46f0aa30de01108238cb01ed728e0d94628`  
		Last Modified: Tue, 09 Feb 2021 17:57:49 GMT  
		Size: 10.7 MB (10653144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37f3ef96f3570acff03f70191ae67291b2f4b9f2ac3778e9b70e1b387a44758`  
		Last Modified: Tue, 09 Feb 2021 17:57:44 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e662f782a54a40cc879686ab700fffffe801c92eb503ce7401e7eb84404808d`  
		Last Modified: Tue, 09 Feb 2021 17:57:50 GMT  
		Size: 30.3 MB (30255502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231e87cfad0e6e0902e9779c69dca083d83cc8c5d3d1f536135207a3c6b431a`  
		Last Modified: Tue, 09 Feb 2021 17:57:44 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285634ae1567972454a4d16960daebbae9726b7145ae943603ec97270ec1c196`  
		Last Modified: Tue, 09 Feb 2021 17:57:44 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae14b5739094bd3f4b289ec08cf5ea1f53d71d64a8079cc6da751f43a8e4ef`  
		Last Modified: Tue, 09 Feb 2021 17:57:46 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a351e9e360276b4d8e14f3720b9b4a5b168e4b8d5aed00291f3e498b6a38e59`  
		Last Modified: Wed, 10 Feb 2021 13:04:17 GMT  
		Size: 1.8 MB (1803342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f682f5e3357d3dd2639617f812e17b803fd91a7bf664ca3767ab3acc613a44ae`  
		Last Modified: Fri, 19 Feb 2021 22:44:45 GMT  
		Size: 16.8 MB (16784548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0c775669e687bc8ce45470a45aa463518af0632f37b70dbae8bdea32e0624f`  
		Last Modified: Fri, 19 Feb 2021 22:44:29 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3454e428c2ca93fc9df3b17fe80e305bec130ac35f661d39d133055108d5bb61`  
		Last Modified: Fri, 19 Feb 2021 22:59:09 GMT  
		Size: 115.3 MB (115342430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab03a768e127241c55330a2d8602aa9fa0c1d0c8a3b176a0f21bb4428cda4a4`  
		Last Modified: Fri, 19 Feb 2021 22:57:28 GMT  
		Size: 2.5 KB (2530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48793a1c46cfc78ece8fd62e8ac343924e280aa5ce880ea58f4a2bebdfb61f6d`  
		Last Modified: Fri, 19 Feb 2021 22:57:28 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; s390x

```console
$ docker pull nextcloud@sha256:9b583a2dc505b5835d012e9fefb3617f649abb5d19ffb679243aa795789b88dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.7 MB (260716905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6027d0660e696c29c844d22d227b48126b5894153cd5074b3b9a645076f1b6b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:49:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 05:49:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 05:49:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:49:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 05:49:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 05:54:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Feb 2021 05:54:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 05:54:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 05:54:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 06:09:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 06:09:20 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 06:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 06:09:21 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 06:09:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 06:09:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:11:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 06:11:47 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:11:48 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 06:11:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 06:11:49 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 06:11:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Feb 2021 06:11:49 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Feb 2021 06:11:50 GMT
EXPOSE 9000
# Tue, 09 Feb 2021 06:11:50 GMT
CMD ["php-fpm"]
# Tue, 09 Feb 2021 13:06:51 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 19 Feb 2021 20:07:28 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:07:28 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:10:32 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:10:34 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:10:34 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:16:04 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:16:42 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 19 Feb 2021 20:16:51 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:16:52 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:16:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5de5518f7317a13d96a78cb6a69d8a40c528b4f9f5cb8ec38cc29d96e0d3a8`  
		Last Modified: Tue, 09 Feb 2021 06:28:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631238e5cca78ca96ac7a1e842104ab9c3ebc4b79becc0737d434640363dd04`  
		Last Modified: Tue, 09 Feb 2021 06:29:02 GMT  
		Size: 64.7 MB (64709263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8411cec4a9e17ed0143fe56c907dc88654d788140303c7f805c87d03077642f7`  
		Last Modified: Tue, 09 Feb 2021 06:28:52 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598635b184b7dbfc3b0bcfa69512b8d371cdc177de8116323a82910be4055551`  
		Last Modified: Tue, 09 Feb 2021 06:31:31 GMT  
		Size: 10.7 MB (10651616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327c7c58cf2897fb1ee93fb866843887bf119c7544495b4318ed08e0078964d5`  
		Last Modified: Tue, 09 Feb 2021 06:31:29 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf39d2989616d1fc8f7cdecc0e9605285b0fd335397a5dee0d8d9245b485ca02`  
		Last Modified: Tue, 09 Feb 2021 06:31:33 GMT  
		Size: 27.7 MB (27682067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815acac977eebca8a596d480d696b0996c24e4e1bc779f79981200945389133b`  
		Last Modified: Tue, 09 Feb 2021 06:31:29 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2415d4c409d86b54c0fb0330c350cdfa1bad941614d439eac10860f54d4f420`  
		Last Modified: Tue, 09 Feb 2021 06:31:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab35dbf7adcf4e89d5cdea6acf95054252c66ed2b0812559cc3051b15aef75c6`  
		Last Modified: Tue, 09 Feb 2021 06:31:29 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d57666a4cb4e96eead2e7b7091c2a04af730a070f7226ee65812bbbd8ecca97`  
		Last Modified: Tue, 09 Feb 2021 13:15:29 GMT  
		Size: 1.6 MB (1595054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeda321cfed821bb56014cc227a90b3fedda5852020a08c4f8774f6bc40dc1c`  
		Last Modified: Fri, 19 Feb 2021 20:27:55 GMT  
		Size: 15.0 MB (15013511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84f419f3b9463db3b2eda4c17da410ba78b38a8d5ef48d834b397cad98a44fa`  
		Last Modified: Fri, 19 Feb 2021 20:27:53 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d7652095496adbf9c15712ae4c0c4b0d437c3909e34a11807d676bd5ce1d1b`  
		Last Modified: Fri, 19 Feb 2021 20:30:49 GMT  
		Size: 115.3 MB (115338414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f552b17ba35a36ce0533ec40e85ed85aefc36150b13eeb829429c0ae2a9435a9`  
		Last Modified: Fri, 19 Feb 2021 20:30:35 GMT  
		Size: 2.5 KB (2530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dea425f299f3c2aed5e6fbc27cec37853506fbd9293aa8894bdeb3fe3c9296`  
		Last Modified: Fri, 19 Feb 2021 20:30:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
