## `phpmyadmin:5-fpm`

```console
$ docker pull phpmyadmin@sha256:b80c7e66942dc3bb3a155f4296787814be730454bb869e7b18b3643fc91ad8e9
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

### `phpmyadmin:5-fpm` - linux; amd64

```console
$ docker pull phpmyadmin@sha256:0325e195a0ec52f43516680b28edb7297417bb73718147d05b352d4be11bf4d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159120622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37197aba9028baffe620dd1af468b664572faf8d10e368b6f2655ba84b21982`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 09:14:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 09:14:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 09:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 09:15:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 09:15:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 09:32:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 09:32:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 09:32:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 09:32:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 10:02:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:16:31 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:16:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 20:16:34 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 20:16:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 20:16:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:25:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 20:25:22 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:25:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 20:25:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 20:25:24 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 20:25:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 20:25:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 20:25:25 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 20:25:26 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 04:53:26 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 04:53:27 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 06 Nov 2020 22:21:12 GMT
ENV VERSION=5.0.4
# Fri, 06 Nov 2020 22:21:12 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 06 Nov 2020 22:21:13 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 06 Nov 2020 22:21:13 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 06 Nov 2020 22:21:24 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 22:21:25 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 06 Nov 2020 22:21:25 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 06 Nov 2020 22:21:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Nov 2020 22:21:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f7a64e4b25ef4677013dcec51e1af42c22625c752488313e0861b1888c723a`  
		Last Modified: Tue, 13 Oct 2020 12:23:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da391f3e81f0b09c13ea57f5a07f660d6d704d6c2f03d7c0b550ea1cc7acf149`  
		Last Modified: Tue, 13 Oct 2020 12:24:18 GMT  
		Size: 76.7 MB (76652309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8199ae3052e18f15705e0e05b817db237cae5bea84678ae2cbc0e9b88b2a2209`  
		Last Modified: Tue, 13 Oct 2020 12:23:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d216da44d6f4ad787f3b7374b67bd50423e50da346b604795eb5336a9d02cc3`  
		Last Modified: Fri, 06 Nov 2020 01:29:15 GMT  
		Size: 10.6 MB (10633510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a797fd0cedc0e37677ae0b13048107dc61154f43ccd9e9207673b0d7760b09e`  
		Last Modified: Fri, 06 Nov 2020 01:29:12 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5505853120d3e25b6371247511f4f30f90090d08db2493924896ece1dc372cf`  
		Last Modified: Fri, 06 Nov 2020 01:29:22 GMT  
		Size: 28.6 MB (28554265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f3b6b2a793ca880d1f858f30370b168dde990d272da53e95b05ae2b86000d6`  
		Last Modified: Fri, 06 Nov 2020 01:29:13 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c6a04f8b00e5f89fda606c6edbdb5871eabd63ab9512eb52f7c675e32d3b88`  
		Last Modified: Fri, 06 Nov 2020 01:29:12 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9319e9027069548d5e9fc9e75ce3394f105423de221bb2170471e5f0df499d`  
		Last Modified: Fri, 06 Nov 2020 01:29:12 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53dbc037735fbc16b40d0b5fd0b26579c63abcaa1bd5a74f7fd9850d2dcff75c`  
		Last Modified: Fri, 06 Nov 2020 04:55:30 GMT  
		Size: 2.9 MB (2876532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0078a17fc75c3ec86cb72b48577798a43579e04b635a21136e240671f795de`  
		Last Modified: Fri, 06 Nov 2020 04:55:28 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b48f5ad8ba4a60cc78f9db683bf742af1392f1998914166bb5c212151a9ff9e`  
		Last Modified: Fri, 06 Nov 2020 22:22:05 GMT  
		Size: 13.3 MB (13297156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70277281dee08413b14cadd0cfac3ff0317f3ebdc9662ec163be314734cb24fe`  
		Last Modified: Fri, 06 Nov 2020 22:22:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46107d75ec4812374ac0b0aff4f412eb902e0dc7e2960002f4f99b443d68f1b8`  
		Last Modified: Fri, 06 Nov 2020 22:22:02 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; arm variant v5

```console
$ docker pull phpmyadmin@sha256:c673ae37793651d860b5c8473f872d924adbe0de5000e59ead4759bc4b3239d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137411835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf98cfde453b0c35839fc12fb14d378ce3409511b05e4209fd16b961720b4d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:19:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 01:19:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 01:19:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:20:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 01:20:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 01:29:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 01:29:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 01:29:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 01:29:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 01:44:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 18 Nov 2020 01:44:59 GMT
ENV PHP_VERSION=7.4.12
# Wed, 18 Nov 2020 01:45:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Wed, 18 Nov 2020 01:45:03 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Wed, 18 Nov 2020 01:45:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 01:45:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 01:48:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 01:48:57 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 01:48:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 01:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 01:49:01 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 01:49:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 01:49:04 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 01:49:04 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 01:49:05 GMT
CMD ["php-fpm"]
# Wed, 18 Nov 2020 11:59:54 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 11:59:56 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 18 Nov 2020 11:59:57 GMT
ENV VERSION=5.0.4
# Wed, 18 Nov 2020 11:59:57 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Wed, 18 Nov 2020 11:59:58 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Wed, 18 Nov 2020 11:59:59 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 18 Nov 2020 12:00:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:00:43 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Wed, 18 Nov 2020 12:00:47 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Wed, 18 Nov 2020 12:00:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 12:00:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776dc65fe485f35eae3d56b942f6eb7b03274125af3dd701b3e7685fc1ce76f`  
		Last Modified: Wed, 18 Nov 2020 03:06:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ffe63163e891daf3bc86acbec5efbf3e6b2a3a86ad699750513ea1dbc0a2a2`  
		Last Modified: Wed, 18 Nov 2020 03:06:23 GMT  
		Size: 58.8 MB (58801122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6a98a4af0ce3ef1a753a35db68ef19dcfc7485e5c4230928dfd98773bb28c1`  
		Last Modified: Wed, 18 Nov 2020 03:06:03 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0197a5ad789ea63bc1023a1f5821134795ec42b0b7692322e29e3bd10faa1a9`  
		Last Modified: Wed, 18 Nov 2020 03:08:43 GMT  
		Size: 10.6 MB (10631755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a9f79e1400362031f518ac14d99d361a395b25f2fe41ea0163673aa41de75c`  
		Last Modified: Wed, 18 Nov 2020 03:08:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807dbbbd3d2ce116a1df05c1e09f8734341596f29a46d783cdad8f59964fce82`  
		Last Modified: Wed, 18 Nov 2020 03:08:49 GMT  
		Size: 27.2 MB (27171381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562f948238c4c6ca170ec28b10224876bf750ac22b578152503c615fca412e60`  
		Last Modified: Wed, 18 Nov 2020 03:08:41 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974848aacfad37b28f8eeb9c6e9f84f54c6614281e2b9eb65e774c1b0da604e`  
		Last Modified: Wed, 18 Nov 2020 03:08:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f58d0e7094bbe808556985e0cac81eaa86a4b6e9e5325a9568f3b892d1e5353`  
		Last Modified: Wed, 18 Nov 2020 03:08:40 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214901ed23abf7d03e39a5941001dc85db2faae0d9a4388c42bbb07cdcd61181`  
		Last Modified: Wed, 18 Nov 2020 12:01:46 GMT  
		Size: 2.6 MB (2649852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82f442019009b3517af7af560b4da71d72a985115c4e63ab88bd89dbc22bd48`  
		Last Modified: Wed, 18 Nov 2020 12:01:45 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581c88032e6fb7dfbba3492b0bd5bb598bf79cea888d99bc047b489d687f9fa`  
		Last Modified: Wed, 18 Nov 2020 12:01:51 GMT  
		Size: 13.3 MB (13292722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d85740c2339af6c16d61f9583384a80d618130c2b21d67b0870ee39d13aa6db`  
		Last Modified: Wed, 18 Nov 2020 12:01:45 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf35a2cb4c21aece5728a6bed002df86ec47290aec85c4f7bde14ccc99f1296e`  
		Last Modified: Wed, 18 Nov 2020 12:01:44 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; arm variant v7

```console
$ docker pull phpmyadmin@sha256:72095490b02255a1c624a9a5d610b0e915e146946bbedddb44897ab7b93e8a50
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134819155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44786ac99b2ea7b69f25b87aa941757ff114624d3deccbb93487dcb5df8f754`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:11:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 07:11:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 07:12:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:12:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 07:12:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 07:19:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 07:19:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:19:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:19:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 07:34:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 21:24:00 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 21:24:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 20:00:33 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 20:01:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 20:01:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:04:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 20:04:38 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:04:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 20:04:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 20:04:42 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 20:04:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 20:04:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 20:04:47 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 20:04:48 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 01:15:33 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 01:15:38 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 06 Nov 2020 22:59:41 GMT
ENV VERSION=5.0.4
# Fri, 06 Nov 2020 22:59:41 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 06 Nov 2020 22:59:42 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 06 Nov 2020 22:59:43 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 06 Nov 2020 23:00:13 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 23:00:14 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 06 Nov 2020 23:00:15 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 06 Nov 2020 23:00:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Nov 2020 23:00:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538673f8bb90cc5d7b249b519736152fa4893d7c0b109a5a96714189e7f04ee6`  
		Last Modified: Tue, 13 Oct 2020 08:53:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a77ccf6376a1f637d5fab657dbcb232fe8740f76f52bf6a260a50f078b50f6`  
		Last Modified: Tue, 13 Oct 2020 08:53:48 GMT  
		Size: 59.5 MB (59508126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d118c7f7dae8945ea56b7c44bb994ee5d8fc6db8cf6d86d843e10de69a2f74`  
		Last Modified: Tue, 13 Oct 2020 08:53:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41414510dcbb95efba7cf84c46049fc985be60e8b722bcbba469d2a6ca03855`  
		Last Modified: Thu, 05 Nov 2020 22:23:14 GMT  
		Size: 10.6 MB (10631823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a30d95605138a0b098887afcc46d1485467306d57f6d6585804a3ff0147e7`  
		Last Modified: Thu, 05 Nov 2020 22:23:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6245c7a701a57ead98c7d8d8586ac43156915111e6821cf8b219f3f2653cfe5c`  
		Last Modified: Thu, 05 Nov 2020 22:23:19 GMT  
		Size: 26.2 MB (26176911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091367187eac3c58d1e2f9ee9238a1230c4651ededc7027446507c1713bd02ae`  
		Last Modified: Thu, 05 Nov 2020 22:23:11 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acf1f8a1a0a2ee22497b098470701eb6b8419c487ed9b5ca4d0095e3a55edf9`  
		Last Modified: Thu, 05 Nov 2020 22:23:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c377305cd02c8f2f2cb63f906a62a508f04f190bb677bf55672d6503966d693`  
		Last Modified: Thu, 05 Nov 2020 22:23:11 GMT  
		Size: 8.4 KB (8450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de185a8b3751897f614edfdf5f76fd02e4f70637004541b84b4df04ee723480c`  
		Last Modified: Fri, 06 Nov 2020 01:18:47 GMT  
		Size: 2.5 MB (2494390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e857267868b02e2fd856b380aa00f98977fa3174d69d6d700df0647c99828172`  
		Last Modified: Fri, 06 Nov 2020 01:18:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da02b3014efbbe7cb7b25ff6ab53f3e2417a60209d0d49e6d5448ecec019b6d4`  
		Last Modified: Fri, 06 Nov 2020 23:01:26 GMT  
		Size: 13.3 MB (13293364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa07aa88044f53bf4e80d89e2901bac9b468f67c980b1669a34479a2b9b3a8a3`  
		Last Modified: Fri, 06 Nov 2020 23:01:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c5e28db9e5f4f30ee1fcaf21acf8fa3e44ed67cf8f4891a3725db925cef31c`  
		Last Modified: Fri, 06 Nov 2020 23:01:21 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; arm64 variant v8

```console
$ docker pull phpmyadmin@sha256:a0734e21847befcd8231bb3abb09f021336da709307846867e5c332638a0b7ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151253421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8fe4cae5588a17e15eecf47b339d7e3f1d22cf13481a4a9948a9242ad9e237`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:30:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 08:30:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 08:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:31:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 08:31:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 08:40:26 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 08:40:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 08:40:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 08:40:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 08:58:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:15:35 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:15:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 19:42:05 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 19:42:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 19:42:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:46:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 19:46:08 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:46:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 19:46:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 19:46:16 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 19:46:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 19:46:21 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 19:46:24 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 19:46:26 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 01:28:34 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 01:28:37 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 06 Nov 2020 23:34:28 GMT
ENV VERSION=5.0.4
# Fri, 06 Nov 2020 23:34:28 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 06 Nov 2020 23:34:29 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 06 Nov 2020 23:34:29 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 06 Nov 2020 23:34:53 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 23:34:54 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 06 Nov 2020 23:34:55 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 06 Nov 2020 23:34:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Nov 2020 23:34:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741eb3f70883555af2816289952b20d3b888dbd646902239d6a4c05a1f56232f`  
		Last Modified: Tue, 13 Oct 2020 10:20:42 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4d4fad1085cd2ca40af4c6202bff16df5a2c09f6e71ae6f410bbf71cdd0a5`  
		Last Modified: Tue, 13 Oct 2020 10:21:04 GMT  
		Size: 70.3 MB (70337534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0022620cb4854b0a96ffdc6a595dd2b1f49e5137ad2c3955a6570b2ff99b96f5`  
		Last Modified: Tue, 13 Oct 2020 10:20:41 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c2a2761bf612efce3709d88b1281473617fb2e6a66ea05a3509d6af46ffcf3`  
		Last Modified: Thu, 05 Nov 2020 21:50:11 GMT  
		Size: 10.6 MB (10632499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16815d6cbe4188d8ccd03abd43ebc563109c2e8249b0982447cae580639bdb4`  
		Last Modified: Thu, 05 Nov 2020 21:50:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd2714de2a359fb28c581b80fd14cbc8d4b34635cbd39d110e4bcfc1ade34cf`  
		Last Modified: Thu, 05 Nov 2020 21:50:15 GMT  
		Size: 28.3 MB (28313024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7e7546198147644241c71209f008fa9955530009dcda7fbe80a43647409e4`  
		Last Modified: Thu, 05 Nov 2020 21:50:09 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd3bda5e7c9bf29077e08fb55890c583949ed1dc9401a41e708085ea924ba4a`  
		Last Modified: Thu, 05 Nov 2020 21:50:08 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510414829acef7caa013cddb6e1d26cfca197418b06fb2eb81c60108bc967f70`  
		Last Modified: Thu, 05 Nov 2020 21:50:08 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc1ee3d2358ea76cf99e27552de39d93a1957cd66cc0dbf42b05a287107c082`  
		Last Modified: Fri, 06 Nov 2020 01:31:43 GMT  
		Size: 2.8 MB (2811205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4981c97188180dc9e5df62707f7fc4314b70c88a0407bfec2e8ea13cdb8c1c`  
		Last Modified: Fri, 06 Nov 2020 01:31:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d47847984ceaf07f7ed9e9760f2358c4cc953142df94d0d4fe00bf7b0d6f35b`  
		Last Modified: Fri, 06 Nov 2020 23:35:57 GMT  
		Size: 13.3 MB (13295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8ce1db4ef655e908bf35449ffa9ab0b69231e0a9b67c661f67b5647d57e493`  
		Last Modified: Fri, 06 Nov 2020 23:35:52 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655a0c1ca46c76f4b9d6b89fe9ce6bed78a02f05abc29852844b83c2aed4107e`  
		Last Modified: Fri, 06 Nov 2020 23:35:52 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; 386

```console
$ docker pull phpmyadmin@sha256:70eb550caa9cbf485bc7c354a1e55a562d8ebb9bba52d71bd5d16f52847f06b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.0 MB (165018878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2463c525b0f84aa2b53cc49329b0468dc78c693ca360a3ae1f4908a36bf3f05`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:47:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 07:47:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 07:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:47:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 07:47:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 08:22:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:51:00 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:51:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 20:51:05 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 20:51:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 20:51:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 21:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 21:00:07 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 21:00:08 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 21:00:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 21:00:09 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 21:00:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 21:00:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 21:00:10 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 21:00:10 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 05:04:59 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 05:05:00 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 06 Nov 2020 22:39:55 GMT
ENV VERSION=5.0.4
# Fri, 06 Nov 2020 22:39:55 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 06 Nov 2020 22:39:55 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 06 Nov 2020 22:39:56 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 06 Nov 2020 22:40:11 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 22:40:11 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 06 Nov 2020 22:40:11 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 06 Nov 2020 22:40:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Nov 2020 22:40:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c025d092578150306e736243d79877f016e308c259079f3050040068805ec2`  
		Last Modified: Tue, 13 Oct 2020 10:37:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af847e2bbb92ee205de4388ed3631534643337cd4c5487a4c0158092a75fba69`  
		Last Modified: Tue, 13 Oct 2020 10:38:32 GMT  
		Size: 81.2 MB (81196048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d53973650961722caa47d6c81a99b797341d74d6986661b78f0f5979b6197`  
		Last Modified: Tue, 13 Oct 2020 10:37:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c069eee61aa67620f123f95ed340377f6af78a3d3a669a69bf0b6dd2f6d8a90`  
		Last Modified: Fri, 06 Nov 2020 02:13:10 GMT  
		Size: 10.6 MB (10632873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067631bb003a4afe44c4c8154dddbe970b03db6aea63dbec841be871fd7b83ad`  
		Last Modified: Fri, 06 Nov 2020 02:13:06 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8731cbe8d8a01a6d0c4fd072966d70b61696a7c169d45749ef73c8447a0038`  
		Last Modified: Fri, 06 Nov 2020 02:13:15 GMT  
		Size: 29.1 MB (29131397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbb8c7a6938993fcffe1a569c93304de6f8b657118add06667fdb616f66284b`  
		Last Modified: Fri, 06 Nov 2020 02:13:07 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf092d0fb70757c04a6ce532c788f53361e66338b7e4e927a1050f17a076e44`  
		Last Modified: Fri, 06 Nov 2020 02:13:06 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d22775e092d33fd9fa4ee62f35c0ae0c6de3848d7f185454cb65b1007915dd`  
		Last Modified: Fri, 06 Nov 2020 02:13:07 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe1edc568a4deab22e7e688461768f39d174deaac17e21f69702199e4b1b94`  
		Last Modified: Fri, 06 Nov 2020 05:07:01 GMT  
		Size: 3.0 MB (2998085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc2059b7cb7d1e60c7729714ab430bc238f2fbd502e526b827ff511b9f6133b`  
		Last Modified: Fri, 06 Nov 2020 05:07:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3a595888a0b88d10d3c143e1f81781d99b04daac80d122029ebd925d3b1188`  
		Last Modified: Fri, 06 Nov 2020 22:41:02 GMT  
		Size: 13.3 MB (13295616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9740c980754d45d7bce62c6d6b3718b55c897d5b4fcd5d605fa46d4373abfed9`  
		Last Modified: Fri, 06 Nov 2020 22:40:57 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39f36f2a459b8057c61fff9d1f95ce63b7e51b3967a0f5a9c04b44e77f7872d`  
		Last Modified: Fri, 06 Nov 2020 22:40:56 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; mips64le

```console
$ docker pull phpmyadmin@sha256:4666d52ae0ca9fbdbc5c4bde961df8553d6579201350ff5953879b05ad9659db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141807346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:500b0feb61f662066c8343f22395d8f2024d6e616dc64c873c8f64a772428848`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:15:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 07:15:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 07:16:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:16:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 07:16:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 07:42:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 07:42:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 07:42:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 07:42:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 08:31:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 18 Nov 2020 08:31:04 GMT
ENV PHP_VERSION=7.4.12
# Wed, 18 Nov 2020 08:31:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Wed, 18 Nov 2020 08:31:05 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Wed, 18 Nov 2020 08:31:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 08:31:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 08:44:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 08:44:04 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 08:44:06 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 08:44:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 08:44:06 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 08:44:08 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 08:44:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 08:44:09 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 08:44:09 GMT
CMD ["php-fpm"]
# Wed, 18 Nov 2020 14:45:50 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 14:45:52 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 18 Nov 2020 14:45:52 GMT
ENV VERSION=5.0.4
# Wed, 18 Nov 2020 14:45:53 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Wed, 18 Nov 2020 14:45:53 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Wed, 18 Nov 2020 14:45:53 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 18 Nov 2020 14:46:28 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 14:46:29 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Wed, 18 Nov 2020 14:46:29 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Wed, 18 Nov 2020 14:46:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 14:46:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8a605388fd73fc0a30049e1816ed2373347cbf1ca6d77be293fa8862d2b3f5`  
		Last Modified: Wed, 18 Nov 2020 09:48:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4e3df7e0f49e71f681e38aaf78e338a20a808236b450b995a1cdc14a23984e`  
		Last Modified: Wed, 18 Nov 2020 09:49:47 GMT  
		Size: 61.4 MB (61388764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6316538eedb24d61e8570cb82fdf616a81fec0940e867631bf9386a7492f304b`  
		Last Modified: Wed, 18 Nov 2020 09:48:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c2b7cfc44f0fa63edd7a86aaf8188497e751bc2d553e814582a75eaec84859`  
		Last Modified: Wed, 18 Nov 2020 09:54:52 GMT  
		Size: 10.6 MB (10631072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4029a2a248b80307bef141a48b9f82ea197bc0fed4cb5e6bf77fbc090ccbafee`  
		Last Modified: Wed, 18 Nov 2020 09:54:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e888238c9ffb6a8bb227c9acf35a3478c428cf6628203d4b400ecb6d896cf7a6`  
		Last Modified: Wed, 18 Nov 2020 09:55:06 GMT  
		Size: 27.9 MB (27920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd12d874f11df99223f767cf2069a65645acc009b22caf26cf74cb5f44c7f7`  
		Last Modified: Wed, 18 Nov 2020 09:54:46 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e07576a31fb468f300017262104655579388a0e21810c5061d86ba2493c0c4`  
		Last Modified: Wed, 18 Nov 2020 09:54:45 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60734b451cd717c7d69ccc295f87437dabe5451ebfce2eb0361c88fd5a9629c3`  
		Last Modified: Wed, 18 Nov 2020 09:54:46 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52829406e50b8f8e026c7323d8c2b12cb15cf7426f6f49bf3f86295e3cb73db`  
		Last Modified: Wed, 18 Nov 2020 14:47:53 GMT  
		Size: 2.8 MB (2785696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c10f9e802a20da1357c0c71139b7db6a98fdc69bad1263e121b0d5da4a80b71`  
		Last Modified: Wed, 18 Nov 2020 14:47:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181ff57968ea04c4ae761edc06f95a3107c7624e01398666b582d8f05e6fa5ce`  
		Last Modified: Wed, 18 Nov 2020 14:48:02 GMT  
		Size: 13.3 MB (13289335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af029bef570677a6dc99c5eeecf60dbffa98ab98f055b0215454d61075d9c87`  
		Last Modified: Wed, 18 Nov 2020 14:47:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3f466424a5015f10926b6b723266d914882edce348cb71ce7fda724ecad3f7`  
		Last Modified: Wed, 18 Nov 2020 14:47:51 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; ppc64le

```console
$ docker pull phpmyadmin@sha256:be5588e7301d77271dd7bf3f07199b1491d5d8e0398a042e3e7d27f42475be35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170084355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba667c4076a1c0340fdf8050d3132ad6a82df4b7deadaeffaea8f3a50330a9d8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:05:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 05:05:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 05:09:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:09:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 05:10:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 05:34:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 05:34:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 05:34:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 05:34:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 06:09:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:41:10 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:41:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 20:45:09 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 20:46:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 20:46:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:50:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 20:50:30 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:50:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 20:50:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 20:50:41 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 20:50:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 20:50:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 20:50:58 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 20:51:01 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 12:20:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 12:20:52 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 06 Nov 2020 23:07:37 GMT
ENV VERSION=5.0.4
# Fri, 06 Nov 2020 23:07:51 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 06 Nov 2020 23:08:02 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 06 Nov 2020 23:08:18 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 06 Nov 2020 23:10:31 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 23:10:39 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 06 Nov 2020 23:10:43 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 06 Nov 2020 23:10:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Nov 2020 23:11:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42e2076538f751963cb6e33d3856a73702f7a90884d34899a5607f79295953e`  
		Last Modified: Tue, 13 Oct 2020 08:17:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e35db0798161ec90aa3e1ad4e128c76fd8dd6eec12cc8b74a4398c1ccd28d92`  
		Last Modified: Tue, 13 Oct 2020 08:18:45 GMT  
		Size: 82.3 MB (82260770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ef3cfefbb151da81c6755b35db85b35469d9f798d1caf63c5dac58e964f7d`  
		Last Modified: Tue, 13 Oct 2020 08:17:27 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9e6f2801c3b9c66cafefa34179860c8a1dd7a9357b21c96b4a6196c1e72013`  
		Last Modified: Thu, 05 Nov 2020 23:39:16 GMT  
		Size: 10.6 MB (10633569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b2d5de11bd95f461dd37cb4a23a178f62268f5ca2da7f755bc8a2884188fd5`  
		Last Modified: Thu, 05 Nov 2020 23:39:10 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576c460846891d144c3067a81481d59f58d4a24540327e0184af8eaf6cc0cda`  
		Last Modified: Thu, 05 Nov 2020 23:39:18 GMT  
		Size: 30.2 MB (30235710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3a10d19236d33e856eaa6b435d3cce6445815ee6af63bb52ad4580b6013fc0`  
		Last Modified: Thu, 05 Nov 2020 23:39:10 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c728617a975a8c48db77e3567ef35bdfada274f7d21a63e23b0ac01057505`  
		Last Modified: Thu, 05 Nov 2020 23:39:10 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba7e16544b3db4f81f97687066ae310cff4acbdca60a86bbf55c0dedc4e4efe`  
		Last Modified: Thu, 05 Nov 2020 23:39:10 GMT  
		Size: 8.5 KB (8452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c63ca9aa4ac6e7a725488835416acf793eb21821c0b39208960e797b66707`  
		Last Modified: Fri, 06 Nov 2020 12:26:24 GMT  
		Size: 3.1 MB (3123127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63361c6f070578856e444091ead829d6eaadcccc4b95e2905b145276d37c1df`  
		Last Modified: Fri, 06 Nov 2020 12:26:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1423d7e89d79969d01fabbb56b8f513ffd4d002bb26f0752ae6c2a94a7ef0c3c`  
		Last Modified: Fri, 06 Nov 2020 23:14:06 GMT  
		Size: 13.3 MB (13298611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51435b29aa67d7a08a12c89619c4d44c83b50dd8a59cd197fdf7344765fc69d0`  
		Last Modified: Fri, 06 Nov 2020 23:14:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253327c1f85820d4c8f43d7db54d53edddac331f304dd876e6318cb6ae31adf4`  
		Last Modified: Fri, 06 Nov 2020 23:14:01 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; s390x

```console
$ docker pull phpmyadmin@sha256:b1e46efe173cbd08b48d14a0255ff62a98939bdc27c95ffe516bc81985cb48ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144828508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66837ba9e5a228ae8d29d3a8e086924ff37d6374cefb59e2e750deb1b938c193`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:22:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 04:22:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 04:22:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 04:22:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 04:22:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 04:28:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 04:28:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:28:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:28:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 04:40:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:13:38 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:13:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 19:39:12 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 19:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 19:39:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:42:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 19:42:46 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:42:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 19:42:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 19:42:48 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 19:42:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 19:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 19:42:50 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 19:42:51 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 00:23:54 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 00:23:56 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 06 Nov 2020 22:42:15 GMT
ENV VERSION=5.0.4
# Fri, 06 Nov 2020 22:42:15 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 06 Nov 2020 22:42:16 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 06 Nov 2020 22:42:16 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 06 Nov 2020 22:42:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 22:42:42 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 06 Nov 2020 22:42:42 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 06 Nov 2020 22:42:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 06 Nov 2020 22:42:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f6fc7eb84774f67a6b6ce7d5bf7074b8b95c83b5abf565c1d5a4ec4a5361b4`  
		Last Modified: Tue, 13 Oct 2020 05:18:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b30e590e0bd29e46f97b1969d6dbc69a84d0546f4e166b9660a0008644c10fe`  
		Last Modified: Tue, 13 Oct 2020 05:18:31 GMT  
		Size: 64.7 MB (64706329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1e2e2347594249a01918a7569ae483d0cf75be8535daf2e2754985b59505e4`  
		Last Modified: Tue, 13 Oct 2020 05:18:21 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9b3f7dae6ddca01dd4576fb0142580183ea52bca0fcd865a18fa40edf924e0`  
		Last Modified: Thu, 05 Nov 2020 21:50:24 GMT  
		Size: 10.6 MB (10631998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602863b04a7a41bcc742a08d56ae69c1961dfdca3f0e71bec3ff2f8d9516488f`  
		Last Modified: Thu, 05 Nov 2020 21:50:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158719c9e11656e63dd65c166bf4c68b670b7141f5e81b2f5b4ac0788b8ca9ca`  
		Last Modified: Thu, 05 Nov 2020 21:50:26 GMT  
		Size: 27.7 MB (27662632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a91d9b85f42babcc652471868b2c8816de30430bf11043d61d244c94e4b9e64`  
		Last Modified: Thu, 05 Nov 2020 21:50:21 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4e96ed0c8a734a6cc63f6c5017a95f8ae7ecc601d316c920bb45b24f54eb06`  
		Last Modified: Thu, 05 Nov 2020 21:50:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6a3d881839a9e39860abf5b6b1f1e7aee3da1e5ebe476b5801570b50ed17ac`  
		Last Modified: Thu, 05 Nov 2020 21:50:21 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17fb9a78ae7feaf31c2174d97be87c9793535e1ae77f09159b462eb79589588`  
		Last Modified: Fri, 06 Nov 2020 00:26:19 GMT  
		Size: 2.8 MB (2811690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e13cc729923994ed29502aee3f2a67004b80f027fc09cb925d3a722a3a46128`  
		Last Modified: Fri, 06 Nov 2020 00:26:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794f4181e06730d34e32fb146134920719370cad443882027fde4c3b8c351a53`  
		Last Modified: Fri, 06 Nov 2020 22:43:46 GMT  
		Size: 13.3 MB (13293648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d3a822de11a25115bb98a5dd47fe3c4a23bdbc9981973ec3537f197faa3e25`  
		Last Modified: Fri, 06 Nov 2020 22:43:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837fea1553ce128e79f6ed33e303b37720de185317835bb42c9f65bd8f9898ea`  
		Last Modified: Fri, 06 Nov 2020 22:43:44 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
