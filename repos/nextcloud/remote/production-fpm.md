## `nextcloud:production-fpm`

```console
$ docker pull nextcloud@sha256:f3332ba3b76c41008568cf5b415e32d7e692a4ece8bf41263bb135af272ba65c
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

### `nextcloud:production-fpm` - linux; amd64

```console
$ docker pull nextcloud@sha256:7139fed70ad35e8f6411b07b21e2d7a3a680d57241728f81500f2ead25db400e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333101944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058be39bcc32b7cc210fd7f6bb70b1a9820b4a295d8234129ded3ddec63dd905`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:36:02 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 28 May 2022 09:01:19 GMT
ENV PHP_VERSION=8.0.19
# Sat, 28 May 2022 09:01:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sat, 28 May 2022 09:01:20 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sat, 28 May 2022 09:01:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 09:01:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 09:10:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 09:10:57 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 09:10:57 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 09:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 09:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 09:10:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 09:10:58 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 09:10:58 GMT
EXPOSE 9000
# Sat, 28 May 2022 09:10:58 GMT
CMD ["php-fpm"]
# Sun, 29 May 2022 03:58:17 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 29 May 2022 03:58:17 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 29 May 2022 03:58:17 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 29 May 2022 04:00:54 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 04:00:55 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 29 May 2022 04:00:55 GMT
VOLUME [/var/www/html]
# Sun, 29 May 2022 04:02:50 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Sun, 29 May 2022 04:03:37 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 04:03:39 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Sun, 29 May 2022 04:03:40 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Sun, 29 May 2022 04:03:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 04:03:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f57c6eca5ef34577f78fe7a047baefdc8c594d6d7482812899c0b938238361`  
		Last Modified: Sat, 28 May 2022 09:57:06 GMT  
		Size: 11.1 MB (11097109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772187e935420c567585f864de113d6a820f8c7abee09244ec5c9c8c3aebdea7`  
		Last Modified: Sat, 28 May 2022 09:57:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb7393cbd51a6d8ce7b9e1dce8c2ed9bad7f5ed236acdf5362803895becd199`  
		Last Modified: Sat, 28 May 2022 09:58:00 GMT  
		Size: 26.0 MB (25966171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c25fbb32b16a0d183e90643da22977ef09ef632200a905a7c28fecfbad37805`  
		Last Modified: Sat, 28 May 2022 09:57:53 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43075683ff38fab3eb2d6da22251ce9d15fcba14d43f3a7733c0f8774e816b26`  
		Last Modified: Sat, 28 May 2022 09:57:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c9ebc89d65d71145f226f39fab56472818cbc65417c25455be9ae170ca0d53`  
		Last Modified: Sat, 28 May 2022 09:57:53 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8db282cd229655989e07377b19d3eb4b7351ea01ef69a78b20182fee1bc3b41`  
		Last Modified: Sun, 29 May 2022 04:06:57 GMT  
		Size: 1.7 MB (1675791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa63b26231300034cf31e42f8d7f7794349d64d60bcea3cc1d98b14eeedac5b6`  
		Last Modified: Sun, 29 May 2022 04:06:57 GMT  
		Size: 17.6 MB (17605380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cd86ce4267c0e5e493ba88ee9e2c0818b105029eaa3925e2efda2c04b43682`  
		Last Modified: Sun, 29 May 2022 04:06:54 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5ddd8c96b4ce3e7febcfe809b0556d7c388e5f7e334b93a0344dd80ed41169`  
		Last Modified: Sun, 29 May 2022 04:08:48 GMT  
		Size: 153.8 MB (153756493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588d36574986167c340765f5fc9cf968ed7ed105bef8b442a3d04493f1d7d6a3`  
		Last Modified: Sun, 29 May 2022 04:08:28 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b384f149fb68c1d01adda262e9f3d5b077b88be057962020ac4fddc64f870001`  
		Last Modified: Sun, 29 May 2022 04:08:27 GMT  
		Size: 2.1 KB (2138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:bfb1c1bc5193d59238ced44956f50cfd6ce1cf367f653255bd6d4e00e4b1f7c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.0 MB (309035742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:980a67aa499a9862621f00585b6d3709dee5c13c5c2091e053dac040efb9d764`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 20:41:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 20:41:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 20:42:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:42:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 20:42:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 20:42:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 20:42:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 20:42:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 21:29:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 00:39:21 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 00:39:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 00:39:21 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 00:39:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 00:39:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:55:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 00:55:32 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:55:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 00:55:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 00:55:35 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 00:55:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 10 Jun 2022 00:55:38 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Jun 2022 00:55:38 GMT
EXPOSE 9000
# Fri, 10 Jun 2022 00:55:39 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 04:29:07 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 10 Jun 2022 04:29:07 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 10 Jun 2022 04:29:08 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 10 Jun 2022 04:36:10 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 04:36:11 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 10 Jun 2022 04:36:12 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 04:40:14 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Fri, 10 Jun 2022 04:41:54 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 04:41:58 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Fri, 10 Jun 2022 04:41:59 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Fri, 10 Jun 2022 04:42:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 04:42:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cf3513616b2ea05dba65517d17dda27a1ceee04ba9287047dd04f6979c06f9`  
		Last Modified: Sat, 28 May 2022 23:50:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443372867141fb1f3fe996587efd00d75c4718138718a4515907898d5c1ad900`  
		Last Modified: Sat, 28 May 2022 23:51:14 GMT  
		Size: 73.7 MB (73685298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728498cc6c6df3b79ec87ce8985063790e5399f12d368c50f635e46a6816ba2e`  
		Last Modified: Sat, 28 May 2022 23:50:24 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310a805b83c9faa2d925e146470cbb598cddf8d7223267fdce9e3388a997e5ce`  
		Last Modified: Fri, 10 Jun 2022 01:38:44 GMT  
		Size: 11.2 MB (11196104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bf4c551596174e572406a9bc48bbd92628a8c5f426270bc6723b36572cb45`  
		Last Modified: Fri, 10 Jun 2022 01:38:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545d4e2fd73f21e027a219a9b3a4bda00e872f51ec1f415e236ccc8347335c8`  
		Last Modified: Fri, 10 Jun 2022 01:40:21 GMT  
		Size: 24.5 MB (24548189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e53e330c0a7ee3aa8b0c81d26b164db15e0e7d3b59b25bed54590dd1df3e2`  
		Last Modified: Fri, 10 Jun 2022 01:40:05 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe7130ecfbaeddf7c317bfb6b01d44b312e5596af78a851d82ef527d9875cff`  
		Last Modified: Fri, 10 Jun 2022 01:40:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb921f2ffe8ad495678b703ea05610e09829ed7101e360566587d7abf857615b`  
		Last Modified: Fri, 10 Jun 2022 01:40:05 GMT  
		Size: 8.6 KB (8575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c353c901c0a75c97ff373a9846b4204e9ac8b0b8599b309a0b810f9f9d5840c1`  
		Last Modified: Fri, 10 Jun 2022 04:50:43 GMT  
		Size: 1.6 MB (1630863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dfe2b2948a83c9176de6d7d264c37c184e030d61238cc8a06fba2a738da994`  
		Last Modified: Fri, 10 Jun 2022 04:50:49 GMT  
		Size: 15.3 MB (15280494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14242764b2b7dd4206b5299bbe6e1e86c9f0b2acf0a46f569197f5a4973d2ae7`  
		Last Modified: Fri, 10 Jun 2022 04:50:40 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc197a21b328414c57cd2fd168515d75f0e1a907e24d55707a8c9e7ac6665db6`  
		Last Modified: Fri, 10 Jun 2022 04:56:50 GMT  
		Size: 153.8 MB (153755360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30a71a46f7767dff3c9d90a17f7b8f35b433b0b0b5a748bcbc76031157f836a`  
		Last Modified: Fri, 10 Jun 2022 04:55:06 GMT  
		Size: 3.0 KB (2962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715361b7679af654c112973d8deab243a721374763dbd7aa43d7252682eecafa`  
		Last Modified: Fri, 10 Jun 2022 04:55:07 GMT  
		Size: 2.1 KB (2137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:9e8797deb2724ec54ccdef4d2d28916b41147101bff71f6a743c6eb30d0728f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300136311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f39b7f5bd127ebec169bc448b808e1f0f8bbe56a2d763c14a429e2599a55dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 07:20:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 29 May 2022 07:20:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 29 May 2022 07:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 07:21:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 29 May 2022 07:21:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 29 May 2022 07:21:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:21:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:21:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sun, 29 May 2022 08:07:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sun, 29 May 2022 08:49:48 GMT
ENV PHP_VERSION=8.0.19
# Sun, 29 May 2022 08:49:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sun, 29 May 2022 08:49:49 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sun, 29 May 2022 08:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 29 May 2022 08:50:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 29 May 2022 09:05:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sun, 29 May 2022 09:05:05 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sun, 29 May 2022 09:05:08 GMT
RUN docker-php-ext-enable sodium
# Sun, 29 May 2022 09:05:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 29 May 2022 09:05:10 GMT
WORKDIR /var/www/html
# Sun, 29 May 2022 09:05:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sun, 29 May 2022 09:05:14 GMT
STOPSIGNAL SIGQUIT
# Sun, 29 May 2022 09:05:15 GMT
EXPOSE 9000
# Sun, 29 May 2022 09:05:15 GMT
CMD ["php-fpm"]
# Mon, 30 May 2022 05:22:48 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Mon, 30 May 2022 05:22:49 GMT
ENV PHP_MEMORY_LIMIT=512M
# Mon, 30 May 2022 05:22:49 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Mon, 30 May 2022 05:29:48 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 05:29:49 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Mon, 30 May 2022 05:29:50 GMT
VOLUME [/var/www/html]
# Mon, 30 May 2022 05:34:01 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Mon, 30 May 2022 05:35:37 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 05:35:39 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Mon, 30 May 2022 05:35:41 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Mon, 30 May 2022 05:35:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 30 May 2022 05:35:42 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d3aba112689c02d6b26a241e0065c97e4d937ec22a83ec2611313d531e8b0a`  
		Last Modified: Sun, 29 May 2022 10:31:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c1acd8b719bd38a8741d6d093c916a6a558e402efb4f9e8a9c0d8331959d0d`  
		Last Modified: Sun, 29 May 2022 10:31:44 GMT  
		Size: 69.3 MB (69318858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669dd875526c016d77dc484bfa38a4f856de0994a919ad17c67ba551ea39613a`  
		Last Modified: Sun, 29 May 2022 10:31:01 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06850456551836064ad3f0463403f6af03d787ec0d8f37e815270a927113493`  
		Last Modified: Sun, 29 May 2022 10:44:13 GMT  
		Size: 11.1 MB (11095691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa58ee0da4f1031588d6d1422d8b9b606ece7a8336f2715b577436a9b6cad46`  
		Last Modified: Sun, 29 May 2022 10:44:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f9720ff394548883a5b5e43f20acc32a3cc0b087ea80de0a5923c5a77100b9`  
		Last Modified: Sun, 29 May 2022 10:45:44 GMT  
		Size: 23.8 MB (23754475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee999243ce86163ca1eac8e542485abc43effb8892bae6c4b32f7390b0f9f66`  
		Last Modified: Sun, 29 May 2022 10:45:29 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2714974985c6703f44df36ef800a862194965d0c8e72e309a4db4e3d711ab968`  
		Last Modified: Sun, 29 May 2022 10:45:29 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d8f1d79314823ec091c4a6b2717ea90ec35603bda63d8e743342bef11fadf9`  
		Last Modified: Sun, 29 May 2022 10:45:29 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cf7b1ba41fbbef1929a9954183a8bfa1e2cf89b316f1936bc1599ed06f9865`  
		Last Modified: Mon, 30 May 2022 05:45:33 GMT  
		Size: 1.5 MB (1484967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3ae45b7a99a818482045cbfaace6d42670af86165f42192d16160397d8da1a`  
		Last Modified: Mon, 30 May 2022 05:45:38 GMT  
		Size: 14.1 MB (14132526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab9d0f78ec6f68adbdaca1d6b202c539274827f029e065a0dbef92e9e952274`  
		Last Modified: Mon, 30 May 2022 05:45:30 GMT  
		Size: 599.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480e78ee4251f4e88721bae20f0269c195f85457bc764153ca5fb8ee41b882d7`  
		Last Modified: Mon, 30 May 2022 05:51:46 GMT  
		Size: 153.8 MB (153755601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2b5123995bc8944495f1a714332b6b1c72dc7b23dfa625e13420e8d08e6814`  
		Last Modified: Mon, 30 May 2022 05:50:02 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ebdb358098479cfa73481f3aef01cc38f78f25ebcea8b40aff76fa61fccfc7`  
		Last Modified: Mon, 30 May 2022 05:50:02 GMT  
		Size: 2.1 KB (2137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:9dc1e61fbe1da0819276c91a58a8547373ac294ebcc0fc4e2cf23275dcbd4460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.0 MB (322967435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec279bf88a39e2a489183dd2e08334bf290b292c1c3a741aa369f86ef831f157`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:40:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 04:40:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 04:40:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 04:40:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 04:40:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 04:40:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 04:40:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 04:40:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 05:15:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 28 May 2022 05:38:55 GMT
ENV PHP_VERSION=8.0.19
# Sat, 28 May 2022 05:38:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sat, 28 May 2022 05:38:57 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sat, 28 May 2022 05:39:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 05:39:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 05:47:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 05:47:36 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 05:47:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 05:47:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 05:47:38 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 05:47:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 05:47:40 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 05:47:41 GMT
EXPOSE 9000
# Sat, 28 May 2022 05:47:42 GMT
CMD ["php-fpm"]
# Sat, 28 May 2022 23:17:28 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 28 May 2022 23:17:28 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 28 May 2022 23:17:29 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 28 May 2022 23:21:36 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 23:21:37 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 28 May 2022 23:21:37 GMT
VOLUME [/var/www/html]
# Wed, 01 Jun 2022 04:32:17 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Wed, 01 Jun 2022 04:33:00 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 04:33:02 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Wed, 01 Jun 2022 04:33:03 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Wed, 01 Jun 2022 04:33:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Jun 2022 04:33:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57f60612e180c578a7a4978e5e3ec509e89e091d56490e890ab31c0413f7907`  
		Last Modified: Sat, 28 May 2022 06:31:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1687b455bba4be0b923345f633dd5dedf683b31e562d99c279245ae0386f68b2`  
		Last Modified: Sat, 28 May 2022 06:31:20 GMT  
		Size: 86.7 MB (86719287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450e89c3c60d5fa89af649f1d70e79286f0f1f1f77330c59c5d151d2f3a0494`  
		Last Modified: Sat, 28 May 2022 06:31:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1ac3b06c4d7f6a36362ba3fa7d61ef3fe9289ca82d0f9b8ad48b96a93fdb38`  
		Last Modified: Sat, 28 May 2022 06:39:27 GMT  
		Size: 10.9 MB (10880425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cef2fd17fc1bc1ab8c42ffac1dd214776ed836d83c5ee55ef836af99abfcf0`  
		Last Modified: Sat, 28 May 2022 06:39:26 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e223535f3fcff00db7a634909dcfde6e0808528bb6a3f1d062ba8659879e4`  
		Last Modified: Sat, 28 May 2022 06:40:27 GMT  
		Size: 25.2 MB (25177468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f044cb12cfcab6e1bea15a8836f32ca00297b3376b543ba6e2834eeda1a2f30b`  
		Last Modified: Sat, 28 May 2022 06:40:23 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05468e3c6fe36d39362201754a838092c8f3f0a097a7898b1ea6d5176df3be4c`  
		Last Modified: Sat, 28 May 2022 06:40:23 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e6a2dbc56be7a9211e79931272e645805b4ec05f0ea6cdc24b22b7ef5f1bb2`  
		Last Modified: Sat, 28 May 2022 06:40:23 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee4e1772f68e19118e2f8ddae896d51cc9b98fddcf85515bdd74c0f4d009f9`  
		Last Modified: Sat, 28 May 2022 23:23:23 GMT  
		Size: 1.4 MB (1406262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da106a34d4aada9a109050c6995045a9ffc185c6cb7ef8fafec14d231949b5d`  
		Last Modified: Sat, 28 May 2022 23:23:22 GMT  
		Size: 15.2 MB (15186590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad9d7268891357a386ab3d45f341f45e96ea380e97832878ca4da2bba0c4d74`  
		Last Modified: Sat, 28 May 2022 23:23:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7e0c2f11ae115c23b3f8ec2028a45b1f03c2dc8f5f3175c853dc7725c5db41`  
		Last Modified: Wed, 01 Jun 2022 04:35:36 GMT  
		Size: 153.5 MB (153513801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82a619288ec5bc705bdce40047d4c0ac9d939f4cadf61aeda49434d33f8e89`  
		Last Modified: Wed, 01 Jun 2022 04:35:15 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868542aaaea66f4eb8222c2be15d44ceb2359670e1ff1a7f2b6149dc88c8a20a`  
		Last Modified: Wed, 01 Jun 2022 04:35:15 GMT  
		Size: 2.1 KB (2138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; 386

```console
$ docker pull nextcloud@sha256:b1df4ff877d11a80873c330370bd2b4b7cc433d140bde3f2aa9aead74d077558
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334003578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cadcf01e02a54ef16be24b4ea234f8360dc5d9693d1c9ff4a402fe38214e46cc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:54:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 12:54:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 12:54:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:54:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 12:54:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 12:54:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 12:54:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 12:54:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 13:21:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 00:34:10 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 00:34:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 00:34:12 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 00:34:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 00:34:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:43:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 00:43:11 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:43:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 00:43:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 00:43:13 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 00:43:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 10 Jun 2022 00:43:15 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Jun 2022 00:43:16 GMT
EXPOSE 9000
# Fri, 10 Jun 2022 00:43:17 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 03:04:51 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 10 Jun 2022 03:04:51 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 10 Jun 2022 03:04:52 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 10 Jun 2022 03:07:15 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 03:07:16 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 10 Jun 2022 03:07:17 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 03:13:15 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Fri, 10 Jun 2022 03:14:06 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 03:14:07 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Fri, 10 Jun 2022 03:14:09 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Fri, 10 Jun 2022 03:14:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 03:14:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c02a78549ec8030de8b3a962c06643d7d8ed9a217cca23d33fec7c51be6b9d`  
		Last Modified: Sat, 28 May 2022 14:39:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491b4ce327992f77619335bcb7ceb213894da2ffaf99044a3546f17bbdb5ed82`  
		Last Modified: Sat, 28 May 2022 14:39:23 GMT  
		Size: 92.5 MB (92512638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85e0a52eb6f63802a15b9900b474ab734e50c976ecef2881f270d3cec6fa5c7`  
		Last Modified: Sat, 28 May 2022 14:39:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaea98b1a001b7dcfef89a5a3d672bf5aa516328be2b76f6758c0fcaff1dec3`  
		Last Modified: Fri, 10 Jun 2022 01:33:58 GMT  
		Size: 11.0 MB (10981261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756e174644754f0fa1d33a84109a43f54098acd642c3b3d3593b5b23ec4fd740`  
		Last Modified: Fri, 10 Jun 2022 01:33:56 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c958291aff45d56048ace59649c06adfb2e2a547b03f0dd8989b1b457ca9bf`  
		Last Modified: Fri, 10 Jun 2022 01:34:57 GMT  
		Size: 26.2 MB (26201682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331b478aabd530bd5f7391d3508a787686bee4cfb3eaa63ebad33419c27b856`  
		Last Modified: Fri, 10 Jun 2022 01:34:53 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9db6c73ec7ca4eaa94646dfc27c1252b0276f25ac91ea3e454ba375e47ddc0a`  
		Last Modified: Fri, 10 Jun 2022 01:34:54 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e5ca96dc9a838f380f45819f1f8215a127d40482fd5a19bb9dbfdad8fecc5`  
		Last Modified: Fri, 10 Jun 2022 01:34:53 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ab93584bf70a3545c0a91c05a6292951ce9066afb27a5ce218259ff5e668c6`  
		Last Modified: Fri, 10 Jun 2022 03:21:08 GMT  
		Size: 1.5 MB (1490471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310b30f4627e64a55db75bb3bd5cbcf28f9dd0be3af9bb6b0164a944b54c42e0`  
		Last Modified: Fri, 10 Jun 2022 03:21:08 GMT  
		Size: 16.9 MB (16895642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da78d9febe2c5a5cddc69c5aa7b8b7beb78d86cdc93659b94cbaad1d5cf245e`  
		Last Modified: Fri, 10 Jun 2022 03:21:10 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af69081969b2f72bc8074a359cb3dbaceba202d8a38cbd7cfdf5a759efe947f`  
		Last Modified: Fri, 10 Jun 2022 03:24:09 GMT  
		Size: 153.5 MB (153513684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b5c7ca01f9d545faa52db82bc2da9955801a00d75809aa77e794defb2857f0`  
		Last Modified: Fri, 10 Jun 2022 03:23:58 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93db00d936cb9345195f9699e3e1ff4ea2b85113b21b3a07736e44108163739a`  
		Last Modified: Fri, 10 Jun 2022 03:23:47 GMT  
		Size: 2.1 KB (2140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; mips64le

```console
$ docker pull nextcloud@sha256:bddc32e0dfecef2776b45e1d56881ca1e14b284531b0e81c2bec96816247d856
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.5 MB (307503281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7869a6ebc522c884258d9a245572f8f8985042998ea5d173c5137b2182549c21`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:30:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 03:30:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:32:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 03:32:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 03:32:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 03:32:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 03:32:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 05:30:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 28 May 2022 07:22:48 GMT
ENV PHP_VERSION=8.0.19
# Sat, 28 May 2022 07:22:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sat, 28 May 2022 07:22:55 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sat, 28 May 2022 07:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 07:23:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 08:05:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 08:05:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 08:05:10 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 08:05:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 08:05:18 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 08:05:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 08:05:28 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 08:05:32 GMT
EXPOSE 9000
# Sat, 28 May 2022 08:05:35 GMT
CMD ["php-fpm"]
# Mon, 30 May 2022 07:40:18 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Mon, 30 May 2022 07:40:21 GMT
ENV PHP_MEMORY_LIMIT=512M
# Mon, 30 May 2022 07:40:25 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Mon, 30 May 2022 07:52:11 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 07:52:18 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Mon, 30 May 2022 07:52:22 GMT
VOLUME [/var/www/html]
# Mon, 30 May 2022 07:59:23 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Mon, 30 May 2022 08:02:06 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 08:02:16 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Mon, 30 May 2022 08:02:24 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Mon, 30 May 2022 08:02:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 30 May 2022 08:02:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48ffa812cba4145b49cbbc61824a577807dfbea2e248d5216b5b1fa5d6d81b5`  
		Last Modified: Sat, 28 May 2022 10:42:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ee5523dfa904c61988aab187090bf4bdb8ce8a4c4b8fa903a0ae6bc67d00cc`  
		Last Modified: Sat, 28 May 2022 10:43:14 GMT  
		Size: 71.8 MB (71812105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85368acf1e84d74f279250b786757fc0fad630ccedb2cf42c99422aee2bd1097`  
		Last Modified: Sat, 28 May 2022 10:42:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cda0a43dc193c7343b40fb44af544b5a2351acc52941a7fceeba85f4fbe1dd`  
		Last Modified: Sat, 28 May 2022 10:53:06 GMT  
		Size: 10.9 MB (10879247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb8278845d6261691d8bcbb2b0f6fec98a501369a1cc194ab3f71c352756371`  
		Last Modified: Sat, 28 May 2022 10:53:04 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d0f9ef0f6b0dfac2a2705917f32bdbcebbcd52b506315ac3e35928f1696691`  
		Last Modified: Sat, 28 May 2022 10:54:39 GMT  
		Size: 25.0 MB (24959544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840cc8157da523f9131b544534c3d98bb46403b43db36e19124a2b75a03759e3`  
		Last Modified: Sat, 28 May 2022 10:54:23 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126bc911d5198a24ba4c5c28b478a3f40c9737099264268ec69e8b7fb8927d6f`  
		Last Modified: Sat, 28 May 2022 10:54:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cd4ca9c0e472e052eff85d671e9ecb2652581ab710092c93e0ba17e1d827b0`  
		Last Modified: Sat, 28 May 2022 10:54:23 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0901d89b5da6e316ad4ac6f7a9ef14fcc22f4f13d68dad770cea081743a07d`  
		Last Modified: Mon, 30 May 2022 08:11:58 GMT  
		Size: 1.5 MB (1542577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e82ef9120b1d6f0fc2097c9afc72a28f84022c8b233e8bdca23eb4cc6c001`  
		Last Modified: Mon, 30 May 2022 08:12:06 GMT  
		Size: 15.1 MB (15136165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f553fe5fe72afdad0481374c24092feeaed46c0424f98cd0812c64e912cd169`  
		Last Modified: Mon, 30 May 2022 08:11:54 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97173e4e3693a48e30e01424379af2cf677769afe83df35079e7b63c6933c000`  
		Last Modified: Mon, 30 May 2022 08:17:40 GMT  
		Size: 153.5 MB (153514529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa041c116d7ead5158eae5c35f3cb248fad8292c728c19ce1c4ada53a5dd34`  
		Last Modified: Mon, 30 May 2022 08:16:02 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61375afbaa3121e0cafd1731a8e50edb279ed146546ecbd67ec3ae0c7bc9393`  
		Last Modified: Mon, 30 May 2022 08:16:02 GMT  
		Size: 2.1 KB (2138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:98269c803e265dc88730bd1432f998f0fb54b5814a5f092eb77fe5b2ef32f404
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332720751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:998ae28bed04bc5766d13eb242c547bea1a4c96b97f416305fe9e84325a1f44f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:22:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 07:22:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 07:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:24:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 07:24:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 07:24:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 07:24:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 07:24:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:26:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 28 May 2022 09:15:36 GMT
ENV PHP_VERSION=8.0.19
# Sat, 28 May 2022 09:15:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sat, 28 May 2022 09:15:43 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sat, 28 May 2022 09:16:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 09:16:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 09:33:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 09:33:11 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 09:33:19 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 09:33:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 09:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 09:33:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 09:33:34 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 09:33:37 GMT
EXPOSE 9000
# Sat, 28 May 2022 09:33:39 GMT
CMD ["php-fpm"]
# Sun, 29 May 2022 15:10:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 29 May 2022 15:10:31 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 29 May 2022 15:10:34 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 29 May 2022 15:18:28 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 15:18:34 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 29 May 2022 15:18:35 GMT
VOLUME [/var/www/html]
# Sun, 29 May 2022 15:23:11 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Sun, 29 May 2022 15:25:09 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 15:25:17 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Sun, 29 May 2022 15:25:20 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Sun, 29 May 2022 15:25:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 15:25:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d642c3f5450a6405bbf9bc2437851b0fead8c5637c2187c3d0138aa4c80ebf`  
		Last Modified: Sat, 28 May 2022 10:59:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dd41b6c195f84ab156bcf8fb6794ba7e3f25a1e949fc8dc500f0fd4caa4d3c`  
		Last Modified: Sat, 28 May 2022 10:59:18 GMT  
		Size: 86.6 MB (86628797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79723c6985ec0cb8d1a54a87d5714b293a1e9dbe5567d6d4997e28bdc5912ae`  
		Last Modified: Sat, 28 May 2022 10:59:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6213cbd7d95e75240b54d3d51213ff3777e21f8e1a46182babd45408fff74afb`  
		Last Modified: Sat, 28 May 2022 11:08:47 GMT  
		Size: 11.1 MB (11097365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3dcf275c37d6fe12debd65367474354c67b34fe792e33c5beec1b537a083c2`  
		Last Modified: Sat, 28 May 2022 11:08:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1efdff96e2f39b13333c83c51f66d50e6393dffb5f16b6b715570816400575`  
		Last Modified: Sat, 28 May 2022 11:09:57 GMT  
		Size: 27.0 MB (26957077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01258546db948bc3ba4649996f22fc9f652e7f638ffc3e54cf4f2bf949c3d01e`  
		Last Modified: Sat, 28 May 2022 11:09:52 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb577e3ab52a856129975e1fc9d36e9063279f036bb4d53b3a6e18fe09685b69`  
		Last Modified: Sat, 28 May 2022 11:09:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b90e580340cd82367fd257fb1a8b4621c5cb15dd91e942f4c98da1b510a8043`  
		Last Modified: Sat, 28 May 2022 11:09:52 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83daf13833de9682d1cdf9840f780aa64cec3b7a1e212d658711a49f93d7fb`  
		Last Modified: Sun, 29 May 2022 15:34:40 GMT  
		Size: 1.8 MB (1844999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95524574af405a7310142474187a0bd48546fc7a8246a75ec018e9b765b2795b`  
		Last Modified: Sun, 29 May 2022 15:34:48 GMT  
		Size: 17.1 MB (17129484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0d1b4806ee50ae61ffe19b06620e8246cc8948f0d4648897a3ad76364600a`  
		Last Modified: Sun, 29 May 2022 15:34:36 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084f1c78377d490f4fff471d545443eb0043667e631c9a8361278b0f42462ae8`  
		Last Modified: Sun, 29 May 2022 15:42:20 GMT  
		Size: 153.8 MB (153758368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3880c2e8c2c280c0e8d4d9c596006837ea8f7bc5aca24e17277c0b817568e5`  
		Last Modified: Sun, 29 May 2022 15:40:14 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7a918c4c2022715c27a59006758927cd234029c8b5f902e3a48dac47997854`  
		Last Modified: Sun, 29 May 2022 15:40:14 GMT  
		Size: 2.1 KB (2141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm` - linux; s390x

```console
$ docker pull nextcloud@sha256:6989b6d4e41f37b32d2a5703e51693c771a747e23c8f8b9d81d61cd8b4485f0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308095481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe4ee64d14480e93629b3910b56cbd683731c5aefd7ad86a02f9159f6e9bcd9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:95dc6dcd4ebd15b42beaf935d91adafb0ea44a443bb44597bc1ff236e831ce18 in / 
# Sat, 28 May 2022 00:43:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 16:09:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 16:10:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 16:10:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:10:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 16:10:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 16:10:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 16:10:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 16:10:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 16:54:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 01:00:48 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 01:00:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 01:00:49 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 01:01:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 01:01:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:15:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 01:15:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:15:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 01:15:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 01:15:14 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:15:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 10 Jun 2022 01:15:15 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Jun 2022 01:15:15 GMT
EXPOSE 9000
# Fri, 10 Jun 2022 01:15:15 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 04:44:30 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 10 Jun 2022 04:44:31 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 10 Jun 2022 04:44:31 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 10 Jun 2022 04:48:52 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 04:48:56 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 10 Jun 2022 04:48:57 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 04:58:12 GMT
ENV NEXTCLOUD_VERSION=23.0.5
# Fri, 10 Jun 2022 04:59:12 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 04:59:33 GMT
COPY multi:497b8d243f90fa6abd88194ba134de5703abecf47c13a92d2f2fb8210d2cfa77 in / 
# Fri, 10 Jun 2022 04:59:34 GMT
COPY multi:7281097c8fd959eff64684726d7707d598f15dc22353d1f6f843624f642bdcd2 in /usr/src/nextcloud/config/ 
# Fri, 10 Jun 2022 04:59:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 04:59:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f7bb6d2d11c3060ba2e66ba762e2aa10a0d1d361cfa6a806bcf26a64cc3a79aa`  
		Last Modified: Sat, 28 May 2022 00:49:46 GMT  
		Size: 29.7 MB (29655258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47e439a4381bc90946be2559c7afda81b0167e9737ff78feb342c01b2f71137`  
		Last Modified: Sat, 28 May 2022 19:04:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e731871658790a1839d3b135f76c62d3c42dcfe04bcd88e657460235dfdd56`  
		Last Modified: Sat, 28 May 2022 19:04:56 GMT  
		Size: 71.6 MB (71623152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4d70c4df3a2e37ece08f89d98c9e3864f9e96559baa39c6eca54cf9b6d109c`  
		Last Modified: Sat, 28 May 2022 19:04:47 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf385d633a76ded6251d9aa52d2a35109b4c8a6f97ea7a8efd2d976064c03089`  
		Last Modified: Fri, 10 Jun 2022 02:11:52 GMT  
		Size: 11.2 MB (11196483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4230eff98cb65e243f6c481c6694e4f5ce87f909e5df0684344dcfad11bbf0`  
		Last Modified: Fri, 10 Jun 2022 02:11:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1f00b000f9538893db58703e00739408b5f78022dcd8d875ad3dc06ab1cb84`  
		Last Modified: Fri, 10 Jun 2022 02:12:30 GMT  
		Size: 25.0 MB (25041298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293cb0cf5e517254d3a455857cf1b1b50aee02a6376c4c9c27a931b1ecd3ae34`  
		Last Modified: Fri, 10 Jun 2022 02:12:27 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1964304f77f0328354689051d8a328139385b4be729f2a7079e4dd2276890cd`  
		Last Modified: Fri, 10 Jun 2022 02:12:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f071324fe563ece3b696851d0872f9592f82a03bf0be520ca4d979cd8eb2d074`  
		Last Modified: Fri, 10 Jun 2022 02:12:27 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bc565edd4cbe25c6f6c4f01f7480404bf3f0019d028b1079e6b7f13c9c8266`  
		Last Modified: Fri, 10 Jun 2022 05:06:59 GMT  
		Size: 1.6 MB (1633808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad15fbde2fa4d51a8a067aa9140896bc01e32357fe4b833886caa3aa2f43885`  
		Last Modified: Fri, 10 Jun 2022 05:06:59 GMT  
		Size: 15.2 MB (15171540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8e15d0d8f206e7f7e1c1a402832177dbc0eda0a53ce87662d2660987bba039`  
		Last Modified: Fri, 10 Jun 2022 05:06:57 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb473928738e6598c92c9cd2849915053832286802680caf4aaa5e3205101e1e`  
		Last Modified: Fri, 10 Jun 2022 05:08:53 GMT  
		Size: 153.8 MB (153755978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cd2cdb6d49938467f2db4dbab371f9100a32b267032ddcc6227952cbd7cf1b`  
		Last Modified: Fri, 10 Jun 2022 05:08:35 GMT  
		Size: 3.0 KB (2964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f162728ab6b6e1839b24a686e1c5c89c3d001bb680600fb45082355238e6896d`  
		Last Modified: Fri, 10 Jun 2022 05:08:35 GMT  
		Size: 2.1 KB (2140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
