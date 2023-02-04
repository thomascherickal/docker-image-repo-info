## `drupal:9-fpm-bullseye`

```console
$ docker pull drupal@sha256:93f5c50ef6379242a9bf6edacbc0366f84a7a21e4be6c298645033c1299b25f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:9-fpm-bullseye` - linux; amd64

```console
$ docker pull drupal@sha256:b3a7d3fa86de4b45fae3d4c79ba52fe3ae3c549f880052a81c8f0c3ee0a1b1de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187004851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e95a873be74125fa58befecbf7c2ac87dfc490055439e030cbe8841b52740fee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:18:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 07:18:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 07:19:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:19:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 07:19:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 07:19:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 07:19:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 07:19:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 07:47:54 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 07:47:54 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 07:47:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 07:47:54 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 07:48:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 07:48:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 07:58:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 07:58:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 07:58:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 07:58:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 07:58:13 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 07:58:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 07:58:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 07:58:13 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 07:58:14 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 22:55:24 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Feb 2023 02:02:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Feb 2023 02:02:06 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Thu, 02 Feb 2023 02:03:42 GMT
ENV DRUPAL_VERSION=9.5.3
# Thu, 02 Feb 2023 02:03:43 GMT
WORKDIR /opt/drupal
# Thu, 02 Feb 2023 02:03:54 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 02 Feb 2023 02:03:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1873be8582646883d25d54eaafb9afa7d778d378e04063e1f616cbdec129b9f4`  
		Last Modified: Wed, 11 Jan 2023 08:44:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6a163d8c1d0c95101cdc4fa31cc6ef5846353b802f3885bc2756afb42d7f8`  
		Last Modified: Wed, 11 Jan 2023 08:44:51 GMT  
		Size: 91.6 MB (91634688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008a172010ba0e6c008f04b19dec142a3b41ef2bcdb59901c88a2a356f61b766`  
		Last Modified: Wed, 11 Jan 2023 08:44:37 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb716163fb0abb23e557d3f38d58da0b45d4ebdc1dc89c7ac2d48f7312ac92d`  
		Last Modified: Wed, 11 Jan 2023 08:48:32 GMT  
		Size: 12.1 MB (12071458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de8adc8e390ea4aad6d9778876db371c83b3a538613ca85e05b21f943eda62`  
		Last Modified: Wed, 11 Jan 2023 08:48:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4052b1622e8e91d7edd6b435440f1bd2af340bf7fc768af274ca1be8acae30`  
		Last Modified: Wed, 11 Jan 2023 08:49:16 GMT  
		Size: 26.2 MB (26234269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47c657dfbc9e79cb7d6b733cd1822a5e5fea74e7422bd0cc106bee6110dbae2`  
		Last Modified: Wed, 11 Jan 2023 08:49:13 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515df302b879e2612773eacf242029ff8ac40c213a7ad45f6bc624b6420ef8bf`  
		Last Modified: Wed, 11 Jan 2023 08:49:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a407f4354f0e3fb393e14a5fb516a4bba934078caa5819edd10d73462833750a`  
		Last Modified: Wed, 11 Jan 2023 08:49:12 GMT  
		Size: 8.7 KB (8733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de05fef8ba646eb428646b2cbefbe571927a7a5d5bba8295c72fbc6ca8cf6c67`  
		Last Modified: Wed, 11 Jan 2023 23:15:49 GMT  
		Size: 2.1 MB (2112039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b7f87269322d74b2236e0126b18fd03886762b3660b36d450fd0ecb09242de`  
		Last Modified: Thu, 02 Feb 2023 02:19:49 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312ce27a0fc7cfd38fd63ae3663d25d9d36b1a6ca6a5508ffd06bc0c8ac8ee83`  
		Last Modified: Thu, 02 Feb 2023 02:19:50 GMT  
		Size: 700.1 KB (700099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1d8bfec47cc196c15d94acd3a964baef16deb79e1c8c16d04c11b6b0251fdc`  
		Last Modified: Thu, 02 Feb 2023 02:22:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61de3f0c5437831c7df030e7250de62070c55c05d495d65331bc90e287dfed0`  
		Last Modified: Thu, 02 Feb 2023 02:22:51 GMT  
		Size: 22.8 MB (22842443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-bullseye` - linux; arm variant v7

```console
$ docker pull drupal@sha256:5e1781f0d14820da0c5e8909414ca4e1656987a3762afa6f87287112957f946b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (156976734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2cefa914d5b7a5b0928243c94b42e0e5d7dae6be11158f20575e8daa6c9219`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 10:36:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 10:36:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 10:36:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 10:36:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 10:36:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 10:36:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 10:36:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 10:36:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 11:03:42 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 11:03:42 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 11:03:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 11:03:42 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 11:03:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 11:03:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 11:14:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 11:14:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 11:14:38 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 11:14:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 11:14:39 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 11:14:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 11:14:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 11:14:39 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 11:14:40 GMT
CMD ["php-fpm"]
# Thu, 12 Jan 2023 03:59:57 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Feb 2023 01:40:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Feb 2023 01:40:51 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Thu, 02 Feb 2023 01:43:19 GMT
ENV DRUPAL_VERSION=9.5.3
# Thu, 02 Feb 2023 01:43:19 GMT
WORKDIR /opt/drupal
# Thu, 02 Feb 2023 01:43:33 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 02 Feb 2023 01:43:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882df4fa64e915a7e386d041f1cda73bb332b579e57d62638e74cbc293a1a162`  
		Last Modified: Wed, 11 Jan 2023 12:19:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e271639575d818d64605a0144af7d5e22a62dc19f38ec2d13aab6713f2a86d`  
		Last Modified: Wed, 11 Jan 2023 12:19:37 GMT  
		Size: 69.3 MB (69321270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60c5e170798d756882d1721e2ee63afb99a31eabe5c6da7c22b3765b21b53a`  
		Last Modified: Wed, 11 Jan 2023 12:19:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5644c8462a2ad51b26107958c60ec341d3f9362ae3052d8511468436f0332f`  
		Last Modified: Wed, 11 Jan 2023 12:25:16 GMT  
		Size: 12.1 MB (12069660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ca62173b79bfbfa0fcea0f1b55b7a1b454791d72eb7a3d40592aaff3cbc023`  
		Last Modified: Wed, 11 Jan 2023 12:25:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f30c07433fc811f96232788dd59699c329c37b3dc80853374d3ba4d51a63e88`  
		Last Modified: Wed, 11 Jan 2023 12:26:22 GMT  
		Size: 24.0 MB (23982057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588eef2b09b67644f82deb988d6bcef3541f9b28d632d809628d5b40ac28fdef`  
		Last Modified: Wed, 11 Jan 2023 12:26:17 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc971eff37033138afff6868d45df7f92d794bd88fa2b489a2a8e47412fede3`  
		Last Modified: Wed, 11 Jan 2023 12:26:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e4df8d193c248af62debf8765410ae7ab8353e133e335e7cd863f935c751a`  
		Last Modified: Wed, 11 Jan 2023 12:26:17 GMT  
		Size: 8.7 KB (8733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af23ad3abf5d5dc519f8ee4b67e6cb7e79e67374f1df2e3a4c03c5f453a775c`  
		Last Modified: Thu, 12 Jan 2023 04:32:12 GMT  
		Size: 1.5 MB (1488422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198fc8b84077030df5bfb5b5c12cda56830ca2cd4395deabd8fafabbf23e555e`  
		Last Modified: Thu, 02 Feb 2023 02:13:07 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed896375ae318165eeee298da438c0343bf74d5a2b395393ceaa58213fb057a`  
		Last Modified: Thu, 02 Feb 2023 02:13:07 GMT  
		Size: 700.1 KB (700097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2849a033a4f16554d1cd92cb642101015aca0b0831be1fd47944c8fa7b5dabae`  
		Last Modified: Thu, 02 Feb 2023 02:17:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a9a50498499ccabda6adbec40890c2fcbb67f4f91ce321ee46a7ed6b4d553d`  
		Last Modified: Thu, 02 Feb 2023 02:17:19 GMT  
		Size: 22.8 MB (22842935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-bullseye` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:b1f47da02b2d5f75abbd59e584ae3405aa4ceac8e5bf7d90a56c3b73f1b11221
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.2 MB (181243380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea8d038310522913c15f60129c477706592311479abf9c14c39cb57bc34c2d4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 08:18:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 08:18:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 08:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 08:18:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 08:18:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 08:18:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 08:18:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 08:18:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 08:43:44 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 08:43:44 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 08:43:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 08:43:44 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 08:43:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 08:43:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:52:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 08:52:46 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:52:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 08:52:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 08:52:47 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 08:52:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 08:52:48 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 08:52:48 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 08:52:48 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 20:26:02 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Feb 2023 00:46:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Feb 2023 00:46:11 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Thu, 02 Feb 2023 00:48:07 GMT
ENV DRUPAL_VERSION=9.5.3
# Thu, 02 Feb 2023 00:48:07 GMT
WORKDIR /opt/drupal
# Thu, 02 Feb 2023 00:48:17 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 02 Feb 2023 00:48:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783d22fac3eac4a07011a625ea45f42515d634508d0c225ac059d5c7735f1446`  
		Last Modified: Wed, 11 Jan 2023 09:28:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aa0709519156981b3de2c39cc2fec319758a1097840b73cd25bf113bd5215a`  
		Last Modified: Wed, 11 Jan 2023 09:29:06 GMT  
		Size: 86.9 MB (86926666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf93b070c8b7a97115750cc9fdd5c981b52c9b188e2ebd105ad95aeec094c5`  
		Last Modified: Wed, 11 Jan 2023 09:28:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57990fa99faae10ba453edf07645dc9defe3a8089fcdf389f2dba1f76a41b061`  
		Last Modified: Wed, 11 Jan 2023 09:32:42 GMT  
		Size: 12.1 MB (12070691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a1b7ed0228b53e4b00a5536a26fcc865b58a97e0b57cf71bed9463315846f3`  
		Last Modified: Wed, 11 Jan 2023 09:32:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cf41e38ee674a495b690299a1e1b166c85fbc5342b248defb974afe7e302ac`  
		Last Modified: Wed, 11 Jan 2023 09:33:26 GMT  
		Size: 26.3 MB (26273585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2ccd1d05f5ea6c36cb3b03f38c9663c4ff26b5b770146965e00673d45fd895`  
		Last Modified: Wed, 11 Jan 2023 09:33:22 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1fd4c8b64b897cdf4395543e9a50d12f479db361edd6c9c6833660bf2a2808`  
		Last Modified: Wed, 11 Jan 2023 09:33:22 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9e7dfbebad7bb65ae3eed0b3150e4ed8b0e9a9a45d3b1906f544838a0663e9`  
		Last Modified: Wed, 11 Jan 2023 09:33:22 GMT  
		Size: 8.7 KB (8729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821bdb0e2afc67669b2707f3389dceac65d92ced47693962256837103de57208`  
		Last Modified: Wed, 11 Jan 2023 20:45:50 GMT  
		Size: 2.4 MB (2371764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185f747cf2f0f693c0abe50bb099f4912e4e30de026ec959899f9809ec01a336`  
		Last Modified: Thu, 02 Feb 2023 01:04:50 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d741a9c16d647e6d88173077415451b9e2c31d9600f46bdd03d1fbb55d3cf9`  
		Last Modified: Thu, 02 Feb 2023 01:04:50 GMT  
		Size: 700.1 KB (700098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35249b1b882906a91739f6ec86a71d76c7dbc552ed9d591f9732bee2ced5338`  
		Last Modified: Thu, 02 Feb 2023 01:07:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff081e41e4cd4417aee38f2b112385698b1e696e616c3ca1420e77e91a3907`  
		Last Modified: Thu, 02 Feb 2023 01:07:47 GMT  
		Size: 22.8 MB (22842881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-bullseye` - linux; 386

```console
$ docker pull drupal@sha256:5b62552f903b1155de35fdd5b312b81f5f38079efd37df4ee90ee200cec0688e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188950937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e66e0dd6a23b1cc7dfc10ea2ce6bb60006ecf4ec216d547fb85e23812543c69`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 03:16:08 GMT
ADD file:68afc7c49a947a9fb253ffeba9950cdc39e241f8a5cf0133043cfc612447f597 in / 
# Wed, 11 Jan 2023 03:16:08 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 09:04:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 09:04:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 09:04:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 09:04:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 09:04:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 09:04:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:04:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:04:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 09:31:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 09:31:33 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 09:31:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 09:31:35 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 09:31:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 09:31:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:40:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 09:40:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:40:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 09:41:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 09:41:01 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 09:41:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 09:41:03 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 09:41:04 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 09:41:05 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 19:34:56 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Feb 2023 00:49:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Feb 2023 00:49:08 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Thu, 02 Feb 2023 00:51:28 GMT
ENV DRUPAL_VERSION=9.5.3
# Thu, 02 Feb 2023 00:51:29 GMT
WORKDIR /opt/drupal
# Thu, 02 Feb 2023 00:51:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 02 Feb 2023 00:51:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:165165b78fad597abd0883f40adcaa0edcfe981a358deea181323680a07b7011`  
		Last Modified: Wed, 11 Jan 2023 03:22:01 GMT  
		Size: 32.4 MB (32375738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a84a4150e372653724ca463ad7086fea342fc6712cc3c99fe069842eb452663`  
		Last Modified: Wed, 11 Jan 2023 10:29:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59f5a3efb63feb7448a39ebe0fa9067e07e2ae3ca03ff866f0a7177cfa8eb82`  
		Last Modified: Wed, 11 Jan 2023 10:29:18 GMT  
		Size: 92.7 MB (92716565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b3b707043ac8815a0b4eda0fff0327772a22183d7ef7ac4b2e0a1cc98b58a`  
		Last Modified: Wed, 11 Jan 2023 10:29:05 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ab9ef68aff635aa6d9ae4a15e1d6d8b59de5f6615fd2e71e1b09f1fb612c53`  
		Last Modified: Wed, 11 Jan 2023 10:33:59 GMT  
		Size: 11.9 MB (11854836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737b55eb746ee144f95d74de3ba0609e21d73294ad9a3c6d7da2412728fa409b`  
		Last Modified: Wed, 11 Jan 2023 10:33:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4cff26b71f434d43489b8c7538f696c2bcffa64940f1b44e1a8be9f60bdd81`  
		Last Modified: Wed, 11 Jan 2023 10:34:53 GMT  
		Size: 26.5 MB (26492772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a702c211fa60313731b616392ada1c5e8cffe174e7da397be732352ecb733`  
		Last Modified: Wed, 11 Jan 2023 10:34:49 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f4eb2ca604554a8eb467255a84006c90895adb15535b7db69a00aee5d1d135`  
		Last Modified: Wed, 11 Jan 2023 10:34:49 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5573c8aeba6c971a0581b4752901ae0b5f9a0e18a2511b7c06aa3d46c8f7570`  
		Last Modified: Wed, 11 Jan 2023 10:34:49 GMT  
		Size: 8.7 KB (8738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4906a2059fc66c607698363a3934294099147c17006e07aaa232ceaae1f2e02e`  
		Last Modified: Wed, 11 Jan 2023 20:02:45 GMT  
		Size: 2.0 MB (1960974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57001520a39d2b79c7d5684031d716f71c657b1344842354b3d6a83a4ae229`  
		Last Modified: Thu, 02 Feb 2023 01:15:58 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e809afeb70f0bd92b4944fb34764acbb0cbb0b3932cdf96915f27009fec2a7b`  
		Last Modified: Thu, 02 Feb 2023 01:15:58 GMT  
		Size: 695.2 KB (695205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75866cd795225cdd2581867c165ff762a6b006ae3488228f4f8effbdceee1d24`  
		Last Modified: Thu, 02 Feb 2023 01:19:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2116332ec90cbe455f2c46ae3dbc923016c35e874505d2ad7cac9a71ee266e`  
		Last Modified: Thu, 02 Feb 2023 01:19:35 GMT  
		Size: 22.8 MB (22842040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-bullseye` - linux; ppc64le

```console
$ docker pull drupal@sha256:6ba481fede8490c879be0501c487a850054e4c20b9fd977f921b2fdb5873c5c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.8 MB (186764253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3126a7997b595d32c52e78ddf4e6e57eca5761386df542350b1f83131a5b776c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:41:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 05:41:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 05:42:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 05:42:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 05:42:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 05:42:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:42:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:42:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 06:00:46 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 06:00:46 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 06:00:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 06:00:47 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 06:01:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 06:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 06:13:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 06:13:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 06:13:38 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 06:13:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 06:13:39 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 06:13:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 06:13:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 06:13:41 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 06:13:41 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 19:11:45 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Feb 2023 00:47:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Feb 2023 00:47:26 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Thu, 02 Feb 2023 00:49:53 GMT
ENV DRUPAL_VERSION=9.5.3
# Thu, 02 Feb 2023 00:49:53 GMT
WORKDIR /opt/drupal
# Thu, 02 Feb 2023 00:50:17 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 02 Feb 2023 00:50:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4379437c86e610929801c4b002ebb0e16e22386c100c3572876389b662ef919`  
		Last Modified: Wed, 11 Jan 2023 06:40:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c872424ad6e42db6d62b5ecf528da108f30b96fd3a50c09dcc034ec3c1046c`  
		Last Modified: Wed, 11 Jan 2023 06:41:01 GMT  
		Size: 86.6 MB (86632852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938343d42556b0999a8c10c21195617ddd37b298b164adc36a426137e969ac19`  
		Last Modified: Wed, 11 Jan 2023 06:40:37 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67539be46154b333d77ba74501d47ce561ce9bf9d208a8c9cea4a0f4c9f5a0e`  
		Last Modified: Wed, 11 Jan 2023 06:44:28 GMT  
		Size: 12.1 MB (12071343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357a75b31e71dae11da4db354dc30ce57de14891cd464472c39c5209f3aeb6a6`  
		Last Modified: Wed, 11 Jan 2023 06:44:26 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f2c3bcd59c3554969a35bdf47ba9eff79bd9663a70aadc15b618b75257c22`  
		Last Modified: Wed, 11 Jan 2023 06:45:34 GMT  
		Size: 27.3 MB (27260453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b26db784804e427f3927fe4eac1dcfa8e87f464343ab26a54274878ef343745`  
		Last Modified: Wed, 11 Jan 2023 06:45:27 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b650f0a79ac95166b388367c17a55321fb62f1911f0a7231208ef5314554e8a1`  
		Last Modified: Wed, 11 Jan 2023 06:45:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246b892f7bf206b4d7815a3ad6cbaa6cca4c53f90951bb74ebba8041bec8b7fe`  
		Last Modified: Wed, 11 Jan 2023 06:45:27 GMT  
		Size: 8.7 KB (8734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db21f6564cad6f49017c904b3fefd97e7a2f64c92111ad688963d316a0e8036`  
		Last Modified: Wed, 11 Jan 2023 19:33:15 GMT  
		Size: 2.0 MB (1974873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b634925a86a39fa500f44f20d92bb1cbe59e5b251ac7d0c4f0046e1a21d061ed`  
		Last Modified: Thu, 02 Feb 2023 01:13:25 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9032aeca388f1df769de6778cd6a44841f93329422a7c08de8512f12d64676f9`  
		Last Modified: Thu, 02 Feb 2023 01:13:25 GMT  
		Size: 700.1 KB (700097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b3e3a598f29223adef4d1c94038cd396b705d368e1a423bf656d78bc87557e`  
		Last Modified: Thu, 02 Feb 2023 01:17:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414545d5e76330af8fe26bfa11648be984107e6aaf5876345d9d28ffddd06a26`  
		Last Modified: Thu, 02 Feb 2023 01:17:56 GMT  
		Size: 22.8 MB (22842976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-bullseye` - linux; s390x

```console
$ docker pull drupal@sha256:ebf2bf1ad814c4d6710eb77e11c9d8e9a0497d0eb099b5764bf414b8e9c5d3e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.4 MB (164374937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e432e4d23d14ad5bc37874520ebbe1834104c1ab0eba3c190424a7d7ef340aab`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 02:22:23 GMT
ADD file:14f332233d8fa1ca519992e52aaf550bcee52d346c375e94ee73d36864933f8e in / 
# Wed, 11 Jan 2023 02:22:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:36:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 05:36:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 05:36:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 05:36:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 05:36:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 05:36:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:36:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:36:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 05:48:50 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 03 Feb 2023 22:49:41 GMT
ENV PHP_VERSION=8.1.15
# Fri, 03 Feb 2023 22:49:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Fri, 03 Feb 2023 22:49:41 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Fri, 03 Feb 2023 22:49:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Feb 2023 22:49:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Feb 2023 22:56:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Feb 2023 22:56:19 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 03 Feb 2023 22:56:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Feb 2023 22:56:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Feb 2023 22:56:19 GMT
WORKDIR /var/www/html
# Fri, 03 Feb 2023 22:56:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 03 Feb 2023 22:56:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Feb 2023 22:56:20 GMT
EXPOSE 9000
# Fri, 03 Feb 2023 22:56:20 GMT
CMD ["php-fpm"]
# Sat, 04 Feb 2023 02:27:59 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 02:28:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Feb 2023 02:28:00 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Sat, 04 Feb 2023 02:30:27 GMT
ENV DRUPAL_VERSION=9.5.3
# Sat, 04 Feb 2023 02:30:27 GMT
WORKDIR /opt/drupal
# Sat, 04 Feb 2023 02:30:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 04 Feb 2023 02:30:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:5895b3b9300287ac4aca79440c1c4979b6d4fad1ceb06fba32443d012c83cc37`  
		Last Modified: Wed, 11 Jan 2023 02:26:52 GMT  
		Size: 29.6 MB (29629731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46739b5e342705d87e956551b94a4293567f93b87294ea6230885a9e858fc4e1`  
		Last Modified: Wed, 11 Jan 2023 06:15:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b7e3dfc171ac8a890c6f6cbae546440e66dfeb4da57ab3dd89beb4a9560257`  
		Last Modified: Wed, 11 Jan 2023 06:16:07 GMT  
		Size: 71.6 MB (71626761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b1de7a4314c02dc967cb9909fd47c236937c2eae2f61f3cff1c938395eedf`  
		Last Modified: Wed, 11 Jan 2023 06:15:57 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24c96536fd4b1119c4d8e067d618fdf44516d40b108ed15d3b0fc7f966f7bd`  
		Last Modified: Fri, 03 Feb 2023 23:23:50 GMT  
		Size: 12.1 MB (12131900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edde2e165b1434002965e104cea5682e100d3d736a2a4bfc3873440e2d17ac76`  
		Last Modified: Fri, 03 Feb 2023 23:23:50 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41ea0dc9df03c696c6d28672314e74b1f2cfaec90fca432d08f423607a2482`  
		Last Modified: Fri, 03 Feb 2023 23:24:29 GMT  
		Size: 25.7 MB (25726044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a948dbd543a3755ade0b388085c39220d28105ce4c9941e720af081df82e010`  
		Last Modified: Fri, 03 Feb 2023 23:24:26 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c50106a55b34822cd97e325fd30dc157085f446dea044794f3a39f8f7238f90`  
		Last Modified: Fri, 03 Feb 2023 23:24:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac2c593402cbb9263bfb436f128c938675d5ceb2e2a9f4abd5e7aeabeb9649`  
		Last Modified: Fri, 03 Feb 2023 23:24:26 GMT  
		Size: 8.8 KB (8845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d384ad1bcf69d1bdec0ca73ce25d1aacd27720f0a308464e4ff736e21011ae62`  
		Last Modified: Sat, 04 Feb 2023 02:42:23 GMT  
		Size: 1.7 MB (1703204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdcc20ff0be271761007f02da3789b98954c74148aaaad63efa41581929d72f`  
		Last Modified: Sat, 04 Feb 2023 02:42:23 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85038a9c754a6221aca714802e394825782c3ca405c08d57d033f835368071d`  
		Last Modified: Sat, 04 Feb 2023 02:42:23 GMT  
		Size: 700.1 KB (700099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c96d6a0e4a6924aaa20f51c4977e57a3068f78589aaff2fb418e7d39c492fc`  
		Last Modified: Sat, 04 Feb 2023 02:44:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cea3a8efdf9c40bf987de7e7dab7cd7216cc2eae1b0100d07ede7283b5248a0`  
		Last Modified: Sat, 04 Feb 2023 02:44:07 GMT  
		Size: 22.8 MB (22844209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
