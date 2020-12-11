## `monica:fpm`

```console
$ docker pull monica@sha256:2fb56dbb7323ff23bfe5343fce4fb59d9d6fe7a2865c98ac31e4336da49495f4
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

### `monica:fpm` - linux; amd64

```console
$ docker pull monica@sha256:fb0de32e7ab19e791b942623d105e16392938b31cb07f40f92c1ef802845763f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.1 MB (201132788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ebfa518fc857d8177339dd2d0be06c911c26141191b1277bfb72db6fc650ec`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 08:44:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 08:44:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 08:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 08:44:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 08:44:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 09:02:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 09:02:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 09:02:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 09:02:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 10:07:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 01 Dec 2020 05:42:56 GMT
ENV PHP_VERSION=7.3.25
# Tue, 01 Dec 2020 05:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Tue, 01 Dec 2020 05:42:57 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Tue, 01 Dec 2020 05:43:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Dec 2020 05:43:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 05:51:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 05:51:01 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 05:51:03 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 05:51:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 01 Dec 2020 05:51:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 05:51:06 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 05:51:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 05:51:08 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 05:51:08 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 05:51:08 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 09:43:46 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Tue, 01 Dec 2020 09:43:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 09:46:40 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 09:46:41 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Tue, 01 Dec 2020 09:46:41 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Tue, 01 Dec 2020 09:46:42 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Tue, 01 Dec 2020 09:46:42 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 09:46:42 GMT
ENV MONICA_VERSION=v2.19.1
# Tue, 01 Dec 2020 09:46:43 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Tue, 01 Dec 2020 09:47:07 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 09:47:09 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Tue, 01 Dec 2020 09:47:09 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 01 Dec 2020 09:47:09 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266fc315b0155934606f2688364a42d4233b2a7605f51f06d6aced8c88fe2e6`  
		Last Modified: Wed, 18 Nov 2020 12:03:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8a5fa787a1ee6c4cb42f9b382aacfeb33d97504cbd3d35e23727bab752e5cd`  
		Last Modified: Wed, 18 Nov 2020 12:04:07 GMT  
		Size: 76.7 MB (76652404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc127c18841756f8fef538b2136f8b2c1c90b972c621e0f7885f7fbc7a15cb`  
		Last Modified: Wed, 18 Nov 2020 12:03:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2570f74bf29cd1f85cf71c7fd1ecbc0417fd0becd4886c70899d9d00e6ac8dc8`  
		Last Modified: Tue, 01 Dec 2020 07:28:39 GMT  
		Size: 12.5 MB (12458285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf6d4b9bc7039f5821bbc74aa1e4d8b74ad8e6861b38ee9583e8c2de46e5d99`  
		Last Modified: Tue, 01 Dec 2020 07:28:38 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e9411b68b1f12245f7b61683e68c390e8d0a6aa77a48eeb608d4e9a0676f4`  
		Last Modified: Tue, 01 Dec 2020 07:28:43 GMT  
		Size: 28.8 MB (28767104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e4882cd798a73a51332c484457172341a46652240a85f51bb848c28af75ec8`  
		Last Modified: Tue, 01 Dec 2020 07:28:38 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf90b12ffa778cae4e07da64cde976c7bd9fe86e93443788f2c9b4a56163919`  
		Last Modified: Tue, 01 Dec 2020 07:28:37 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f784670350194b8ed1838283249c811cdf969e5641435da2a2f02d2306ac19a6`  
		Last Modified: Tue, 01 Dec 2020 07:28:37 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cab5625ec5f964c27562f4666bbf283788a01e7296291c854740506fa41885`  
		Last Modified: Tue, 01 Dec 2020 07:28:37 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322a1ffc890d4f859398c778dbec95b26876b3982d512fa102168103a01eff98`  
		Last Modified: Tue, 01 Dec 2020 09:50:43 GMT  
		Size: 1.3 MB (1332554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c96f865d18a013847f71c29f5cfa962feb96f913c9736318e354bb136ad595`  
		Last Modified: Tue, 01 Dec 2020 09:50:45 GMT  
		Size: 16.2 MB (16207265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4397c088e07734e1bb4c6c5c9bcfa32f8ea9432ef28afe7ebea11e027c3be2a0`  
		Last Modified: Tue, 01 Dec 2020 09:50:41 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823425a960b151cad883438509628a8b59be8bd0ee6028f6ec1a0326d945d99c`  
		Last Modified: Tue, 01 Dec 2020 09:50:41 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563996407cf218137fd6bc7b3cd50a524542de0c42db3c6393931ccbcd0b616`  
		Last Modified: Tue, 01 Dec 2020 09:50:54 GMT  
		Size: 38.6 MB (38595555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738190a324b994932dc3b50d6c68b1c30d36720957f47a372df7fbeb214655d4`  
		Last Modified: Tue, 01 Dec 2020 09:50:41 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; arm variant v5

```console
$ docker pull monica@sha256:b908ddc066a6567e4247629a4d63cd461d80b9ccd8128d0fcfbb8fe949175e1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178069002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e780787fb62d46fb1d366d7a54915dbdca4aac99e4d3378e689c24958e708770`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 07:13:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 07:13:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 07:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 07:13:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 07:13:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 07:23:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 07:23:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:24:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:24:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 08:01:41 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 11 Dec 2020 08:01:42 GMT
ENV PHP_VERSION=7.3.25
# Fri, 11 Dec 2020 08:01:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Fri, 11 Dec 2020 08:01:44 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Fri, 11 Dec 2020 08:02:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 08:02:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 08:06:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 08:06:06 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 08:06:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 08:06:14 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 11 Dec 2020 08:06:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 08:06:17 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 08:06:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 08:06:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 08:06:25 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 08:06:28 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 18:07:22 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 11 Dec 2020 18:07:32 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:12:00 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:12:03 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 11 Dec 2020 18:12:04 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 11 Dec 2020 18:12:06 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 11 Dec 2020 18:12:07 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 18:12:07 GMT
ENV MONICA_VERSION=v2.19.1
# Fri, 11 Dec 2020 18:12:08 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Fri, 11 Dec 2020 18:13:32 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:13:39 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Fri, 11 Dec 2020 18:13:40 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 11 Dec 2020 18:13:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed9b2f20ffb0bcade877c21585737821b1abdd1b29ec2742ef3d8bc1a8a71b2`  
		Last Modified: Fri, 11 Dec 2020 09:10:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086596dbe8ce93733486082312fbe0cffefc063795aa2ae18459ce018c64bd`  
		Last Modified: Fri, 11 Dec 2020 09:10:30 GMT  
		Size: 58.8 MB (58801419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5a47fff6f79bd0fed3070e2cbe30a88324dcd19c6597080333fabbf9adf49d`  
		Last Modified: Fri, 11 Dec 2020 09:10:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cb77578e324ec267cdc57171ff321abd5533c01d04f5a7d79407df90878435`  
		Last Modified: Fri, 11 Dec 2020 09:14:47 GMT  
		Size: 12.5 MB (12456382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601336e0a1ca8d29db93bf56223921f72fac6a6af0125387d98bdae41f39c9c9`  
		Last Modified: Fri, 11 Dec 2020 09:14:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7e4625e96c688145addffce6b3694743c2b7c89b1d739b11225e2ab2fad317`  
		Last Modified: Fri, 11 Dec 2020 09:14:51 GMT  
		Size: 27.3 MB (27320800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84e9102552597fa5748a73342bbbbe88cf31f44072add24405a0f714351ae7d`  
		Last Modified: Fri, 11 Dec 2020 09:14:43 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249045e4c5dfb2dc71367b77f506c602a48ee7f199465da42eeab5947a10bf12`  
		Last Modified: Fri, 11 Dec 2020 09:14:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386283599a3a889e40d74725185ba9e13aafb5cd034ca2bc6434f4356bd85b61`  
		Last Modified: Fri, 11 Dec 2020 09:14:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a423d36d4579cb4afdfa8e00ebc293b2e8d1136107dde738ff2614a1aa67bd`  
		Last Modified: Fri, 11 Dec 2020 09:14:43 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc3697c6cd6c53c953048ed9cb2b7260bd9497d44244590f39fc62d532bcac5`  
		Last Modified: Fri, 11 Dec 2020 18:14:52 GMT  
		Size: 1.3 MB (1271656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223e2efcd94b1cdb43ae5ec5d80f7e788b26021fa867dbfc9c57863025da4ade`  
		Last Modified: Fri, 11 Dec 2020 18:14:54 GMT  
		Size: 14.8 MB (14767705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ce24387d491cde7e4cd88e67016f73fe4f2e0265b02b7b457893e55cd081c`  
		Last Modified: Fri, 11 Dec 2020 18:14:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31811a22d198023a600512b324b1575b458caa79558858996a43b825c8928a6`  
		Last Modified: Fri, 11 Dec 2020 18:14:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b9e77b7c7e94501d97a9a4bfdc31b1413d14e9ea6c40c02bc8bde4c136efa`  
		Last Modified: Fri, 11 Dec 2020 18:15:10 GMT  
		Size: 38.6 MB (38593370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637daf36e7e8a6ccbfcf386e19e208db58af32accec5a6228c336198717131ee`  
		Last Modified: Fri, 11 Dec 2020 18:14:49 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; arm variant v7

```console
$ docker pull monica@sha256:d1867c534d9fd61a7e6552291361f170b35515aac24854116c84d237d593e9c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.5 MB (174506120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63450f7b6ce06f404ef2eafca02547b6296586f2c14b55598fdef521feea6027`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:47:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Nov 2020 23:47:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Nov 2020 23:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 23:48:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Nov 2020 23:48:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Nov 2020 23:56:13 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 17 Nov 2020 23:56:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 23:56:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 23:56:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 00:26:34 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 01 Dec 2020 03:08:59 GMT
ENV PHP_VERSION=7.3.25
# Tue, 01 Dec 2020 03:09:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Tue, 01 Dec 2020 03:09:01 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Tue, 01 Dec 2020 03:09:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Dec 2020 03:09:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 03:12:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 03:12:26 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 03:12:31 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 03:12:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 01 Dec 2020 03:12:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 03:12:40 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 03:12:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 03:12:44 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 03:12:45 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 03:12:46 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 05:59:56 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Tue, 01 Dec 2020 06:00:04 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 06:04:26 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 06:04:30 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Tue, 01 Dec 2020 06:04:31 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Tue, 01 Dec 2020 06:04:34 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Tue, 01 Dec 2020 06:04:35 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 06:04:36 GMT
ENV MONICA_VERSION=v2.19.1
# Tue, 01 Dec 2020 06:04:36 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Tue, 01 Dec 2020 06:05:27 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 06:05:33 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Tue, 01 Dec 2020 06:05:36 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 01 Dec 2020 06:05:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531bbb917fccba63f54fa698cfc54068c09767ead93fc6e6644347dd27b257a3`  
		Last Modified: Wed, 18 Nov 2020 01:34:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5e8740a1696bf1e23f4e8db4ddeeefdc469ea5cbc5030b4b966a023c71c05`  
		Last Modified: Wed, 18 Nov 2020 01:34:34 GMT  
		Size: 59.5 MB (59507784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea34a36e19ecf6fc3c24c0040632cc43cf946a21a2874da82d860ca8b00de30`  
		Last Modified: Wed, 18 Nov 2020 01:34:15 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27130a5aa30b0a45f4d7fc9daaf6c7a18f2aecce2c4bc92ac59f6230950da84a`  
		Last Modified: Tue, 01 Dec 2020 04:03:25 GMT  
		Size: 12.5 MB (12456285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e374e015061f7aacb4c5a61f3d5f98d586f1f37612f61e64c6e472d146f944e`  
		Last Modified: Tue, 01 Dec 2020 04:03:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e0e1af81c13d94ad90c95cbb1fbee56247155f00e3702541ae73395c1741f9`  
		Last Modified: Tue, 01 Dec 2020 04:03:33 GMT  
		Size: 26.3 MB (26320027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6737a1b17f64a00810129487d31ca7668b7fdcfa4b74329e3977663e605f09`  
		Last Modified: Tue, 01 Dec 2020 04:03:21 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37c24777bfda6ece1b649ab9b6067b3d59d4c2ea83d6f521dcb3d0fea4eca6b`  
		Last Modified: Tue, 01 Dec 2020 04:03:22 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0430aeec7d22c059617bfbe9b20f69adcab5fecdde933b995abaef2f1f2b32f8`  
		Last Modified: Tue, 01 Dec 2020 04:03:23 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cdb16cd32cad7b38cf1d972761b5968e7c3b7475cfe13ae30e97431e2be5ed`  
		Last Modified: Tue, 01 Dec 2020 04:03:22 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae186f9b5a859a18b93f1896634b7719a0a0b06859d9adcd70ac7c21a5a28169`  
		Last Modified: Tue, 01 Dec 2020 06:10:26 GMT  
		Size: 1.2 MB (1151272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd533e75db6d15f72100c0486dc14645538da99b6343e24436034c5e9b07486`  
		Last Modified: Tue, 01 Dec 2020 06:10:27 GMT  
		Size: 13.7 MB (13749081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab59d093062920fc7fa6bb945505c0c370b2d997c85552d72459724e0382905`  
		Last Modified: Tue, 01 Dec 2020 06:10:23 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c4829564ed1e6677a7a869efb3f6f68768c49cef0ffabd98b9c0c4cb94f289`  
		Last Modified: Tue, 01 Dec 2020 06:10:23 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14a36df82389fdb520afaaab6faf4102fbf5181a4017ab01d6fa0b4c3cd9bb2`  
		Last Modified: Tue, 01 Dec 2020 06:10:46 GMT  
		Size: 38.6 MB (38593263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeb7e39340da8787274c6d9b58be6dde66b6e429194d0f12488a7bce46ba8c3`  
		Last Modified: Tue, 01 Dec 2020 06:10:23 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; arm64 variant v8

```console
$ docker pull monica@sha256:02639156da0fa39ccebcb7f2cf81ae6ca0f814805f9374bbf8157ebca60763d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191516298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1424308aff2ccd91626320f03346254945bf478beccd47046206c736dac4ce2f`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:54:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 02:54:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 02:54:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:54:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 02:54:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 03:04:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 03:04:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:04:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:04:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 03:36:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 01 Dec 2020 03:59:43 GMT
ENV PHP_VERSION=7.3.25
# Tue, 01 Dec 2020 03:59:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Tue, 01 Dec 2020 03:59:45 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Tue, 01 Dec 2020 04:00:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Dec 2020 04:00:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 04:03:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 04:03:11 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 04:03:14 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 04:03:17 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 01 Dec 2020 04:03:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 04:03:18 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 04:03:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 04:03:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 04:03:23 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 04:03:24 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 06:35:48 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Tue, 01 Dec 2020 06:35:56 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 06:39:52 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 06:39:55 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Tue, 01 Dec 2020 06:39:56 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Tue, 01 Dec 2020 06:39:58 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Tue, 01 Dec 2020 06:39:59 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 06:40:00 GMT
ENV MONICA_VERSION=v2.19.1
# Tue, 01 Dec 2020 06:40:00 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Tue, 01 Dec 2020 06:40:37 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 06:40:40 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Tue, 01 Dec 2020 06:40:41 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 01 Dec 2020 06:40:42 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfe6c188ae8daf1a09a047918e301010eaa2f14f98648e742a0beb8cc525ad7`  
		Last Modified: Wed, 18 Nov 2020 04:37:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7496e2962f6d5953bde1d172cf95cf12b1d8a90c07354c68de7ccd67923764`  
		Last Modified: Wed, 18 Nov 2020 04:37:40 GMT  
		Size: 70.3 MB (70337639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0299a101fd6922debd223a74c36a8a9c1d2503a553b2aadc7bb529d39bcdfe95`  
		Last Modified: Wed, 18 Nov 2020 04:37:21 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c9bea670af560c35cd01cc41038650f72ae1f0b3a0d18a65166b662a0f0b78`  
		Last Modified: Tue, 01 Dec 2020 04:56:36 GMT  
		Size: 12.5 MB (12457143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78272e8ed25451b252d22cfd79b21ca7d866378e8f9c4e3122840baf88546cfa`  
		Last Modified: Tue, 01 Dec 2020 04:56:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46a26d5677a160d0f2e29cdb396cd42cb4e1bdbe885cda03df69322331b1a0b`  
		Last Modified: Tue, 01 Dec 2020 04:56:39 GMT  
		Size: 28.4 MB (28437479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0785906b486188a8f36865a35b90523e2a6304dbbeefe44c20b4b5f44d0e1ee3`  
		Last Modified: Tue, 01 Dec 2020 04:56:32 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c227d77486841928ad7c316cf7f07816857af93229d19fef6767e0d600e80e44`  
		Last Modified: Tue, 01 Dec 2020 04:56:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd0ae88609ccbd9f6a690054d1d7ae28cea0c6afed649d187977c8113fc06f2`  
		Last Modified: Tue, 01 Dec 2020 04:56:33 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee1ba618e3f02d572b1f22fa46ffeaa07d2c91027ee7ba53fc2de1e9878bac6`  
		Last Modified: Tue, 01 Dec 2020 04:56:32 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb5cb105ee72b090ad3ce776f1f0e2ab6b52bf71cc63a6abfd25dbc93e84ced`  
		Last Modified: Tue, 01 Dec 2020 06:45:36 GMT  
		Size: 1.3 MB (1290165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3069f12c356ee5c29839936904319660b5781c880893b5bbb428f068c3c2647e`  
		Last Modified: Tue, 01 Dec 2020 06:45:35 GMT  
		Size: 14.5 MB (14523279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e9d2569f642dd3d7bde1f592bb1b38f6d371b211f45e0ddf134dd513f8b375`  
		Last Modified: Tue, 01 Dec 2020 06:45:31 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618faeb71c414056c0280c3a367896105cebe8dad982bc317ef16a36ac4698d`  
		Last Modified: Tue, 01 Dec 2020 06:45:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9d17ce35708814e4c833749d8bb9960a77c4f16247c459de2f6103c6328bae`  
		Last Modified: Tue, 01 Dec 2020 06:45:48 GMT  
		Size: 38.6 MB (38593846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee0da14142e40eb7f2c77baa08d62c16fde49020b2922340f0c8b86fb70dfeb`  
		Last Modified: Tue, 01 Dec 2020 06:45:31 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; 386

```console
$ docker pull monica@sha256:07fb69a2a03f33573a435ece91b2da4c9760fbd4d876e4d4eb843357d9a4b399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.2 MB (206201661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:451bb9cb7b7dc5acf07c9b764b8cc45e760c0ae61fea8e27fc775ba7b2bbf687`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 03:24:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 03:24:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 03:25:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 03:25:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 03:25:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 03:44:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 03:44:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:44:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:44:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 04:52:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 01 Dec 2020 05:15:12 GMT
ENV PHP_VERSION=7.3.25
# Tue, 01 Dec 2020 05:15:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Tue, 01 Dec 2020 05:15:12 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Tue, 01 Dec 2020 05:15:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Dec 2020 05:15:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 05:24:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 05:24:13 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 05:24:14 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 05:24:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 01 Dec 2020 05:24:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 05:24:17 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 05:24:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 05:24:19 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 05:24:19 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 05:24:19 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 08:01:01 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Tue, 01 Dec 2020 08:01:07 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 08:03:59 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 08:04:00 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Tue, 01 Dec 2020 08:04:00 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Tue, 01 Dec 2020 08:04:01 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Tue, 01 Dec 2020 08:04:01 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 08:04:01 GMT
ENV MONICA_VERSION=v2.19.1
# Tue, 01 Dec 2020 08:04:01 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Tue, 01 Dec 2020 08:04:28 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 08:04:29 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Tue, 01 Dec 2020 08:04:29 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 01 Dec 2020 08:04:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b286c870dff8cb1929fbcb70282146dec74dfd25503c8ee95518743a76455a37`  
		Last Modified: Wed, 18 Nov 2020 06:40:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16888cf2c682a0bc6383a40a53149f94c86cc5ee6a60875cafa7d9c4fb7a34`  
		Last Modified: Wed, 18 Nov 2020 06:40:53 GMT  
		Size: 81.2 MB (81195906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43330c18aaac349884e28f75883e60a253334146c5305e6dbe41ac0803c67ab`  
		Last Modified: Wed, 18 Nov 2020 06:40:26 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8741888a972251c93881bdabc82aa895d51bae4a700559736558fe50b6507e51`  
		Last Modified: Tue, 01 Dec 2020 07:17:44 GMT  
		Size: 12.5 MB (12457576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf8df77aa0e9968d16fe2d350cca1ff580ef489a844b2f6208f9acb5f53474`  
		Last Modified: Tue, 01 Dec 2020 07:17:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f01145a86c861a75a561d8a72192983aa536c5e6f0ebde956dd097357859c0c`  
		Last Modified: Tue, 01 Dec 2020 07:17:54 GMT  
		Size: 29.3 MB (29309304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3b4f033030242a559ec6ec8607186420e93ec71984b079f8483c736b5012c2`  
		Last Modified: Tue, 01 Dec 2020 07:17:39 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e038297021a42b133a5ea0002a83d43b819f039d129fc98f3ed3cfc8a515c0bc`  
		Last Modified: Tue, 01 Dec 2020 07:17:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114d7b416f0dbde8e22267f41b11c014e8090ec45036bdd9a898ac36e1802ff2`  
		Last Modified: Tue, 01 Dec 2020 07:17:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7c64b899099fb74088a3d197c8be0964f4aaeb182f1f03525734c8e7ee99f`  
		Last Modified: Tue, 01 Dec 2020 07:17:40 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0514a668b82ae599e2bd697f5bfebb1e183da53243804f9918f191ef01a97fa`  
		Last Modified: Tue, 01 Dec 2020 08:08:27 GMT  
		Size: 1.3 MB (1334379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f02567a3ce9e0e29f000446d68a1f37ed56e77e368f3e7b11eea48795dc7ca`  
		Last Modified: Tue, 01 Dec 2020 08:08:30 GMT  
		Size: 15.5 MB (15530315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad48410b874921f66dfd9630263340201af6d92e0fdbbfa346b5999bfde5f89a`  
		Last Modified: Tue, 01 Dec 2020 08:08:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dfd56c0d8ab74470deff996195a0c77ff54e2fe0a7a0c9ab46c3bfc724beba`  
		Last Modified: Tue, 01 Dec 2020 08:08:25 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5225ce139399b6bc0a604ab0e534a379d1e527eb42c8769a49e0e8c8c024f8df`  
		Last Modified: Tue, 01 Dec 2020 08:08:43 GMT  
		Size: 38.6 MB (38593856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ecb81c40a9501fa44a484032698e1970db3431c48ef9a3015b7c6a7cbf1139`  
		Last Modified: Tue, 01 Dec 2020 08:08:25 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; mips64le

```console
$ docker pull monica@sha256:d2a5b464498ad4e142eba6a928c49120832c516bfc9744e1daf2801f9e2ca389
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182369715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70f057432fa73974e803b1b291a8c1592776dc14c4ba4413ca0863ab3697052`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:25:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 04:25:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 04:26:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:26:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 04:26:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 04:52:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 04:52:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 04:52:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 04:52:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 06:31:01 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 11 Dec 2020 06:31:02 GMT
ENV PHP_VERSION=7.3.25
# Fri, 11 Dec 2020 06:31:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Fri, 11 Dec 2020 06:31:02 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Fri, 11 Dec 2020 06:31:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:31:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 06:44:21 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 06:44:23 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 06:44:25 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 11 Dec 2020 06:44:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 06:44:26 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 06:44:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 06:44:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 06:44:28 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 06:44:28 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 20:02:04 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 11 Dec 2020 20:02:16 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:09:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:09:05 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 11 Dec 2020 20:09:06 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 11 Dec 2020 20:09:08 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 11 Dec 2020 20:09:08 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 20:09:08 GMT
ENV MONICA_VERSION=v2.19.1
# Fri, 11 Dec 2020 20:09:09 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Fri, 11 Dec 2020 20:10:22 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:10:25 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Fri, 11 Dec 2020 20:10:25 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 11 Dec 2020 20:10:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b3d5e3fa447bed7791080d575c40219a0b0de0c2e5ead844514214998183e0`  
		Last Modified: Fri, 11 Dec 2020 06:59:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1851d26f0412137a20989be3bda0a0351df126006d6402dc3ded381e8c9869`  
		Last Modified: Fri, 11 Dec 2020 07:00:41 GMT  
		Size: 61.4 MB (61389791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abb65a130446f126e756b4748232dd20e059e4dfb57760a20063aad1e3ce00b`  
		Last Modified: Fri, 11 Dec 2020 06:59:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8b3ea74ba536c1debd0d1bdd9bc60772095bbdf235067b725c7316e7c5ab25`  
		Last Modified: Fri, 11 Dec 2020 07:08:37 GMT  
		Size: 12.5 MB (12455541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5066eb256145fce34c3b5adebf3e5d694e581278cecd846d0780308314405a03`  
		Last Modified: Fri, 11 Dec 2020 07:08:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb5812d2f17804b5e6ba8f6c43b118337ffd6f183ac6d14c3f3a90c24e3ce76`  
		Last Modified: Fri, 11 Dec 2020 07:08:45 GMT  
		Size: 28.1 MB (28117819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824d02d9f231e0d89b1fce29fdd2eed75be3ef64e8ccfdc59d93d9419c5f6425`  
		Last Modified: Fri, 11 Dec 2020 07:08:26 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4878ae5b0a14b8a3ee026082fc0a2579ccbb63f93558271acc79217c7f004ca`  
		Last Modified: Fri, 11 Dec 2020 07:08:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840781dc8bfe429483a28f9abb81df37f46bb42728a86fb1723a47a877918dd`  
		Last Modified: Fri, 11 Dec 2020 07:08:26 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd68e2d1769ece3115803e3880d7dc3b461e32b625321ea8f3b7eca5308e5e87`  
		Last Modified: Fri, 11 Dec 2020 07:08:25 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50f63ed712f16fe9d84bd99cf48fdf8ea3668587a6a9cd166bcac91f9478bb`  
		Last Modified: Fri, 11 Dec 2020 20:12:15 GMT  
		Size: 1.4 MB (1421124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ebb0f8b792e8c31f5674f5781772018c2387857d97f23aa8984f348314117a`  
		Last Modified: Fri, 11 Dec 2020 20:12:21 GMT  
		Size: 14.6 MB (14608067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f750f677da2f3c915f40cbb6977f1d5ec23a3ace90ce3c04e0bd90917f50d126`  
		Last Modified: Fri, 11 Dec 2020 20:12:10 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3de796c83760becfa958caa4caace35c72c9fb5a59482269e36cb5301d51ea0`  
		Last Modified: Fri, 11 Dec 2020 20:12:12 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e47c9ee7f4ca1485b5919097da1ca6b7dcdfeae2227c1f3af5961d08cecbac`  
		Last Modified: Fri, 11 Dec 2020 20:12:56 GMT  
		Size: 38.6 MB (38593355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9729fa48e59d2c9295b17ebf2b545bdd7b783df538cfa5408233b0f85f4397`  
		Last Modified: Fri, 11 Dec 2020 20:12:10 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; ppc64le

```console
$ docker pull monica@sha256:9cb2d805eac5220e5fe2249a2c0dbe2b7a195ca25ca38f3a697206d118b81c37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212161722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd11fd21e98115fc9a6dd0d0f7c173e136a132592f7e91d4f207d9aa252135cf`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 13:25:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 13:26:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 13:29:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 13:29:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 13:29:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 13:49:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 13:49:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 13:49:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 13:49:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 14:54:26 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 01 Dec 2020 04:48:17 GMT
ENV PHP_VERSION=7.3.25
# Tue, 01 Dec 2020 04:48:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Tue, 01 Dec 2020 04:48:52 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Tue, 01 Dec 2020 04:52:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Dec 2020 04:52:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 04:57:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 04:57:41 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 04:57:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 04:58:10 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 01 Dec 2020 04:58:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 04:58:18 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 04:58:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 04:58:33 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 04:58:42 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 04:58:47 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 10:00:47 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Tue, 01 Dec 2020 10:01:12 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 10:13:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 10:13:54 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Tue, 01 Dec 2020 10:13:59 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Tue, 01 Dec 2020 10:14:08 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Tue, 01 Dec 2020 10:14:12 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 10:14:16 GMT
ENV MONICA_VERSION=v2.19.1
# Tue, 01 Dec 2020 10:14:22 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Tue, 01 Dec 2020 10:16:08 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 10:16:20 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Tue, 01 Dec 2020 10:16:26 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 01 Dec 2020 10:16:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7345157b43f0655c8ac09a2a234d8a2f94542bb32ab16cf4880d4b09722e59`  
		Last Modified: Wed, 18 Nov 2020 15:46:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449b8a70df5c7fde5f5f4a781a4c6b695e0a940f7b4e10d3dcd0774e1efcc891`  
		Last Modified: Wed, 18 Nov 2020 15:47:05 GMT  
		Size: 82.3 MB (82259488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5babd79ef916acbafae12a90aa7e8b4ffa775d7104905dca61473f86a20263`  
		Last Modified: Wed, 18 Nov 2020 15:46:32 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb535fe39894cdf2a679347bc0568252c345258e81916846cd8becd2011c04`  
		Last Modified: Tue, 01 Dec 2020 05:54:16 GMT  
		Size: 12.5 MB (12458321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7f6d324fc917e8798f388b8c99d3e815f770265d415d38be9e7392785a952e`  
		Last Modified: Tue, 01 Dec 2020 05:54:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379da4a8c91c36449862161832932fd03a121b39e7f386332e28da6167fec008`  
		Last Modified: Tue, 01 Dec 2020 05:54:18 GMT  
		Size: 30.5 MB (30465416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dcf9753cf8d2362a61e9a546e51a1d41803f4497fd51088cfed0c275d7eb17`  
		Last Modified: Tue, 01 Dec 2020 05:54:10 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e29a923bdd1e4d1634f27748d98d0dcb0ad259468850ba4b89408c474f80af`  
		Last Modified: Tue, 01 Dec 2020 05:54:10 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529226791bf6dcb24623703d3866a795ca419a9d3e989933d7513bd786e56fb`  
		Last Modified: Tue, 01 Dec 2020 05:54:09 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75584b331c6b6e92a80469508d9cbc7392aac30fd527f4cc3896b0083e605a`  
		Last Modified: Tue, 01 Dec 2020 05:54:10 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cc3617e4ad029522e4701520fb1131400269a92b327674d1f02b65574ae576`  
		Last Modified: Tue, 01 Dec 2020 10:23:04 GMT  
		Size: 1.4 MB (1444146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d30c4aa16c97c967573a0a3092aa7b9316c1b27bcd52e8193842fd82cd3f06b`  
		Last Modified: Tue, 01 Dec 2020 10:23:03 GMT  
		Size: 16.4 MB (16392465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b33f9f0f61a843a71d4f93904d7b8024c45eebc4cd6d1754ae141bc17c8f34`  
		Last Modified: Tue, 01 Dec 2020 10:22:59 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15c31c8ffa15a2f823d7f6043ccecd87e3393092ab40282f9780781c8478523`  
		Last Modified: Tue, 01 Dec 2020 10:22:59 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4352cc1ae060101a617beb84da5d272ed4332145ccbca64c988e9d64d008a65b`  
		Last Modified: Tue, 01 Dec 2020 10:23:13 GMT  
		Size: 38.6 MB (38595963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a52e186c5bc8b3bbf086f613e48223d18cc18bb31520b9f9a24a3c169c881f`  
		Last Modified: Tue, 01 Dec 2020 10:22:59 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:fpm` - linux; s390x

```console
$ docker pull monica@sha256:d6be5af460b95fc69964c9fe8749cf020b3fac0da09d321326a83c0dc6c54a90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.4 MB (185353442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b80d61060a8f6365cad734892a708ae00e8c8d0ece2104fbbf12a89ea9daa74a`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 11:11:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 11:11:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 11:12:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 11:12:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 11:12:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 11:21:51 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 11:21:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 11:21:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 11:21:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 12:31:27 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 11 Dec 2020 12:31:28 GMT
ENV PHP_VERSION=7.3.25
# Fri, 11 Dec 2020 12:31:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Fri, 11 Dec 2020 12:31:29 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Fri, 11 Dec 2020 12:31:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 12:31:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 12:36:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 12:36:59 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 12:37:01 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 12:37:03 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 11 Dec 2020 12:37:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 12:37:04 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 12:37:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 12:37:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 12:37:06 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 12:37:07 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 19:04:56 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 11 Dec 2020 19:05:01 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:08:39 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libmagickwand-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:08:42 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 11 Dec 2020 19:08:43 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 11 Dec 2020 19:08:45 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 11 Dec 2020 19:08:45 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 19:08:46 GMT
ENV MONICA_VERSION=v2.19.1
# Fri, 11 Dec 2020 19:08:46 GMT
LABEL org.opencontainers.image.revision=6d809fda1d59048521c6d5c7e8c3306039b18d4c org.opencontainers.image.version=v2.19.1
# Fri, 11 Dec 2020 19:09:33 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -r "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:09:50 GMT
COPY multi:aec98ea2c6fccdbefed9f2908282c495dd184d4d94c7452e4cdb9b0ddeec1338 in /usr/local/bin/ 
# Fri, 11 Dec 2020 19:09:50 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 11 Dec 2020 19:09:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e848b987a55bcc9612a0ff983cfffc62ac173eb600e57e1f26d2f62d666fdf`  
		Last Modified: Fri, 11 Dec 2020 13:46:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aeb6ec9142dee6d014f57c94fb0a215e2d28aa691b8568428e5e462d17ebd92`  
		Last Modified: Fri, 11 Dec 2020 13:46:19 GMT  
		Size: 64.7 MB (64707189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd418c632e5e527db12983ceffec6fb69c3ae70b420bb36ce3f0bc2f72b76bee`  
		Last Modified: Fri, 11 Dec 2020 13:46:08 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870d0da918b3dd3fe6a51bd2af72dea6ca8d0d16ab8917cbbbcc44e79ecffd`  
		Last Modified: Fri, 11 Dec 2020 13:52:15 GMT  
		Size: 12.5 MB (12456644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cac5fddd827587c1f0e5e34e91c56a2b52aea383dce0531826147ed4ed03a`  
		Last Modified: Fri, 11 Dec 2020 13:52:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375a64ad13163aad0c4079806ac1d3be707020691cb854d6bb12d6634118d36`  
		Last Modified: Fri, 11 Dec 2020 13:52:16 GMT  
		Size: 27.9 MB (27905279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93a2922fa097c415045e164025f19ed789c31abf349211eb3a1c58cf3de6f6d`  
		Last Modified: Fri, 11 Dec 2020 13:52:11 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06026616da6faa4798ffacac2743f2ef366ea4dfaa455b82b50ea3d471a2c64c`  
		Last Modified: Fri, 11 Dec 2020 13:52:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5966d0498daefa2b7ab14063d0e371a12a648f9d130f5de4987437c623636c7`  
		Last Modified: Fri, 11 Dec 2020 13:52:11 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5ed5c23991f008f44527a8a4e52563aaeb4429f0ecf266b13503693c9bbd27`  
		Last Modified: Fri, 11 Dec 2020 13:52:11 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551675f0175a13d9a978cdc53adafc3b803f7d06e1c1a8279fbfb0d68adad05`  
		Last Modified: Fri, 11 Dec 2020 19:14:47 GMT  
		Size: 1.3 MB (1292537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368c074a1989962bf9560baf0dbe16bc157f2071fae9b85e7c30f8dc93f1088b`  
		Last Modified: Fri, 11 Dec 2020 19:14:46 GMT  
		Size: 14.7 MB (14670179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddb3fc58aa83c4cd0b8cede58059afae731ed87c85f745a6e4908e67531a976`  
		Last Modified: Fri, 11 Dec 2020 19:14:45 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242dae1b7b8b5559dbd854634e899793264b07ec74c8f08c31c4f7295e43baa5`  
		Last Modified: Fri, 11 Dec 2020 19:14:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b33ee46e7744f3480084b30f1403fd4b28c9d80d23517ac31c04a6f4590cdb`  
		Last Modified: Fri, 11 Dec 2020 19:14:52 GMT  
		Size: 38.6 MB (38593439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fe6310ea08d7a3b19dca9910c4a2186246f1e1052bc07a86f3bfa22576ae22`  
		Last Modified: Fri, 11 Dec 2020 19:14:44 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
