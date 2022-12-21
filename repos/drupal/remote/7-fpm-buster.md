## `drupal:7-fpm-buster`

```console
$ docker pull drupal@sha256:3590006befa1d35fe32e3280a7f3cfbe63e0f66e8d7e636c54acbf9d2e117477
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:7-fpm-buster` - linux; amd64

```console
$ docker pull drupal@sha256:e3faaabc5f7089376e95082f889e6e98b1dfb377639dc94a1dd1a04b2bc76a44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146120897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c0e376051a9fe4c1129ee7456728cfdc9c05043546d7c7fe79da598310efeb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:20:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 05:20:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 05:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:20:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 05:20:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 05:20:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:20:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:20:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 07:07:39 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 21 Dec 2022 07:07:39 GMT
ENV PHP_VERSION=8.0.26
# Wed, 21 Dec 2022 07:07:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Wed, 21 Dec 2022 07:07:39 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Wed, 21 Dec 2022 07:07:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 07:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:17:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 07:17:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:17:24 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 07:17:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 07:17:24 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 07:17:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 21 Dec 2022 07:17:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 21 Dec 2022 07:17:25 GMT
EXPOSE 9000
# Wed, 21 Dec 2022 07:17:25 GMT
CMD ["php-fpm"]
# Wed, 21 Dec 2022 13:32:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:32:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 13:35:27 GMT
ENV DRUPAL_VERSION=7.94
# Wed, 21 Dec 2022 13:35:27 GMT
ENV DRUPAL_MD5=dae634ea0da005c5c435cfa9a9c5c322
# Wed, 21 Dec 2022 13:35:28 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5e7e2c529af2f434f1cd170dacc2d1d41e98be050c7513fcf7967a1366ccab`  
		Last Modified: Wed, 21 Dec 2022 07:26:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d385a4ba170008aa047844209f3315470643dd6cf691a34edb91a2b2fc50d1b`  
		Last Modified: Wed, 21 Dec 2022 07:26:43 GMT  
		Size: 76.7 MB (76687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07776926a26c83e59429f19e43d5f71af16d4beee2837c3c5873353005c859b8`  
		Last Modified: Wed, 21 Dec 2022 07:26:31 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b85169de013431a239c7f4b25568c410f6b84d41cc856933a6111db3668607a`  
		Last Modified: Wed, 21 Dec 2022 07:37:18 GMT  
		Size: 11.2 MB (11191680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6cbf5dd50ed6971076e387c08a1dd89c04b0dfd692680f436d43879fde50bb`  
		Last Modified: Wed, 21 Dec 2022 07:37:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdf6ec41146866f7fbc5e4fae0316642c61c1d1d96ff42839366b08fdd201b5`  
		Last Modified: Wed, 21 Dec 2022 07:37:48 GMT  
		Size: 25.5 MB (25462717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c33c17243f8ffa076d7819bacd606b2f93acc23de148a886c9f6666d52327d4`  
		Last Modified: Wed, 21 Dec 2022 07:37:44 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fd920552ee87f577237eb55a1e72c36f9bce8929759e1d7266cd8db1c2fd05`  
		Last Modified: Wed, 21 Dec 2022 07:37:44 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4674f28092fd2d090b4c4c08bc15eb86d306af0610ea9bbdde5367b3fb4b29c`  
		Last Modified: Wed, 21 Dec 2022 07:37:44 GMT  
		Size: 8.6 KB (8577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a488061224fb66b387380fd96b52a8c2f190ad87b64f69396c3051679fa029`  
		Last Modified: Wed, 21 Dec 2022 13:48:09 GMT  
		Size: 2.2 MB (2223379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533f8742d409aabd6557cadd29d4487d591f35614bed67f2ae66892e69768bb8`  
		Last Modified: Wed, 21 Dec 2022 13:48:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946e96c6d5f2b2d7ebaf473ddd1c3c0d0c611ec9610eaf9f253d6600f3c13c1b`  
		Last Modified: Wed, 21 Dec 2022 13:52:53 GMT  
		Size: 3.4 MB (3402615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:aeadf5ff1ee1f5381892cb8024065d03f58404804d2b5011633c15f565575ead
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121726128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6840803fe18f73ccdc22ce052a4202dd9434e5b064c5f41c193529c253f8df93`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 06 Dec 2022 00:59:27 GMT
ADD file:be297820b3c24f32c3d19e62f8aad3c9d2b37db08077869258a7d3aba92f555f in / 
# Tue, 06 Dec 2022 00:59:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:43:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 03:43:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 03:43:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 03:43:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 03:43:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 03:43:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 03:43:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 03:43:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 04:31:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 06 Dec 2022 04:31:14 GMT
ENV PHP_VERSION=8.0.26
# Tue, 06 Dec 2022 04:31:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Tue, 06 Dec 2022 04:31:15 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Tue, 06 Dec 2022 04:31:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 04:31:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:39:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 04:39:42 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:39:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 04:39:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 04:39:43 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 04:39:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 06 Dec 2022 04:39:44 GMT
STOPSIGNAL SIGQUIT
# Tue, 06 Dec 2022 04:39:44 GMT
EXPOSE 9000
# Tue, 06 Dec 2022 04:39:44 GMT
CMD ["php-fpm"]
# Tue, 06 Dec 2022 14:25:40 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 14:25:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Dec 2022 01:09:56 GMT
ENV DRUPAL_VERSION=7.94
# Thu, 15 Dec 2022 01:09:56 GMT
ENV DRUPAL_MD5=dae634ea0da005c5c435cfa9a9c5c322
# Thu, 15 Dec 2022 01:09:57 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:f2a5c00904a21a940a9e4ec3efaca80bebbbf2775e4c9bbe0ce9c05e967335f0`  
		Last Modified: Tue, 06 Dec 2022 01:06:56 GMT  
		Size: 22.7 MB (22748937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0fd527e893f67f85a1c13343cbede410f56ac2185449a54edd3b425543be96`  
		Last Modified: Tue, 06 Dec 2022 04:53:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac07484df679107c13570d32f6ecb607555e90ad4d72b959e42627a3f272b0e8`  
		Last Modified: Tue, 06 Dec 2022 04:53:39 GMT  
		Size: 59.5 MB (59542386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e21f2c80981b6bcaf17192519e63c71cc6376e9e11ebd6bc867f7fd4e961d0`  
		Last Modified: Tue, 06 Dec 2022 04:53:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e648499a5c2ebe9098edb00c8f48e9ce81d068c0332619e830cd93404f2efc`  
		Last Modified: Tue, 06 Dec 2022 05:02:05 GMT  
		Size: 11.2 MB (11189745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71f25b826fb96795747654f7335092e17278f9eaf21c0d9d4af4c27862add5e`  
		Last Modified: Tue, 06 Dec 2022 05:02:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43350f0dd869db71dc366cd9d323e2235195b8f5861f1cb68f3f38a57a46c67`  
		Last Modified: Tue, 06 Dec 2022 05:02:48 GMT  
		Size: 23.2 MB (23221620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ee8bddce9e03acc53bbd13ff1908ea207adda05d69b7d397377c7626827f1`  
		Last Modified: Tue, 06 Dec 2022 05:02:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff627b2a123cfa32e121e0c2ba3f5864a20e705569079082f7082003b2c929`  
		Last Modified: Tue, 06 Dec 2022 05:02:43 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8e70f7ba9af37104a9b66fcc852bf34cc009af18821a051446db1f7782fa80`  
		Last Modified: Tue, 06 Dec 2022 05:02:43 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e047c61f0f6366dd7ab38caf81e6afa4b2d407f0e266e3a67d9b43cdaa99295a`  
		Last Modified: Tue, 06 Dec 2022 14:51:35 GMT  
		Size: 1.6 MB (1608605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53de35b363ac088d90b211a2042cb59cdb1395ea73be03be2871c8c6917d35f9`  
		Last Modified: Tue, 06 Dec 2022 14:51:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b37a0f38f539eee65862aaddb8cd922cfae2d10a9eb364e15284074941d18a8`  
		Last Modified: Thu, 15 Dec 2022 01:25:33 GMT  
		Size: 3.4 MB (3402295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:f1baabb4916ef6bc4260015670c0c7290f3a07d9ddcc5d6b28aae914faf8ad76
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137664687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6f92dec6a7338adac9b4b89112b00b5b67a3c9f244163a0528d783b07a2c42`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 11:37:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 11:37:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 11:37:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 11:37:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 11:37:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 11:37:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 11:37:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 11:37:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 12:23:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 06 Dec 2022 12:23:01 GMT
ENV PHP_VERSION=8.0.26
# Tue, 06 Dec 2022 12:23:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Tue, 06 Dec 2022 12:23:01 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Tue, 06 Dec 2022 12:23:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 12:23:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:29:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 12:29:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:29:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 12:29:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 12:29:12 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 12:29:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 06 Dec 2022 12:29:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 06 Dec 2022 12:29:13 GMT
EXPOSE 9000
# Tue, 06 Dec 2022 12:29:13 GMT
CMD ["php-fpm"]
# Tue, 06 Dec 2022 18:16:05 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 18:16:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Dec 2022 01:45:56 GMT
ENV DRUPAL_VERSION=7.94
# Thu, 15 Dec 2022 01:45:56 GMT
ENV DRUPAL_MD5=dae634ea0da005c5c435cfa9a9c5c322
# Thu, 15 Dec 2022 01:45:57 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcfb88424deadf3813dacd34bdd5c43e0efbd63081ff1150e5dec324b5cb9ca`  
		Last Modified: Tue, 06 Dec 2022 12:36:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe65ddacb555d1b9f51638b7e3ba1d5bb8acc73fbb6c25384b75e2be98e18d5`  
		Last Modified: Tue, 06 Dec 2022 12:36:18 GMT  
		Size: 70.4 MB (70362880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fa4c2f5fe9157eb2e01d87095eef0519b1db09108d017084f6446fff830a5a`  
		Last Modified: Tue, 06 Dec 2022 12:36:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea2288e913584ca8eb3674598273505acea11e0337de1cc08194272bcd0b61e`  
		Last Modified: Tue, 06 Dec 2022 12:41:57 GMT  
		Size: 11.2 MB (11190445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2756b0c232e2edee06336edc00035caf85de528e3afa087281e4e86c32f5dce`  
		Last Modified: Tue, 06 Dec 2022 12:41:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45beea1f3b0198e6c9029e109f57d2c215a236fac7569e068c5a6d05cd089c3`  
		Last Modified: Tue, 06 Dec 2022 12:42:27 GMT  
		Size: 24.9 MB (24905025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7206c860cef04df4523436676cebd4c50de37e82369598d02c892768dacd84`  
		Last Modified: Tue, 06 Dec 2022 12:42:24 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d255d8dcdf027bee94346d7a84efc21358393e851b857fe36eea31624d5354c2`  
		Last Modified: Tue, 06 Dec 2022 12:42:24 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0253bfac6a20863b1f160b82997225193ad90f5ed44972d556139d5a9f81695`  
		Last Modified: Tue, 06 Dec 2022 12:42:23 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc9fee610ede6d6e673b7197f873b7e6be52406ae5fb3a0a1e99e8523825127`  
		Last Modified: Tue, 06 Dec 2022 18:30:53 GMT  
		Size: 1.9 MB (1876185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc847f62dc6e802ad1d846b0b17f4aa6611b08bf06b0296ec6bdfa5e755f792f`  
		Last Modified: Tue, 06 Dec 2022 18:30:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50650d4af371b68103fcc496ea9c7ef4cc343346a1c9b9930d295dbab16a119e`  
		Last Modified: Thu, 15 Dec 2022 01:52:32 GMT  
		Size: 3.4 MB (3402618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-buster` - linux; 386

```console
$ docker pull drupal@sha256:b8d0d851d8499ae914e7d549c947922bdcf5f7f3d4ca971b2090d974c02853cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926af4c33fa3817decb16084f2b9fceba49fa883281ee3dc99f70cc76eab07f1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:45 GMT
ADD file:48a2a0e6cb166df412bb4f6ad30537c66bc6be97ce4c8fc582fd5ac8c6129b5a in / 
# Wed, 21 Dec 2022 01:39:46 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:52:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 02:52:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 02:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:52:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 02:52:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 02:52:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 02:52:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 02:52:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 04:33:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 21 Dec 2022 04:33:28 GMT
ENV PHP_VERSION=8.0.26
# Wed, 21 Dec 2022 04:33:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Wed, 21 Dec 2022 04:33:30 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Wed, 21 Dec 2022 04:33:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 04:33:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:42:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 04:42:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:42:28 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 04:42:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 04:42:30 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 04:42:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 21 Dec 2022 04:42:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 21 Dec 2022 04:42:33 GMT
EXPOSE 9000
# Wed, 21 Dec 2022 04:42:34 GMT
CMD ["php-fpm"]
# Wed, 21 Dec 2022 15:29:59 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 15:29:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 15:34:06 GMT
ENV DRUPAL_VERSION=7.94
# Wed, 21 Dec 2022 15:34:06 GMT
ENV DRUPAL_MD5=dae634ea0da005c5c435cfa9a9c5c322
# Wed, 21 Dec 2022 15:34:08 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:9099d8a02dc0a7901931d2811fa3078b18ecd3a40a156cbcfd91629126463f80`  
		Last Modified: Wed, 21 Dec 2022 01:45:34 GMT  
		Size: 27.8 MB (27798412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059e8367727edb1fc1a41e9b0f8ad5b0608020745ccabd6b8d52e53026bd118c`  
		Last Modified: Wed, 21 Dec 2022 04:56:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8ad3db0ab49efd6bd406a7d3ad6840dbb73a96a726765be6e3a8850335c2a6`  
		Last Modified: Wed, 21 Dec 2022 04:57:11 GMT  
		Size: 81.2 MB (81234660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d0ba56dcb1911150c21614d7e7a92926708de4a7f09f08247c3d90328b56f5`  
		Last Modified: Wed, 21 Dec 2022 04:56:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191b8dac6aa023bba3544380a5b2ed246145038b6aee1b1163f0154d4caf2044`  
		Last Modified: Wed, 21 Dec 2022 05:10:40 GMT  
		Size: 11.0 MB (10977076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c06e0c34e5cb0013a1a168ebe16f0feda53e1377d4848c10f4dadb9386dfef`  
		Last Modified: Wed, 21 Dec 2022 05:10:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9019f15efd332d93ffee878ca51b94d42836052f5d5492d75eef399e45b78c`  
		Last Modified: Wed, 21 Dec 2022 05:11:15 GMT  
		Size: 25.7 MB (25703123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14898c65c3e4417740f5682247a48fc32c247239cc3ecb792da3b330e564de`  
		Last Modified: Wed, 21 Dec 2022 05:11:12 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acbe2fa9110b179ee99c9551db124cd722238cf609d789b6bdb4e1c5ddd79c9`  
		Last Modified: Wed, 21 Dec 2022 05:11:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccff768486e0709e45e10ca21d5d7f6dca695ed10ef04ec5fb5df164af8813b`  
		Last Modified: Wed, 21 Dec 2022 05:11:12 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea71e77a88f2ad2e9ed55d5749eb1af0126dc9f270c885022dd450d603b1f23`  
		Last Modified: Wed, 21 Dec 2022 15:53:53 GMT  
		Size: 2.1 MB (2078052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506879b24948e326d0e7629bbf3b5b2f084053a15d1be1437c1640a2f1603883`  
		Last Modified: Wed, 21 Dec 2022 15:53:53 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3f281286cf7672bbbeb5e425317fe28ae9d4ba945e23cf28697b187d978f2a`  
		Last Modified: Wed, 21 Dec 2022 15:59:35 GMT  
		Size: 3.4 MB (3402288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
