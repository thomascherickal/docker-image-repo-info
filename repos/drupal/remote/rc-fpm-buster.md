## `drupal:rc-fpm-buster`

```console
$ docker pull drupal@sha256:9a307ac3cdcaf0a0a535cc1662c2683468f88ec88cacd5129fb045107601e63b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:rc-fpm-buster` - linux; amd64

```console
$ docker pull drupal@sha256:0245d247d4df23026916b734139e8e07a10d3246b7602dc7470012217f736842
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (161973505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c31a6b854275a5922f1cb0814c7a877b8122d20ceafff54a373d0c6dfbc0d8ee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:26:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 04:26:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 04:27:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:27:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 04:27:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 04:27:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:27:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:27:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 04:53:52 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 15 Nov 2022 04:53:52 GMT
ENV PHP_VERSION=8.1.12
# Tue, 15 Nov 2022 04:53:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Tue, 15 Nov 2022 04:53:52 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Tue, 15 Nov 2022 04:54:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 04:54:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:03:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 05:03:39 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:03:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 05:03:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 05:03:39 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 05:03:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 05:03:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 05:03:40 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 05:03:40 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 08:15:39 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 08:15:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 08:15:39 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Tue, 15 Nov 2022 08:15:40 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Tue, 15 Nov 2022 08:15:40 GMT
WORKDIR /opt/drupal
# Tue, 15 Nov 2022 08:15:52 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 15 Nov 2022 08:15:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a022f9f4db63bdf619d892ab06b0861dc6b1b17b3a137c35093f0937aa7e57`  
		Last Modified: Tue, 15 Nov 2022 06:24:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff96ba8ea962f6736c4fa62505f2aa4b5405f5388b5424727cd3af64cb7cf44`  
		Last Modified: Tue, 15 Nov 2022 06:25:00 GMT  
		Size: 76.7 MB (76687327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b28c78a7e238dc26ddcd2d9ea3c2512abab7fb02db8f343763046433d33bc9c`  
		Last Modified: Tue, 15 Nov 2022 06:24:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d3e1119cbe635479d4e37c2ab3613f75976d013a699c993dc2dcd620b4c2f9`  
		Last Modified: Tue, 15 Nov 2022 06:28:22 GMT  
		Size: 12.1 MB (12070142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a465790d1e7b1d7b47bdb9ea5fffe6710bdec796cdab4841f1ea99df57854ab`  
		Last Modified: Tue, 15 Nov 2022 06:28:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334da69b573db21d92509f4fe6ae2e1c5b804549320f99403c1c44ad7aaf5e56`  
		Last Modified: Tue, 15 Nov 2022 06:29:10 GMT  
		Size: 25.7 MB (25727084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3cfab4b40cc308e84b56f13900bb9c86db45d7acda4757b1a1844630b6cf07`  
		Last Modified: Tue, 15 Nov 2022 06:29:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe52fa5db082d53417243204ad176d2fff6f6031c42178972b4dee9dfed02a6`  
		Last Modified: Tue, 15 Nov 2022 06:29:06 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae506b83df703ddd73def46cd1688a2c2e17f5be46b610cfd024667d742048a`  
		Last Modified: Tue, 15 Nov 2022 06:29:06 GMT  
		Size: 8.6 KB (8621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdfbbd116b97bfc4143c64348ca6ed2b5b3341e136b3768bc3db939cf6bd010`  
		Last Modified: Tue, 15 Nov 2022 08:37:45 GMT  
		Size: 2.1 MB (2064503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef489bfc9aeab03eea5aa90882acf202898080759e58ec0b5275ab9ee30017`  
		Last Modified: Tue, 15 Nov 2022 08:37:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de476253170c66ac66412c40dda86a98b798e95e0bab7693f7f5e010b49e598a`  
		Last Modified: Tue, 15 Nov 2022 08:37:44 GMT  
		Size: 695.2 KB (695198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e87e4d68d60af7d06bc4e4b22dc4fd5508a68ad01956a04c1cb3f5d37293e8`  
		Last Modified: Tue, 15 Nov 2022 08:37:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b8a52988d465dc871a4cf5c34877fc2b053545fa35436b1f2d10d8012d939b`  
		Last Modified: Tue, 15 Nov 2022 08:37:48 GMT  
		Size: 17.6 MB (17576138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-fpm-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:2ea08bc4ee0757fce2d19268db1f713d9b3382ad45916b1cde133bad6853b89c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137557611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799b6849472b225427185cfe88adef156b73f0482d79d16e91f80f304e7e2737`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:57 GMT
ADD file:02e51e32df426f4ee14093de5240d396191761b03f60af08b7e920c86c3df725 in / 
# Tue, 15 Nov 2022 03:43:57 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:07:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 04:07:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 04:07:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:07:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 04:07:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 04:07:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:07:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:07:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 04:31:59 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 15 Nov 2022 04:31:59 GMT
ENV PHP_VERSION=8.1.12
# Tue, 15 Nov 2022 04:31:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Tue, 15 Nov 2022 04:31:59 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Tue, 15 Nov 2022 04:32:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 04:32:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 04:40:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 04:40:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 04:40:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 04:40:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 04:40:26 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 04:40:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 04:40:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 04:40:26 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 04:40:26 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 07:46:12 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 07:46:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 07:46:13 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Tue, 15 Nov 2022 07:46:13 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Tue, 15 Nov 2022 07:46:13 GMT
WORKDIR /opt/drupal
# Tue, 15 Nov 2022 07:46:29 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 15 Nov 2022 07:46:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:e14edb06ef42285b9a4c82509f85d76caeb037799d6631d8d272f86af363a045`  
		Last Modified: Tue, 15 Nov 2022 03:51:01 GMT  
		Size: 22.7 MB (22748928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a744950c0c95ea35eac5bd289ec7493aa3d866cb171b0b7b2617100323dafddd`  
		Last Modified: Tue, 15 Nov 2022 06:06:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a0c468d8145d2641efffc44b06bbdbbcb730f11fcc94864e28dcc5ab9d69f2`  
		Last Modified: Tue, 15 Nov 2022 06:06:56 GMT  
		Size: 59.5 MB (59542292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cf3287317716a59fab00c89f0f363fdfab61ba1aa6ec645c3ec4b50c904401`  
		Last Modified: Tue, 15 Nov 2022 06:06:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882f6c57d68645c730af7eced3f6284aca6d63d2193673b5e34961ee79ded0ef`  
		Last Modified: Tue, 15 Nov 2022 06:11:21 GMT  
		Size: 12.1 MB (12068118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d43bb743efcccd0f75c88c3acc49e79acbdd2a85d58ffed25b92a824ece5db0`  
		Last Modified: Tue, 15 Nov 2022 06:11:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160e08832ad59ea6707c35fc9356995faba6f2a548e706dd5bdd0c82cc280b86`  
		Last Modified: Tue, 15 Nov 2022 06:12:22 GMT  
		Size: 23.5 MB (23457769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3805f2c7e1bc169fc3c8877ec85ba6fd69b3b85cdd588caa388d35eb627034b`  
		Last Modified: Tue, 15 Nov 2022 06:12:17 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5337884cf28e830c121776353840abe56de39c24bf4ba90b1b0a5baa71aca1`  
		Last Modified: Tue, 15 Nov 2022 06:12:17 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63163d31f30bef3be76042ece3676748708ef3d5fcd4f26312db57a5dd649c98`  
		Last Modified: Tue, 15 Nov 2022 06:12:17 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fea945072e027adb302d903efb7331b4b7f3de7b8463de45f201513e25f113c`  
		Last Modified: Tue, 15 Nov 2022 08:27:03 GMT  
		Size: 1.5 MB (1456697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f833f83651158c446b0ba0620e02529c4c7297c9207242da054b6a445dfc535`  
		Last Modified: Tue, 15 Nov 2022 08:27:03 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4afadedff07db2e00eee3e62aa1d3500af2e2382bea53d228476141df37a72`  
		Last Modified: Tue, 15 Nov 2022 08:27:03 GMT  
		Size: 695.2 KB (695192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2dd354add703932dba99ab97217d024d7739ac563d36161e8dacd0c3e5b04a0`  
		Last Modified: Tue, 15 Nov 2022 08:27:03 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f7462005b81842242f69c0cac035811e85ef966ebf93e8c4b3c81ade6bf92b`  
		Last Modified: Tue, 15 Nov 2022 08:27:09 GMT  
		Size: 17.6 MB (17575909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-fpm-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:7ab5a1278f7e37bf5e564f7e36ffe98116aac3bcbce25e5898bea987ae56072c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154736180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d8c3f3d06243ffd18bb6bbcd00e7edf5d16b1abe25d51d8215179ebc114209`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 02:10:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 02:10:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 02:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 02:11:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:35:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 15 Nov 2022 02:35:14 GMT
ENV PHP_VERSION=8.1.12
# Tue, 15 Nov 2022 02:35:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Tue, 15 Nov 2022 02:35:15 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Tue, 15 Nov 2022 02:35:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 02:35:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 02:44:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 02:44:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 02:44:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 02:44:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 02:44:13 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 02:44:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 02:44:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 02:44:13 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 02:44:13 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 16:02:43 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 16:02:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 16:02:43 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Tue, 15 Nov 2022 16:02:43 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Tue, 15 Nov 2022 16:02:43 GMT
WORKDIR /opt/drupal
# Tue, 15 Nov 2022 16:03:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 15 Nov 2022 16:03:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a519f5af3edd9577a7d7eecaf5bb04c787a7af6c91565ef581b3c81dffe93b8d`  
		Last Modified: Tue, 15 Nov 2022 03:59:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd12efc1398d9588db8c0fe6a81579bd5cf22ddeda1ee4ed50728cb8927b993`  
		Last Modified: Tue, 15 Nov 2022 03:59:23 GMT  
		Size: 70.4 MB (70363086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a68f17ee8b59b47c2af378bcbc598995c02bb47e3ee4d56eb01cf3a51bdb9`  
		Last Modified: Tue, 15 Nov 2022 03:59:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6657d6b00d7a29608046e43c0482d7ee21d49a337855cd2a401bfb6a157508d0`  
		Last Modified: Tue, 15 Nov 2022 04:02:23 GMT  
		Size: 12.1 MB (12068843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54532370cc168a5ad780096ba13d638db85a56402056b0a5f09442c0627bd1c`  
		Last Modified: Tue, 15 Nov 2022 04:02:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac316d4eb5888b912c58b4d1c000ca88e348bc28a0ccf2592a904e8e67af7129`  
		Last Modified: Tue, 15 Nov 2022 04:03:09 GMT  
		Size: 25.8 MB (25772740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b15ab5052991a0d3d28ea659fb73557c3cb94231c276211b46dc80c19bb2024`  
		Last Modified: Tue, 15 Nov 2022 04:03:05 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334b87a74b620a0d817bb5ed151dfe76cb2150876e93ccb9cf9572a96adce077`  
		Last Modified: Tue, 15 Nov 2022 04:03:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a743cb06bf94f619e77bb6b008717bd8b9c92530fc7fb7cede7616f57eda537`  
		Last Modified: Tue, 15 Nov 2022 04:03:05 GMT  
		Size: 8.6 KB (8622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cc0732dacf7ab5c43d1aa364e445795cfca86d93829071e9c36d6dddf35f`  
		Last Modified: Tue, 15 Nov 2022 16:25:47 GMT  
		Size: 2.3 MB (2332445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b68afd6373677e938a96ff768d957c4c683f34ebab3427c02e20e691ad4f28`  
		Last Modified: Tue, 15 Nov 2022 16:25:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4730ae6445164698b6935a9b21de6b5dd4795249fd5c58e61cf009d6517178a0`  
		Last Modified: Tue, 15 Nov 2022 16:25:47 GMT  
		Size: 695.2 KB (695193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3af0879f62ec33733053e2674c859c82841c40903f414a6438c23789d2277`  
		Last Modified: Tue, 15 Nov 2022 16:25:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127edcce7984e315661554b6d1413e65bf076854910860725e33430bcd6675d`  
		Last Modified: Tue, 15 Nov 2022 16:25:50 GMT  
		Size: 17.6 MB (17576164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-fpm-buster` - linux; 386

```console
$ docker pull drupal@sha256:c4ad61957de406114937ec81f107317096487bfcd0e7756edb698f676caa8520
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.1 MB (167077727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d3005c51a0c9081605dc1b3c93d8191b5c24ad39477a0d3e4a3c50a6f837439`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:02 GMT
ADD file:49981fa4bc36bce6e4fdd74b2c4429cc4faef5498c3d8fb20fb98b426bbf8c4d in / 
# Tue, 25 Oct 2022 02:23:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 25 Oct 2022 07:56:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 25 Oct 2022 07:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 25 Oct 2022 07:56:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 25 Oct 2022 07:56:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 25 Oct 2022 07:56:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 25 Oct 2022 07:56:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 25 Oct 2022 08:22:28 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 28 Oct 2022 19:07:12 GMT
ENV PHP_VERSION=8.1.12
# Fri, 28 Oct 2022 19:07:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Fri, 28 Oct 2022 19:07:14 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Fri, 28 Oct 2022 19:07:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Oct 2022 19:07:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Oct 2022 19:16:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Oct 2022 19:16:17 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Oct 2022 19:16:17 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Oct 2022 19:16:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Oct 2022 19:16:19 GMT
WORKDIR /var/www/html
# Fri, 28 Oct 2022 19:16:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 28 Oct 2022 19:16:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Oct 2022 19:16:22 GMT
EXPOSE 9000
# Fri, 28 Oct 2022 19:16:23 GMT
CMD ["php-fpm"]
# Fri, 28 Oct 2022 21:21:07 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Oct 2022 21:21:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Oct 2022 21:21:10 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 28 Oct 2022 21:21:10 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Fri, 28 Oct 2022 21:21:11 GMT
WORKDIR /opt/drupal
# Fri, 28 Oct 2022 21:21:24 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 28 Oct 2022 21:21:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:32caca2e9abac2a8ffc2b083d202d57e1970d8adc212be17451a992441fad01b`  
		Last Modified: Tue, 25 Oct 2022 02:29:19 GMT  
		Size: 27.8 MB (27799224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140e6bcf950ee2d755ce50e370b6647bc357dcbd24dd0ece7e8d7b388f84d94d`  
		Last Modified: Tue, 25 Oct 2022 09:56:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d087454ecae3a96210f9074f3beccfe18b333cf212f9946b1aa8a54c4d0c064c`  
		Last Modified: Tue, 25 Oct 2022 09:57:02 GMT  
		Size: 81.2 MB (81234271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2520a6c0f52f7418abcd797a402d8844158c345af1bc2f6a196ef56b0d9b85d6`  
		Last Modified: Tue, 25 Oct 2022 09:56:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83772c2fe3c33ffc1ae7672a4d1d277ee66883ff3dceb968a59bf73a7b69d95c`  
		Last Modified: Fri, 28 Oct 2022 20:45:08 GMT  
		Size: 11.9 MB (11856657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090bf37ac0c38a0c60b2cbf8b398a716a6b3399ac4734872d20d658b45d905c`  
		Last Modified: Fri, 28 Oct 2022 20:45:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371f5875a000a6ea1d8863163ec4ff9d3e27d4cd17ce89008b54ff6d0a723fb`  
		Last Modified: Fri, 28 Oct 2022 20:46:08 GMT  
		Size: 26.0 MB (25981181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d0a9b2db9d3a773ff873f3e21da02ad461cd71dd9ae84346b84fc9653c96f5`  
		Last Modified: Fri, 28 Oct 2022 20:46:05 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a58901009b911e31140a92c9bf577679d4d2ab7107fb91bd4f49d92c86fc260`  
		Last Modified: Fri, 28 Oct 2022 20:46:04 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184eebcc477e23a743fe23cf7c1d5b074be2e098cbd7d4da3498a773a24fd58f`  
		Last Modified: Fri, 28 Oct 2022 20:46:05 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0468288e5a3cf81653ee9f33e067ba4f801bdcd92f4e264584dc2ff005e96aa`  
		Last Modified: Fri, 28 Oct 2022 21:56:30 GMT  
		Size: 1.9 MB (1919980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cfc61f646b4bcefaa9afd71e69154d5911e75a52031e5de382365d23111281`  
		Last Modified: Fri, 28 Oct 2022 21:56:30 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d021bfac3b6801e991e3bc31c9c54d7a809b6297b38d4cd90e934b7e8a0efd86`  
		Last Modified: Fri, 28 Oct 2022 21:56:30 GMT  
		Size: 695.2 KB (695193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d143595f3017d8db623e66aef247c54c88fa7729199be5249ad1f5b0f5680f`  
		Last Modified: Fri, 28 Oct 2022 21:56:30 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d85244121299939f3374802dac16ec9c0cf3ab77398323857cbd064765e369a`  
		Last Modified: Fri, 28 Oct 2022 21:56:34 GMT  
		Size: 17.6 MB (17578517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
