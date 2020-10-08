## `nextcloud:20-fpm`

```console
$ docker pull nextcloud@sha256:be471725d3f888cd162ae4dfbcea85ac8ee37f2119528b10eec19900b72062b5
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

### `nextcloud:20-fpm` - linux; amd64

```console
$ docker pull nextcloud@sha256:f3d0b543a190d974a884403e4a1920348b0f36c3dcf2b4ac03f0eac4cd768e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291385789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffdfe565474bcfb7004d0f3999a0e9d8ab2df07d3f150c7e93f29918f49ec1ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 13:07:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 13:07:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 13:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 13:07:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 13:07:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 13:21:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 13:21:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 13:21:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 13:21:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 13:51:10 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 19:36:26 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 19:36:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 19:36:27 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 19:36:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 19:36:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:45:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 19:45:45 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:45:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 19:45:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 19:45:47 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 19:45:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 19:45:48 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 19:45:48 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 19:45:48 GMT
CMD ["php-fpm"]
# Fri, 02 Oct 2020 01:14:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 19:52:04 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:52:05 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 19:52:05 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 19:54:52 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Thu, 08 Oct 2020 19:55:32 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:55:33 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 19:55:34 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 19:55:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 19:55:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b3577b786a8fc924e77061e0347784852f282e0c823a01d273188d615f3c37`  
		Last Modified: Thu, 10 Sep 2020 16:10:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60538287851f83ed7cc28af3c1fdc4dc70a191246efe8076aacfaca909833f51`  
		Last Modified: Thu, 10 Sep 2020 16:10:38 GMT  
		Size: 76.7 MB (76652017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53ff72fe22523d07d5c67bbb6672cc482f34b724d6a788b7895afc35e48332b`  
		Last Modified: Thu, 10 Sep 2020 16:10:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c222f4cd715f61ff0593ce234a067d772d18ca350c56973f8288be16c597322`  
		Last Modified: Fri, 02 Oct 2020 00:43:18 GMT  
		Size: 10.6 MB (10623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d143941282c5fe189ff8149a671760b5a54d79e7aeaad5116750ea05925654d3`  
		Last Modified: Fri, 02 Oct 2020 00:43:13 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddef4337bccbfc73df9a871a21c0c09a27d3293824d8a8cf43d00929060617d6`  
		Last Modified: Fri, 02 Oct 2020 00:43:19 GMT  
		Size: 28.5 MB (28542588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3101cbea2e176faaaef5755be31084e7d2f6a7c141e2e520c443703678f08af8`  
		Last Modified: Fri, 02 Oct 2020 00:43:14 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9224738969c921ad4506ae18807020d616466da35979e854f26b6e2033f65f91`  
		Last Modified: Fri, 02 Oct 2020 00:43:14 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31726538378edc1e67137ea0c8ec95e44a659f1d6b0190b21f3476442e5680b9`  
		Last Modified: Fri, 02 Oct 2020 00:43:14 GMT  
		Size: 8.5 KB (8452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72598a1acdf53c5f584949050bf0c618f2252621a49d3f0dacc2da2f7d52cd2b`  
		Last Modified: Fri, 02 Oct 2020 01:29:58 GMT  
		Size: 1.6 MB (1635675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25268310922430e875e5cdd9d58807f221a495817d27f20e3ffc0ade98d4998e`  
		Last Modified: Thu, 08 Oct 2020 20:01:21 GMT  
		Size: 16.5 MB (16524813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca13b03cd8d6664af667ef729e40ccef49bedbdecc4b7cde862a25ce48680d`  
		Last Modified: Thu, 08 Oct 2020 20:01:17 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6c03be2562cd88135a2c937c744d753452401f3a02eeffe2e4c92761b17aad`  
		Last Modified: Thu, 08 Oct 2020 20:03:45 GMT  
		Size: 130.3 MB (130298261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee829f1daae7f5ae9e03dad842848c3bec4cf6a0ab8ded85ea41da310475ec6`  
		Last Modified: Thu, 08 Oct 2020 20:03:17 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c338e641f88d29d5fdfc356e91185d4f09b64ff1e75091be6d11069ea35322`  
		Last Modified: Thu, 08 Oct 2020 20:03:17 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:44b07729ee34ff7e93b81b155740771eeb800b3b2d8796c276a2cd659e705e00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268392124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb8681973b52a1b206bb97cc66a713cf6d8afeeea94a9b58a6bffdca175fd59`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:19:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 02:19:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 02:20:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:20:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 02:20:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 02:31:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 02:31:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 02:31:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 02:31:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 02:55:11 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 18:58:19 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 18:58:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 18:58:22 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 18:58:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 18:58:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:02:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 19:02:43 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:02:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 19:02:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 19:02:52 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 19:02:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 19:02:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 19:02:57 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 19:02:57 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 21:19:13 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 19:45:26 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:45:29 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 19:45:30 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 19:48:41 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Thu, 08 Oct 2020 19:49:50 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:49:52 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 19:49:55 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 19:49:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 19:49:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca52621e29f0be906227dd042c4f23109d45e98133e6803aee1fad26c1b9853`  
		Last Modified: Thu, 10 Sep 2020 04:34:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3919fd67c6fcaafe16fd897b661b5e1035df3defb96c7a2889e35349a70445f`  
		Last Modified: Thu, 10 Sep 2020 04:34:26 GMT  
		Size: 58.8 MB (58801370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cac75e8ebdf4a331c6f82fe7860ac1631d98af62eeb150a688a5e59f4a4a13`  
		Last Modified: Thu, 10 Sep 2020 04:34:02 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd141a03167afe17bccafc9635becbf8fe5647bc69277e74816c416317e5007`  
		Last Modified: Thu, 01 Oct 2020 20:41:44 GMT  
		Size: 10.6 MB (10621550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6484ae0c3a55fcb2050d5e1c75cf2deef1e4b8b1daeb35adc5918ed9fc28dd`  
		Last Modified: Thu, 01 Oct 2020 20:41:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b586c1d580a907eca66714620cbeb7180494af1eff8cfedb2ed1bf0042de03`  
		Last Modified: Thu, 01 Oct 2020 20:41:47 GMT  
		Size: 27.2 MB (27162757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a5bf9bedf7952f7a6fd59b85607851546953940708dd0f82d95daf680963a6`  
		Last Modified: Thu, 01 Oct 2020 20:41:38 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d555dfaf5dbe7624e0c2c9f589e3dded085cf63343f4a72ff141a09ad5a74b`  
		Last Modified: Thu, 01 Oct 2020 20:41:37 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d78d6855ea4129be27e1b6ed5fa9ba2149c509a1ad89f0a7ccca5603af0f7f`  
		Last Modified: Thu, 01 Oct 2020 20:41:38 GMT  
		Size: 8.5 KB (8453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd89319ad305602f1bfe20d968ad05f8d553f47fd8367119ceb75b0d83a38a4`  
		Last Modified: Thu, 01 Oct 2020 21:36:35 GMT  
		Size: 1.6 MB (1573610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf023046fbd2d99d811e71d6a3dd52076f0829b555990d54c2ff3af20e3db207`  
		Last Modified: Thu, 08 Oct 2020 19:55:14 GMT  
		Size: 15.1 MB (15082989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91627b9cce18e7581626174076ca607ca6b20387d885a4225a280dcc8579a05`  
		Last Modified: Thu, 08 Oct 2020 19:55:09 GMT  
		Size: 536.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5871922d2292e6d75bb3df375a6cfad330edcd33b29b78e394c195ce463218d`  
		Last Modified: Thu, 08 Oct 2020 19:57:47 GMT  
		Size: 130.3 MB (130296945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855cf75286cc8d2a5cba592c923290c7fbf94f045c22b680bc71aacdf969888a`  
		Last Modified: Thu, 08 Oct 2020 19:57:01 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4c81f6c75814ca72c1f023f4d9cde0bec55177ebc288aeac494f5f70190e1b`  
		Last Modified: Thu, 08 Oct 2020 19:57:01 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:08c8f0c6c9e8b6871378e15a481059f40291b222155cf4716c82c4414049e06a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.8 MB (264755603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1632acb4d808d7b933c6da25abfdea65fe59d311050a49723bfe9a40a05ba43c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 08:24:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 08:24:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 08:25:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 08:26:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 08:26:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 08:38:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 08:38:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 08:38:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 08:38:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 08:59:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 19:09:26 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 19:09:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 19:09:27 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 19:09:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 19:09:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:13:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 19:13:40 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:13:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 19:13:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 19:14:01 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 19:14:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 19:14:12 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 19:14:13 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 19:14:13 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 23:20:28 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 01 Oct 2020 23:25:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 01 Oct 2020 23:26:36 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 01 Oct 2020 23:26:44 GMT
VOLUME [/var/www/html]
# Mon, 05 Oct 2020 22:34:46 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Mon, 05 Oct 2020 22:36:25 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Mon, 05 Oct 2020 22:36:29 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Mon, 05 Oct 2020 22:36:35 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Mon, 05 Oct 2020 22:36:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Oct 2020 22:36:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a7c65856610cb24c46ede2ffe313cbf933c44fa20ba213835af953646f3eb1ed`  
		Last Modified: Thu, 10 Sep 2020 00:17:52 GMT  
		Size: 22.7 MB (22699896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643be151265f556a263774f5b21b7accd984f18c255388e7760c8d2d44416fd0`  
		Last Modified: Thu, 10 Sep 2020 10:47:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a849c10c3e87343a463ee7084ac0544d6b8499ddc44119b7612900ba8d1f9426`  
		Last Modified: Thu, 10 Sep 2020 10:48:15 GMT  
		Size: 59.5 MB (59507912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333d40d36c170afca40c7040d7daff5778b30f80388c97c53b96297729b8c52f`  
		Last Modified: Thu, 10 Sep 2020 10:47:57 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6662b322d159607801053d02c7d33fe30d275c5c767bced0a2ba570847171a`  
		Last Modified: Thu, 01 Oct 2020 21:51:47 GMT  
		Size: 10.6 MB (10621484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918657105214ba30efbf88d4039a8d855ced3fd56fd6a8488b45a04fb04228b1`  
		Last Modified: Thu, 01 Oct 2020 21:51:43 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7d0878a0fc80b64bacb58289f57c1ee6d9dafbb2ea7c6379c64e8d8b6e33e`  
		Last Modified: Thu, 01 Oct 2020 21:51:53 GMT  
		Size: 26.2 MB (26171167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2ab622a39c919fb33dcb2a4484a25b76114ac58b3eb2a8f4327b18616e0208`  
		Last Modified: Thu, 01 Oct 2020 21:51:44 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d4962bea3f6f00accc36eb7dbd67a5760a00568f1cf29acf0761d294d9c7e`  
		Last Modified: Thu, 01 Oct 2020 21:51:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6052d02b85076c8cafc262d5efd558c7756e242e35b922033a510839a649e28`  
		Last Modified: Thu, 01 Oct 2020 21:51:43 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f145005a28040c385492350da8b9c32958ea42fb5a23183abd412aa50bf11ac`  
		Last Modified: Thu, 01 Oct 2020 23:53:38 GMT  
		Size: 1.4 MB (1425604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be53fa7bf498fa0a6321d9583240e956e9590a8e5da447e5cac2c0aadf6aacf2`  
		Last Modified: Thu, 01 Oct 2020 23:53:41 GMT  
		Size: 14.0 MB (14015693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b552a079ce525b2bb0e1249e50c426f82be1e970de8084f47332c239aea6f1`  
		Last Modified: Thu, 01 Oct 2020 23:53:36 GMT  
		Size: 532.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0e4e88a31c8e123e3c4b4035a8fd72895e8c6700d25d6b29f9657e82cbb49`  
		Last Modified: Mon, 05 Oct 2020 22:47:45 GMT  
		Size: 130.3 MB (130296922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f1d8ec2f16751b7d3936bd90b66b2e83ad4dcb6304c35569ea5f2216afbde1`  
		Last Modified: Mon, 05 Oct 2020 22:47:03 GMT  
		Size: 2.5 KB (2523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4704dbdd9a447b87e2c2365c5479bb1ea186c02e09a540fe290e3cda6c926609`  
		Last Modified: Mon, 05 Oct 2020 22:47:03 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:8e00fb5c2d67f336d620e913691ac99aadc6faeb314b411caeb393f6a7495baf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.9 MB (281890135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e787f5b9ad0ca58daca29b8b018b177ad608567f7fc0423f32aad920eebac815`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:03:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 12:03:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 12:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 12:04:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 12:04:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 12:13:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 12:13:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 12:13:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 12:13:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 12:33:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 18:48:07 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 18:48:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 18:48:08 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 18:48:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 18:48:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:51:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 18:51:54 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:52:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 18:52:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 18:52:08 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 18:52:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 18:52:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 18:52:22 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 18:52:25 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 22:31:56 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 19:50:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:50:05 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 19:50:06 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 19:54:13 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Thu, 08 Oct 2020 19:55:21 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:55:26 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 19:55:29 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 19:55:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 19:55:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b765cd8dd18ccad037620f2765e6c4d1d213e1efd39d254ed77be7e075bde1b`  
		Last Modified: Thu, 10 Sep 2020 14:15:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c348cef873eb53c0c25878ea8bc2e47bfb9eb575a1b3138fc1ef02731b8840f`  
		Last Modified: Thu, 10 Sep 2020 14:15:45 GMT  
		Size: 70.3 MB (70337546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76bca23f69b13b0ba97ffcb96964a27c90a234bb33d13b977d46f15defb9299`  
		Last Modified: Thu, 10 Sep 2020 14:15:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eed3947bd405ce9c5cb006318ea37145761521665832a1ee8f420be3832d438`  
		Last Modified: Thu, 01 Oct 2020 21:34:54 GMT  
		Size: 10.6 MB (10622290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19d2b62bbc38505936fb24816c4b0fb7a382bdbb00d917d522efc53a9db4732`  
		Last Modified: Thu, 01 Oct 2020 21:34:51 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591b747e24f83f60b809b8110a15f8a4f9b7a826b22273667b3a3c605b7db1e8`  
		Last Modified: Thu, 01 Oct 2020 21:34:58 GMT  
		Size: 28.3 MB (28308238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcada6f7890808375bb42d967b52fe86770932000ea0fd1dfda07f892c8480ba`  
		Last Modified: Thu, 01 Oct 2020 21:34:50 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f88b702ce8416f05c49e052ad2703608a725be6e00b7ef494506e7c7a1a3f`  
		Last Modified: Thu, 01 Oct 2020 21:34:50 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be4f4d5f0f70663e59b05948df84a109d52c5d6b527f6c06760dd511f60612`  
		Last Modified: Thu, 01 Oct 2020 21:34:51 GMT  
		Size: 8.4 KB (8450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2645c4ef57bc3e1c6e80d58bc345617b386653d4bd55cf688de96d2e5babff`  
		Last Modified: Thu, 01 Oct 2020 22:57:09 GMT  
		Size: 1.6 MB (1602344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d5eef92618dbd42d14e65b53059271a530ab56798c2bbb8a116beb083bef32`  
		Last Modified: Thu, 08 Oct 2020 20:02:08 GMT  
		Size: 14.9 MB (14855626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d6366f97626d557824140f105c243fa5e8055fd3878d5ec44a73a4d0d3c93d`  
		Last Modified: Thu, 08 Oct 2020 20:02:04 GMT  
		Size: 535.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4269bc2d55bfd89a148d132b2f6c5a447e4c3bcdd301751bd7e4b3baad4a345b`  
		Last Modified: Thu, 08 Oct 2020 20:05:12 GMT  
		Size: 130.3 MB (130297846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cce283ca81690ba4cbc4c721e72d5c309e4193e66391a83edeb6b38dd4254c`  
		Last Modified: Thu, 08 Oct 2020 20:04:38 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b6ead55732802c9c04044592395a72dfbc8f7385f5544add0d89bdcc8a26cb`  
		Last Modified: Thu, 08 Oct 2020 20:04:38 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; 386

```console
$ docker pull nextcloud@sha256:b2ac616cdd93ed5b5c8739297aa5728db99c368b8843b63a8b1a22e1a37da80e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.5 MB (296532541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6906de8dca77a2da8df8cb834f7e9c0ee33ad6ff21e46152cb3992c664242a7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:59:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 07:59:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 08:00:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 08:00:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 08:00:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 08:18:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 08:18:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 08:18:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 08:18:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 08:50:54 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 18:49:07 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 18:49:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 18:49:07 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 18:49:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 18:49:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:54:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 18:54:23 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:54:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 18:54:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 18:54:24 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 18:54:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 18:54:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 18:54:26 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 18:54:26 GMT
CMD ["php-fpm"]
# Fri, 02 Oct 2020 00:53:14 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 19:43:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:43:18 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 19:43:18 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 19:46:15 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Thu, 08 Oct 2020 19:47:26 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:47:27 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 19:47:28 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 19:47:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 19:47:28 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4499d39307af22ef88aa638bef03c5200dff89508044e2c60c643661d7c32428`  
		Last Modified: Thu, 10 Sep 2020 11:36:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2a27492887c5f58eef5824ca61cad1ff9fe49b5516d22376a78d3512ab4f1b`  
		Last Modified: Thu, 10 Sep 2020 11:36:42 GMT  
		Size: 81.2 MB (81195618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b173dfa8aeceae006c385cf967f923282ff5dfc5d2587884d84158a283e8e8c`  
		Last Modified: Thu, 10 Sep 2020 11:36:12 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e542c0407b6ca77318666986a48b4f7f0a21da6f27e7183ce6f58ada22b4e9`  
		Last Modified: Fri, 02 Oct 2020 00:14:11 GMT  
		Size: 10.6 MB (10622681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fbca042085d2f03fdf7171c8ec16ab87f42515de31fdc5475a403d8252354`  
		Last Modified: Fri, 02 Oct 2020 00:14:06 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20586b946b800977c0697edf3b4444f62efdc54558cb736fdbd973536a1388d3`  
		Last Modified: Fri, 02 Oct 2020 00:14:22 GMT  
		Size: 29.1 MB (29122419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a08c16725aaa3fb6f08ec4730685dd75b1eca767860e9100aa0a348955772`  
		Last Modified: Fri, 02 Oct 2020 00:14:06 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759fb68a06915e833d66f0c15d4ec555aa070786118d0fdd568ec207a71d42cf`  
		Last Modified: Fri, 02 Oct 2020 00:14:06 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90eb2b7f15125e40dcb58dc8208f89746468e4c4e042e4e520a3eec5bf6c4354`  
		Last Modified: Fri, 02 Oct 2020 00:14:06 GMT  
		Size: 8.5 KB (8452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989b33cae33a5b3c11f8cff30fbb633e0eb11fac936a4e9832fa8531a9b9efd4`  
		Last Modified: Fri, 02 Oct 2020 01:06:50 GMT  
		Size: 1.7 MB (1659651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb670c2e29296b67f66116282fa3b4042e53f8e140f1fac2a6cd573ed1e5db3a`  
		Last Modified: Thu, 08 Oct 2020 19:53:44 GMT  
		Size: 15.9 MB (15867154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f6237f3da14c53c49980183191fabd83801c3a4617e187a1c06f41a4e845a9`  
		Last Modified: Thu, 08 Oct 2020 19:53:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb3501b6430545d1a77ed25fd0d21f95e0e97100db0b048fd71e8ec03c6264`  
		Last Modified: Thu, 08 Oct 2020 19:56:45 GMT  
		Size: 130.3 MB (130297836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3710e5c1a13578c316686a5f66403285ae61b8596bc80213f71b2c0daa88e9`  
		Last Modified: Thu, 08 Oct 2020 19:56:06 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fededb3c16165cf62e755d3c262cb3cbca47d5f72d0a6faa186dcbabf2d00258`  
		Last Modified: Thu, 08 Oct 2020 19:56:06 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; mips64le

```console
$ docker pull nextcloud@sha256:bbb94f02121676bcff6a8d63984ad7cd66e7b4bce5c07246d5d18eb963ecc110
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272670099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cdbe742fba8a8e52f1a9d6c5d1db42f69aa73a19b7a9e342170da69deed7d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 10 Sep 2020 00:10:03 GMT
ADD file:dec5e74bd1dacf4dd26507ac5227dfca6591d05d13bdf06c16217b9efff06ed9 in / 
# Thu, 10 Sep 2020 00:10:04 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 13:14:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Sep 2020 13:14:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Sep 2020 13:15:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 13:15:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Sep 2020 13:15:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Sep 2020 13:41:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 15 Sep 2020 13:41:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Sep 2020 13:41:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Sep 2020 13:41:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Sep 2020 14:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 19:29:31 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 19:29:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 19:29:31 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 19:29:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 19:29:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:42:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 19:42:28 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:42:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 19:42:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 19:42:31 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 19:42:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 19:42:33 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 19:42:33 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 19:42:34 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 21:27:12 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 20:00:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 20:00:06 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 20:00:06 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 20:04:29 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Thu, 08 Oct 2020 20:06:12 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 20:06:15 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 20:06:17 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 20:06:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 20:06:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3e11c32dbce8eae675cead1f63aeade46d661eb3764bff6c26bb8ca6e2c364fb`  
		Last Modified: Tue, 15 Sep 2020 01:13:19 GMT  
		Size: 25.8 MB (25762660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73debcd652f37bb4d5f93765d53fedb44c5a9ef2a2886f7802225a95aae86`  
		Last Modified: Tue, 15 Sep 2020 15:52:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab85c92b3a5acb56954ee8f14a4d3869b6e2f3324638cd0ba434cb8b7544ca`  
		Last Modified: Tue, 15 Sep 2020 15:53:10 GMT  
		Size: 61.4 MB (61389317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec3ebf555d5e153773a45213e85adb3bfc1782a517543e560d18989d47a17e6`  
		Last Modified: Tue, 15 Sep 2020 15:52:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec42332e0e931f894497a53a0ef69d12b2465eb05b8a324f22883986e7fbb7a`  
		Last Modified: Thu, 01 Oct 2020 20:49:59 GMT  
		Size: 10.6 MB (10620734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e867eb5ddc410099a15459179cfce3360466e68c8ac81152d9254fd30c9750f`  
		Last Modified: Thu, 01 Oct 2020 20:49:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8cf0d26fa65e28d16b8fa293a1375b9245efe9b3d2bbd64efe03a357477c02`  
		Last Modified: Thu, 01 Oct 2020 20:50:14 GMT  
		Size: 27.9 MB (27911895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba8df1b7e676524465395d806330ada9fad621dd38d16a332e94633d8717cd`  
		Last Modified: Thu, 01 Oct 2020 20:49:53 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0152e25f03fb1ae8cbfb22ff6c459e282b0e6ee59f67c9bc67d683767d22bef3`  
		Last Modified: Thu, 01 Oct 2020 20:49:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc3de7851c539bfeb6a33d074cc6874874c2f1e0685cdd93e5eec184e5bef61`  
		Last Modified: Thu, 01 Oct 2020 20:49:54 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db0f876fae49ee6cf8c3c25a14c1ea427b7453dce13cffeb20106270c7cbed5`  
		Last Modified: Thu, 01 Oct 2020 21:49:35 GMT  
		Size: 1.7 MB (1740060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3dc298678b0f03fb9ea7e1da6b606bc7bbf20cd789bbf206dd3562d2e0d848`  
		Last Modified: Thu, 08 Oct 2020 20:14:29 GMT  
		Size: 14.9 MB (14931586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6797c441868def59a0e85836ecd275e358b2356b14b274547dc9c3df548181fb`  
		Last Modified: Thu, 08 Oct 2020 20:14:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e566383922c2bbf2b012de12f87e0b9103c5ccde35aba525c0b45d1b896af325`  
		Last Modified: Thu, 08 Oct 2020 20:19:03 GMT  
		Size: 130.3 MB (130296997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fcecb4979e2154c67cd969160931cacbc085db71fa13b56b8719c0e461bcd9`  
		Last Modified: Thu, 08 Oct 2020 20:17:44 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a4906ff569006190631fda7f46f4badaf17cf6f041a03e4072ad3a7433a3df`  
		Last Modified: Thu, 08 Oct 2020 20:17:44 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:afa4addc63674307b882ec2924ba472aaec6ed4ddaec0805d6ea8d11dc384725
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.5 MB (302490467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cadb0270c17b25c2ee91a400a2e7329a782250a8614e4ee3087e060d79967d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 11:58:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 11:58:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 12:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 12:01:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 12:01:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 12:25:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 12:25:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 12:25:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 12:25:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 13:16:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 19:35:56 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 19:36:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 19:36:03 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 19:37:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 19:37:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:42:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 19:42:44 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:42:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 19:42:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 19:42:59 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 19:43:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 19:43:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 19:43:13 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 19:43:17 GMT
CMD ["php-fpm"]
# Fri, 02 Oct 2020 00:22:21 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 02 Oct 2020 00:34:21 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Oct 2020 00:34:38 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 02 Oct 2020 00:34:44 GMT
VOLUME [/var/www/html]
# Tue, 06 Oct 2020 07:41:46 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Tue, 06 Oct 2020 09:16:41 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Oct 2020 09:16:56 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Tue, 06 Oct 2020 09:17:00 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Tue, 06 Oct 2020 09:17:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Oct 2020 09:17:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b6d09588296694c116e9adc99909df057a299ccb72aaf6929e3df19b421dab`  
		Last Modified: Thu, 10 Sep 2020 15:32:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2b21df1bee324f13738f65d0318ece3f0e9f0569ce6b32ddd30f67f34204e4`  
		Last Modified: Thu, 10 Sep 2020 15:33:25 GMT  
		Size: 82.3 MB (82260209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d861da2f7d287a59a9e7f854ef705258cd56635a414e1361c62a90f6e142701`  
		Last Modified: Thu, 10 Sep 2020 15:32:07 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff9b659e7f5e4112786244b846a3b3d0e09f14631c612e16c6019a5cd3ff10`  
		Last Modified: Thu, 01 Oct 2020 22:34:47 GMT  
		Size: 10.6 MB (10623396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7334b038bbbe3b24e3bcdc620938690c2743ea2e3ec63a4fe37631c83904e1`  
		Last Modified: Thu, 01 Oct 2020 22:34:23 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42246379da8a77920ee6c47675e46def2e3bdd6da1741e7b9b7b3412944946d2`  
		Last Modified: Thu, 01 Oct 2020 22:34:38 GMT  
		Size: 30.2 MB (30228002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a366f6ce9e1c307e72b78ec851537bf65618779b4e63ab1a5539e22a249ea1ac`  
		Last Modified: Thu, 01 Oct 2020 22:34:23 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5862df2fcf37d6a9554149f63a3cf4dd4b95c44ab49f88dc6aaa346c4f9e79`  
		Last Modified: Thu, 01 Oct 2020 22:34:23 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2cc6d4749e8241f3885b3588bc0554b83f9ba1d9ebcf1fc4625711cb7878dd`  
		Last Modified: Thu, 01 Oct 2020 22:34:23 GMT  
		Size: 8.5 KB (8454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de629f0d5a5f9fe9b74111dd57025a1d06f3ad131bdd60da5305d71a5c85afe`  
		Last Modified: Fri, 02 Oct 2020 01:15:17 GMT  
		Size: 1.8 MB (1803140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ede20c7ec8933694f062a72aeca5dd92b522b18232db06580fd46c87a75d798`  
		Last Modified: Fri, 02 Oct 2020 01:15:28 GMT  
		Size: 16.7 MB (16740609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5cc636b717e7afad2a0b57cc107e685378cbd78b784403eebc48cce48d7245`  
		Last Modified: Fri, 02 Oct 2020 01:15:09 GMT  
		Size: 536.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8bd615ed3249802d018322c9ab3ab0363f87d413c0ed06c39bdeb3ce0b23d`  
		Last Modified: Tue, 06 Oct 2020 09:40:09 GMT  
		Size: 130.3 MB (130300296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404100d2ff05962b3a1e19bdd1607a4371ccfd170e41b562fc2870d067159e04`  
		Last Modified: Tue, 06 Oct 2020 09:37:48 GMT  
		Size: 2.5 KB (2523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65e86bc1b70e7414c27d440aaea54a5a42bd56c79b48118ae2bda4f02f6b69e`  
		Last Modified: Tue, 06 Oct 2020 09:37:48 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:20-fpm` - linux; s390x

```console
$ docker pull nextcloud@sha256:3ca7288c35b605eb5d649fa2f8767aa4b2921d7813e38c092cadfd58a5f76eb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.6 MB (275612866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb36a006e8d55cfa892aa117d16c9382daf644f77f2461d340b490d6c66bbe0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:08:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 03:08:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 03:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 03:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 03:09:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 03:15:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 10 Sep 2020 03:15:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 03:15:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 03:15:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 03:25:10 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 18:47:32 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 18:47:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 18:47:33 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 18:47:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 18:47:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:50:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 18:50:03 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:50:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 18:50:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 18:50:04 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 18:50:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 18:50:05 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 18:50:06 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 18:50:06 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 20:28:43 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 19:51:53 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:51:55 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 19:51:55 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 19:54:30 GMT
ENV NEXTCLOUD_VERSION=20.0.0
# Thu, 08 Oct 2020 19:55:14 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Oct 2020 19:55:19 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 19:55:20 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 19:55:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 19:55:20 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41f81f5ba533e5fb32c0cfcf148fd10f7157036df317d3440322ee13328ea09`  
		Last Modified: Thu, 10 Sep 2020 03:54:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4e35c34d5aea8c49d40ce4058e764f58b846eea3c34245ea9040071aff201c`  
		Last Modified: Thu, 10 Sep 2020 03:54:34 GMT  
		Size: 64.7 MB (64706227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe2203ba81a2f860cc2e28027c6f86906241199bd4c535778c6f7a7ddb66cc`  
		Last Modified: Thu, 10 Sep 2020 03:54:24 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67295e107e7111122ec9d522ddd2b505c6b7394a38b16c3d2042cb26e3066ac`  
		Last Modified: Thu, 01 Oct 2020 20:03:46 GMT  
		Size: 10.6 MB (10621742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc6398c77ec34f8adb371a50a47cc8fa6733134496712c057fa91445f2f6820`  
		Last Modified: Thu, 01 Oct 2020 20:03:44 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b6b9d5ea3c2a9ba345aed452ce1eb20688cd1b94b17e80b597dc213958c1ea`  
		Last Modified: Thu, 01 Oct 2020 20:03:50 GMT  
		Size: 27.7 MB (27654235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00d1b550b104daccbd86dc63bb7184e1a29d5b72758e8c19d836af623f8defe`  
		Last Modified: Thu, 01 Oct 2020 20:03:42 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d535dafaf3e6c2901c4e559b21777b0211670face757a75e80626b74fc5a31c`  
		Last Modified: Thu, 01 Oct 2020 20:03:43 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75be4a0e823dd759c0834f824f6a0298f72367b5804460a63524e320c4692720`  
		Last Modified: Thu, 01 Oct 2020 20:03:42 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1711897627049e1d1f585ade4bde07394e1e7eb4d5ff735f89ebaaa3830a27`  
		Last Modified: Thu, 01 Oct 2020 20:38:28 GMT  
		Size: 1.6 MB (1594998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810348fdd4d637d0360b6a90813154093a7e78d791104ea09404ecdeb8ea025`  
		Last Modified: Thu, 08 Oct 2020 20:01:17 GMT  
		Size: 15.0 MB (15014331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844eef946ee865b8a0fd910f975ddc3910d01a964305cd5ab5ce07e5f554fc76`  
		Last Modified: Thu, 08 Oct 2020 20:01:15 GMT  
		Size: 534.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79ec329b2cd2843c24473fe50e1e0a80d4bb3f06dda6077b14d27e4bf985020`  
		Last Modified: Thu, 08 Oct 2020 20:07:50 GMT  
		Size: 130.3 MB (130296810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77da48d62222a4b9410943c81989f07b57d4d83000971dde605236336cb5c0bb`  
		Last Modified: Thu, 08 Oct 2020 20:04:21 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fce2424ed9e94a7fef2a48dd5bffea22bda04edc6b4fd15718ad7a843b490b9`  
		Last Modified: Thu, 08 Oct 2020 20:04:21 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
