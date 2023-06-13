## `backdrop:fpm`

```console
$ docker pull backdrop@sha256:aa3a06ac6f304d3d3cf8fb1382fcc3cfbe244be30eb4c41191b60229b08555e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:d96c206e3183cc8367d2ce268a79092397a13a1cca4e27b69f637c2677a67f72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172616830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f7273a9156f373d365828ba8a07984c4055b556f22ff87d438954c753832d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 10:48:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Jun 2023 10:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Jun 2023 10:49:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 10:49:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Jun 2023 10:49:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 13 Jun 2023 10:49:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 10:49:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 10:49:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Jun 2023 11:42:42 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Jun 2023 11:42:42 GMT
ENV PHP_VERSION=8.1.20
# Tue, 13 Jun 2023 11:42:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Tue, 13 Jun 2023 11:42:42 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Tue, 13 Jun 2023 11:42:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Jun 2023 11:42:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Jun 2023 11:52:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Jun 2023 11:52:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 13 Jun 2023 11:52:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Jun 2023 11:52:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Jun 2023 11:52:28 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 11:52:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 13 Jun 2023 11:52:28 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jun 2023 11:52:28 GMT
EXPOSE 9000
# Tue, 13 Jun 2023 11:52:28 GMT
CMD ["php-fpm"]
# Tue, 13 Jun 2023 23:01:25 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Tue, 13 Jun 2023 23:01:25 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 23:01:25 GMT
ENV BACKDROP_VERSION=1.25.1
# Tue, 13 Jun 2023 23:01:25 GMT
ENV BACKDROP_MD5=9c2bbcb4ddd52cbd85e1e31ee4fc8a17
# Tue, 13 Jun 2023 23:01:28 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Tue, 13 Jun 2023 23:01:29 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Tue, 13 Jun 2023 23:01:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 23:01:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a8e7424b0eb1756156f3f94aa6075c6842bc72bcaadd91cf3f610ddbac736`  
		Last Modified: Tue, 13 Jun 2023 12:38:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf7646946631a4f463704b65ca33340db6357e1731ad2aa74b5ba46d5ae7910`  
		Last Modified: Tue, 13 Jun 2023 12:38:26 GMT  
		Size: 91.6 MB (91635678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c4f9b927126ea34eb19ac1b8a7d304e352049cadcef67dae288b0b3fa4a6c`  
		Last Modified: Tue, 13 Jun 2023 12:38:13 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910752c8303d3bd4528b96e6d2aa704dcd9760f064bf62b1a729ee8ddae4da36`  
		Last Modified: Tue, 13 Jun 2023 12:44:00 GMT  
		Size: 12.1 MB (12111633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845bf6b9034a9f5d49659fce7dd068adcec8af99adc05cba152c1b951d1d0738`  
		Last Modified: Tue, 13 Jun 2023 12:44:00 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0aa3e7d0d43d2b277db294d75548a03fce7e3f8736f486ee851cab3fd207a7`  
		Last Modified: Tue, 13 Jun 2023 12:44:43 GMT  
		Size: 26.3 MB (26250179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33568ede0d664f92e94002a37f14c0fcfb9a0c9d0ab8be28b48c200d8b01f122`  
		Last Modified: Tue, 13 Jun 2023 12:44:39 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f796a09aca7e6b3f41787e0260105d5aee8e2e397d5edc4f8a5aba9883a6a4a0`  
		Last Modified: Tue, 13 Jun 2023 12:44:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19898b61118835ab383d3767498bb7a1829400cbf73bccf7be074e9f4cf334e`  
		Last Modified: Tue, 13 Jun 2023 12:44:39 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcb5d427e586068ce2825332b2f4152dc71bc0bff51a8ad086c8993d2ec536d`  
		Last Modified: Tue, 13 Jun 2023 23:02:22 GMT  
		Size: 2.4 MB (2422710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad935bd5d9fb394811723788c360806fea4a556ed672e47529a20c082b34064`  
		Last Modified: Tue, 13 Jun 2023 23:02:23 GMT  
		Size: 8.8 MB (8765712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c396e410eed10a3fb42557c9800ab4d392f5fbc304e1a22e7eb9ac2d20c4f528`  
		Last Modified: Tue, 13 Jun 2023 23:02:21 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:34417d7868f201e40d518cebd2fbf8cd8249e0a3ae675094a765ce9127a6fb56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166556146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f51af6351a70a4162931d5d520945770da696cf754054f393a09e19b1052f7e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 08:27:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Jun 2023 08:27:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Jun 2023 08:27:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 08:27:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Jun 2023 08:27:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 13 Jun 2023 08:27:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 08:27:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 08:27:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Jun 2023 09:18:05 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Jun 2023 09:18:05 GMT
ENV PHP_VERSION=8.1.20
# Tue, 13 Jun 2023 09:18:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Tue, 13 Jun 2023 09:18:05 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Tue, 13 Jun 2023 09:18:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Jun 2023 09:18:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Jun 2023 09:27:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Jun 2023 09:27:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 13 Jun 2023 09:27:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Jun 2023 09:27:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Jun 2023 09:27:04 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 09:27:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 13 Jun 2023 09:27:05 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jun 2023 09:27:05 GMT
EXPOSE 9000
# Tue, 13 Jun 2023 09:27:05 GMT
CMD ["php-fpm"]
# Tue, 13 Jun 2023 19:09:30 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Tue, 13 Jun 2023 19:09:30 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 19:09:30 GMT
ENV BACKDROP_VERSION=1.25.1
# Tue, 13 Jun 2023 19:09:30 GMT
ENV BACKDROP_MD5=9c2bbcb4ddd52cbd85e1e31ee4fc8a17
# Tue, 13 Jun 2023 19:09:33 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Tue, 13 Jun 2023 19:09:33 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:09:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:09:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130acfd80cbcc92bb088194a5f70107163cf2c64ec03afbb8cef48a8d5cb64b9`  
		Last Modified: Tue, 13 Jun 2023 10:01:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c452fc3771f0e24d7a4608cb7fa0a3fef8338f180867edddc951516ee483df5f`  
		Last Modified: Tue, 13 Jun 2023 10:01:56 GMT  
		Size: 86.9 MB (86928318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e73365700a60b46358bf991bb3261b2892f868de457a8248e947d38b0e2ec7`  
		Last Modified: Tue, 13 Jun 2023 10:01:46 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057240c114d62c093225ecb2f25e1fb120d14d85d1ae5ffebcbf3235a060f639`  
		Last Modified: Tue, 13 Jun 2023 10:07:22 GMT  
		Size: 12.1 MB (12110892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261cdaf3dea02295e9b652f0a6e24217fa30b46c56137b29556d72355ccf37bb`  
		Last Modified: Tue, 13 Jun 2023 10:07:21 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9667c550c5b773eae15d1d8286dbf153b0970f8e3faaf5989e8cb8af60fa1e7e`  
		Last Modified: Tue, 13 Jun 2023 10:08:03 GMT  
		Size: 26.3 MB (26289957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bd8b43a56a5ba574db217ae164bf8d0c5b1f1807909f6d020f760389cf4da3`  
		Last Modified: Tue, 13 Jun 2023 10:08:00 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8edcfd607aa0599182b1c27bb0b11ae99f227fd3c81fdf8ce3e1e42a0de84f`  
		Last Modified: Tue, 13 Jun 2023 10:08:00 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389016bdc7b75157113a00b89a23ac21dfa9197d65ecb6fa81f1742ff1e27d45`  
		Last Modified: Tue, 13 Jun 2023 10:08:00 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66003234794732c9b9029059a3551949ff32f8cb6c267937828ea98cc4efa76`  
		Last Modified: Tue, 13 Jun 2023 19:10:20 GMT  
		Size: 2.4 MB (2384896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d523a2b4c34cd9649c633e56f3ef2ae01b39f151d302d4c5e6f82e068615ab`  
		Last Modified: Tue, 13 Jun 2023 19:10:21 GMT  
		Size: 8.8 MB (8765744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a398e269f3cab8cbb1c467d7120dc7f89a45405717a22d559ec83e6c8e5a50fa`  
		Last Modified: Tue, 13 Jun 2023 19:10:20 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
