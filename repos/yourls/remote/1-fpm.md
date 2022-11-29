## `yourls:1-fpm`

```console
$ docker pull yourls@sha256:4cc511eb3277ab11cc513218e894babbb71fb1ee57873d47785d614c3f19bc5d
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

### `yourls:1-fpm` - linux; amd64

```console
$ docker pull yourls@sha256:7d30f1f9f6d734b7b6ca99ff0cea173daf8726a11ef2ddb036e4816bac5841a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165838149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58aa4553890d4cfc8e4749dd209107f4ee3ff42973eadb379bfbda82601ba1d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:12:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 04:12:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 04:13:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:13:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 04:13:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 04:13:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:13:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:13:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 04:40:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:29:59 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:29:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:29:59 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:30:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:30:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:39:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:39:41 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:39:41 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:39:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:39:41 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:39:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Nov 2022 02:39:42 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Nov 2022 02:39:42 GMT
EXPOSE 9000
# Tue, 29 Nov 2022 02:39:42 GMT
CMD ["php-fpm"]
# Tue, 29 Nov 2022 06:52:06 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 29 Nov 2022 06:52:07 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 29 Nov 2022 06:52:47 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 29 Nov 2022 06:52:48 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Nov 2022 06:52:48 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 06:52:48 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 06:52:48 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 29 Nov 2022 06:52:48 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 06:52:48 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 06:52:50 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 29 Nov 2022 06:52:50 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 29 Nov 2022 06:52:50 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 29 Nov 2022 06:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 06:52:50 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c428f1a494230852524a2a5957cc5199c36c8b403305e0e877d580bd0ec9e763`  
		Last Modified: Tue, 15 Nov 2022 06:23:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156740b07ef8a632f9f7bea4e57e4ee5541ade376adf9169351a1265382e39de`  
		Last Modified: Tue, 15 Nov 2022 06:23:30 GMT  
		Size: 91.6 MB (91634870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a4c8af82f00730b7427e47bda7f76cea2e2b9aea421750bc9025aface98d8`  
		Last Modified: Tue, 15 Nov 2022 06:23:16 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cec524356b5e0d7eab06c9c1c368a40a25383a09b1f0d19cb275158b4ca695`  
		Last Modified: Tue, 29 Nov 2022 04:16:45 GMT  
		Size: 12.1 MB (12122958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b8793c8b77074150f2fb364fde747711c8cd06a6d26cff8db983c501a466b`  
		Last Modified: Tue, 29 Nov 2022 04:16:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875d136c67265cf991615a23185fb5aa185492abadc8f93ae971ee655e144a48`  
		Last Modified: Tue, 29 Nov 2022 04:17:58 GMT  
		Size: 26.2 MB (26233480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e27463d4d66a9b230003380a91262cf14c35f7f74c97f6c12734ba3c90d39e`  
		Last Modified: Tue, 29 Nov 2022 04:17:54 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a48c560dd1f4538dac1d59e35dc50802ecaf71f48406b01ab2caadd0c02738e`  
		Last Modified: Tue, 29 Nov 2022 04:17:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb32a346dc5e9d40a463036155903fee8c4d3a71b537de4f2c1db7abc58d71ae`  
		Last Modified: Tue, 29 Nov 2022 04:17:54 GMT  
		Size: 8.6 KB (8627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ae0e848ac60618501a6688b52a65351559e1e8770ae14caf520b53661fe76f`  
		Last Modified: Tue, 29 Nov 2022 06:54:50 GMT  
		Size: 514.4 KB (514425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723bdb5e936f69235f457c765d5c8b5b01c2de53c1ab0e23b665b6500018639e`  
		Last Modified: Tue, 29 Nov 2022 06:54:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9abda10b8bc59e6f3d8c8a996550efdfce5d85877f443fccd97524067740f3d`  
		Last Modified: Tue, 29 Nov 2022 06:54:50 GMT  
		Size: 3.9 MB (3903533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb61698a6d39c2964b91077ca076b9731f612f2ef493f2e2cd8bc95ae44dd81`  
		Last Modified: Tue, 29 Nov 2022 06:54:49 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6e83d0257a536ec69e5becc6d716d9bd3dda9523bc215130ffde9c0dab4181`  
		Last Modified: Tue, 29 Nov 2022 06:54:49 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:36eb608067a3ee8407e092da0304cbec556fa88da333f99fe0ecae9fd8785106
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143613447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367149352a348753dbc550e4ca2c5adecf04d3abdc9dd4606612a736b0a2ebe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 01:57:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 01:57:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 01:58:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 01:58:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 01:58:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 01:58:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 01:58:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 01:58:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:13:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:07:07 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:07:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:07:07 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:07:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:07:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:19:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:19:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:19:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:19:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:19:26 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:19:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Nov 2022 02:19:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Nov 2022 02:19:26 GMT
EXPOSE 9000
# Tue, 29 Nov 2022 02:19:27 GMT
CMD ["php-fpm"]
# Tue, 29 Nov 2022 04:31:43 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 29 Nov 2022 04:31:43 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 29 Nov 2022 04:31:43 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 29 Nov 2022 04:31:43 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 29 Nov 2022 04:31:44 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 29 Nov 2022 04:31:44 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 29 Nov 2022 04:31:44 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 29 Nov 2022 04:31:44 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 29 Nov 2022 04:32:07 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 29 Nov 2022 04:32:08 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Nov 2022 04:32:08 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 04:32:08 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 04:32:09 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 29 Nov 2022 04:32:09 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 04:32:09 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 04:32:11 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 29 Nov 2022 04:32:11 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 29 Nov 2022 04:32:11 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 29 Nov 2022 04:32:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 04:32:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf8f13a67ff628e982fa37f19e46a30b6c95f885b9caf0fe288d9e44fc0fe23`  
		Last Modified: Tue, 15 Nov 2022 03:18:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b67f60155678149aec805bafe02c6067447f321279766240c3ae4d1bf9745`  
		Last Modified: Tue, 15 Nov 2022 03:18:47 GMT  
		Size: 73.7 MB (73687967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee4232fc94727d61967ec10566bb2eb1be8604bec5ccee5d4cbf30b97fac1a7`  
		Last Modified: Tue, 15 Nov 2022 03:18:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e082f0a05a1a065be888c0c4418b2a1fadb1df7e0e66a6c55f34eec7ee3c98`  
		Last Modified: Tue, 29 Nov 2022 02:53:15 GMT  
		Size: 12.1 MB (12121344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076046b4cd140dab26fb231ad6f5af584b28ea7423f8ad495e9e08f307d38874`  
		Last Modified: Tue, 29 Nov 2022 02:53:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac290aa2621c9d486231d468ed018a1dc6d443d62f8a03723228997d322a09b`  
		Last Modified: Tue, 29 Nov 2022 02:55:17 GMT  
		Size: 24.8 MB (24819562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9132efcf0cfd70bd2f959528b7c0676ba4406203c6481b8284083a9a14cea84`  
		Last Modified: Tue, 29 Nov 2022 02:55:11 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43139bafa6b8fcd54f72117c51a62f502c819ff5a99c5d5a0c9c7d41d2382c5`  
		Last Modified: Tue, 29 Nov 2022 02:55:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0626e8a5778ba6727540968943d077dbc064bf2afb1766c5278a39ebc7cac70`  
		Last Modified: Tue, 29 Nov 2022 02:55:11 GMT  
		Size: 8.6 KB (8626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea72f1546d1a9a0771bd3a549fd2de4c4c1638d978366a218a32d20de5b12de`  
		Last Modified: Tue, 29 Nov 2022 04:33:32 GMT  
		Size: 150.7 KB (150709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1b3be19ffd6967532543b9446e9e28c9f1f7ee06595fc121131b6a530aecbb`  
		Last Modified: Tue, 29 Nov 2022 04:33:32 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1abd9868e12d050f5b2a7b75a0b234ccad5a042b339e07cd952c2d3589ebab`  
		Last Modified: Tue, 29 Nov 2022 04:33:33 GMT  
		Size: 3.9 MB (3903530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae289bb54a63bf85d43c0e71ceb8396a20a1fdaffe0da5062df88d67e26ed7fb`  
		Last Modified: Tue, 29 Nov 2022 04:33:32 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab08c4cffa781b9e51174fe4ea6637c3ede362a1035157ae5e9df66875e0b3c8`  
		Last Modified: Tue, 29 Nov 2022 04:33:32 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:de8d08bc5ad593f5623b5750712bdba79f7f97fbeb113d2ca7dfa0355d9cb8a7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135999208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2337322abdad729ffd6a7cd22ead7feac78f03bd09f62845860e7cef92687efa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 03:55:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 03:55:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 03:56:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:56:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 03:56:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 03:56:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 03:56:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 03:56:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 04:20:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 15 Nov 2022 04:20:39 GMT
ENV PHP_VERSION=8.1.12
# Tue, 15 Nov 2022 04:20:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Tue, 15 Nov 2022 04:20:39 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Tue, 15 Nov 2022 04:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 04:20:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 04:28:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 04:28:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 04:28:59 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 04:28:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 04:29:00 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 04:29:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 04:29:00 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 04:29:00 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 04:29:00 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 15 Nov 2022 10:26:12 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 15 Nov 2022 10:26:13 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 15 Nov 2022 10:26:32 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 15 Nov 2022 10:26:32 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 10:26:32 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 15 Nov 2022 10:26:33 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 15 Nov 2022 10:26:33 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 15 Nov 2022 10:26:33 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 15 Nov 2022 10:26:33 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 15 Nov 2022 10:26:35 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 15 Nov 2022 10:26:35 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 15 Nov 2022 10:26:35 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:26:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9882e3666a8ea23dcd83cf24efee4c2bc629f92dcf64bbfb5c9323497a250bd`  
		Last Modified: Tue, 15 Nov 2022 06:04:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc118326146d74f82c6277eb8df1029bf3b7f96486d7830fea19631b696893be`  
		Last Modified: Tue, 15 Nov 2022 06:05:05 GMT  
		Size: 69.3 MB (69320668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823b0bab372d5757e3e8f322d5ca5aefbd8984c35bed9771179b5de70ac8aad0`  
		Last Modified: Tue, 15 Nov 2022 06:04:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30e7c62057020e1d1911fb38ba64ce6c81b6017019b0a047aa2e1df1d69cc3c`  
		Last Modified: Tue, 15 Nov 2022 06:08:32 GMT  
		Size: 12.1 MB (12065148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea387960ad5f04ce87d91fed96a1fa304ff205b5840392ae8f17d16fcbf242ef`  
		Last Modified: Tue, 15 Nov 2022 06:08:30 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547dd2db466b77aa9a00e3e7c212db2d0e940c0bea712b9c3084cafe2a8d6e16`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 24.0 MB (23979051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef117fe7785237dc1a3616fe5058a6310b02ffef8bbf76326a2b142f38156a0`  
		Last Modified: Tue, 15 Nov 2022 06:10:11 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b07e382c1b86fcae510fbdb7c30c1586aa9d3cabff85d387acd2436dd435a2`  
		Last Modified: Tue, 15 Nov 2022 06:10:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8220be868d8d83861532351c8fa37d4cf4dbcd26147a42d809893ba2a9cbbb`  
		Last Modified: Tue, 15 Nov 2022 06:10:11 GMT  
		Size: 8.6 KB (8621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4140e1709660041793420f6de2550e914b4b61da91b835e0e558db8a1ab9b1`  
		Last Modified: Tue, 15 Nov 2022 10:28:10 GMT  
		Size: 138.4 KB (138427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5911aee9aa481b9e4dccfe5bb271055b6953350572dc81cfb41a7f4a1dad3660`  
		Last Modified: Tue, 15 Nov 2022 10:28:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de9682b1a673480992412b0dd44b9d20cd2c547bd0c6085029218123263a7dc`  
		Last Modified: Tue, 15 Nov 2022 10:28:11 GMT  
		Size: 3.9 MB (3903533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8411dc79028d35e1791410a37d07d2e8d91d2febcef009b2e589ad061391b632`  
		Last Modified: Tue, 15 Nov 2022 10:28:10 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75bdf0fab19d674e015842f674f8f92606eb622a3f88bb45f33e3294fc2b318`  
		Last Modified: Tue, 15 Nov 2022 10:28:10 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:3c0f1639d359721d92bc53c7d62251c1756dbaafe9a5c6298134a6dcca0ff5a8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160096727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b73685abe1cc81d8c7870fb4d598606d2039482d6ff19d3a55fe4ec6f2ac292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 01:58:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 01:58:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 01:58:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 01:58:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 01:58:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 01:58:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 01:58:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 01:58:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:23:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:42:08 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:42:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:42:08 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:42:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:42:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:51:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:51:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:51:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:51:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:51:13 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:51:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Nov 2022 02:51:14 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Nov 2022 02:51:14 GMT
EXPOSE 9000
# Tue, 29 Nov 2022 02:51:14 GMT
CMD ["php-fpm"]
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 29 Nov 2022 05:39:36 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 29 Nov 2022 05:40:30 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 29 Nov 2022 05:40:30 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Nov 2022 05:40:30 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 05:40:30 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 05:40:30 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 29 Nov 2022 05:40:30 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 05:40:31 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 05:40:32 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 29 Nov 2022 05:40:32 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 29 Nov 2022 05:40:32 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 29 Nov 2022 05:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 05:40:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826c69643efc7a2fa413b41d83553f587c092a532d2d6582de3caf323e79a005`  
		Last Modified: Tue, 15 Nov 2022 03:57:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c4af7a39c39eedcaf52194d52f333a71017ffe436a4e3725ebeb10f91baccf`  
		Last Modified: Tue, 15 Nov 2022 03:58:04 GMT  
		Size: 86.9 MB (86928187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bbe7211684bcd10ae8486cd441fc15f18504b0795e1bbc3b0687b492b215e`  
		Last Modified: Tue, 15 Nov 2022 03:57:53 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dae603c4c8705f4bacc06252c7eeb8b444ea302ceb67bc60dfb0dde1e53dd8d`  
		Last Modified: Tue, 29 Nov 2022 04:13:20 GMT  
		Size: 12.1 MB (12122207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317745cb852be98ac94b96ce221ddfcda8a182d82d69bcafc1b5707f149ced8`  
		Last Modified: Tue, 29 Nov 2022 04:13:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d79caecdf2339ba6667d54e4f0a4c6f66579bc3d55850c6e68025ea83545aa`  
		Last Modified: Tue, 29 Nov 2022 04:14:34 GMT  
		Size: 26.3 MB (26273422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175ac046b2b61c00457eb64434251f398736684fa19e7b16f22b9d82b74a2fa8`  
		Last Modified: Tue, 29 Nov 2022 04:14:30 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917380a1868d234de443893755644ba3c3774aec082daf8cea12eb84885d29e7`  
		Last Modified: Tue, 29 Nov 2022 04:14:30 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883a48931058a923f5852d852134d4cc1d6a52c8c482a147cd06db3beedc7533`  
		Last Modified: Tue, 29 Nov 2022 04:14:30 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf10d85da173708012be65f61c78fffe7df75a18c6268658d0217f9d5326324`  
		Last Modified: Tue, 29 Nov 2022 05:43:09 GMT  
		Size: 792.5 KB (792524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1139bf4e454e68445cf12bf661a25cec8045b042cab72360513ff316acdd47de`  
		Last Modified: Tue, 29 Nov 2022 05:43:09 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95600d07e030f166e4f6ec38cf2d2b0018f14c928f9a2d2634ffe7f2d444b898`  
		Last Modified: Tue, 29 Nov 2022 05:43:10 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ac52de984a0b6ce52e511a13fd3058d5e2876cef43cc888cddfa3051649e2`  
		Last Modified: Tue, 29 Nov 2022 05:43:09 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db719b62f74eb7b1c62a2304402bbf17d795010bebd5a14711d87da53c6e76c`  
		Last Modified: Tue, 29 Nov 2022 05:43:09 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; 386

```console
$ docker pull yourls@sha256:44340bee26fd60adf66192bd18b5bd5535cbdd3b9c11b42a5b54b026430e8c8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167716775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cdf8d6069d71731677dff8a98a60cb6d8d15d01eaace0c6a8c48be1da7d986b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 01:52:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 01:52:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 01:52:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 01:52:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 01:52:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 01:52:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 01:52:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 01:52:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:18:46 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:43:20 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:43:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:43:22 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:43:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:43:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:52:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:52:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:52:34 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:52:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:52:36 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:52:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Nov 2022 02:52:38 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Nov 2022 02:52:39 GMT
EXPOSE 9000
# Tue, 29 Nov 2022 02:52:40 GMT
CMD ["php-fpm"]
# Tue, 29 Nov 2022 06:58:45 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 29 Nov 2022 06:58:45 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 29 Nov 2022 06:58:46 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 29 Nov 2022 06:58:47 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 29 Nov 2022 06:58:48 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 29 Nov 2022 06:58:49 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 29 Nov 2022 06:58:50 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 29 Nov 2022 06:58:51 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 29 Nov 2022 06:59:27 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 29 Nov 2022 06:59:28 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Nov 2022 06:59:29 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 06:59:30 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 06:59:31 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 29 Nov 2022 06:59:32 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 06:59:33 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 06:59:36 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 29 Nov 2022 06:59:37 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 29 Nov 2022 06:59:38 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 29 Nov 2022 06:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 06:59:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f74128087fbd00203c9028d953e0a937b12c994f8a56ac87e8ff263befa3b0`  
		Last Modified: Tue, 15 Nov 2022 04:26:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1024123a0ace8893c46fec8ab108beb66e5e2865e5aec7e8a3c42ecd90611099`  
		Last Modified: Tue, 15 Nov 2022 04:26:17 GMT  
		Size: 92.5 MB (92511993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bcd3101f8e73a2151ce2cf6f10ca57081c851c0790ad320f2ce2b6a279802`  
		Last Modified: Tue, 15 Nov 2022 04:26:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541fa53efa298bf12dd369dd8e61229327364c9aca97615c0cca2627ad530061`  
		Last Modified: Tue, 29 Nov 2022 04:34:36 GMT  
		Size: 11.9 MB (11904961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a0d660f33ca3e4e0c44412dca66d7c47cc31623cfcc9fba08954d253bbc3e2`  
		Last Modified: Tue, 29 Nov 2022 04:34:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695aaf18681f95c720002bc81d63180fbd883ccf2a82761ed1b24c1a8287e128`  
		Last Modified: Tue, 29 Nov 2022 04:36:06 GMT  
		Size: 26.5 MB (26492393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f468fa5cdd5be0f7f2a23bd0b025fc98d0c7c699bd830a09a5be32e779f659ed`  
		Last Modified: Tue, 29 Nov 2022 04:36:02 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981fce4b7a6f2e0e4fc4961dfb35cd2498ea44579dbd244df96b9790fc07edf2`  
		Last Modified: Tue, 29 Nov 2022 04:36:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc826b3f712bb533f1f8958a0a17d3d3035a5b0551051f2bc2b6eddda2af6913`  
		Last Modified: Tue, 29 Nov 2022 04:36:02 GMT  
		Size: 8.6 KB (8625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b3936c3e5d7097dfb188926dd947f3d74da9f2a7d45ae35aca5e8975cd109b`  
		Last Modified: Tue, 29 Nov 2022 07:02:20 GMT  
		Size: 494.8 KB (494818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40777d9fe6bf4308dc226db071e5c0b86beef42f066e8f82fc2580db3ab8c8ef`  
		Last Modified: Tue, 29 Nov 2022 07:02:19 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64737f589cf24ac8dc81f7e828731ebe9ae488f8bf82c8ccc790fd51524d7724`  
		Last Modified: Tue, 29 Nov 2022 07:02:20 GMT  
		Size: 3.9 MB (3903423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5382a71488f4a18f131127920bc5777a4a97db725ee21ece8a848f997ada52fb`  
		Last Modified: Tue, 29 Nov 2022 07:02:19 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e926f119e44827843839cebc988da130aa30fdc997239fca6ee3f3c7d9c4acd3`  
		Last Modified: Tue, 29 Nov 2022 07:02:20 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:1058f810f5f4e1213432ca069085f9cb1b476af25c04f9a6934a93467949a996
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142598517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc1a9df44d76d4eb9a86ba8b211b6ef506fd43d14cc8bf42b5ee622f0d433e9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 08:47:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 08:47:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 08:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 08:49:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 08:49:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 08:49:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 08:49:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 08:49:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 09:48:08 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 15 Nov 2022 09:48:12 GMT
ENV PHP_VERSION=8.1.12
# Tue, 15 Nov 2022 09:48:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Tue, 15 Nov 2022 09:48:18 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Tue, 15 Nov 2022 09:49:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 09:49:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:30:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 10:30:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:30:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 10:30:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 10:30:50 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 10:30:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 10:30:59 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 10:31:02 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 10:31:06 GMT
CMD ["php-fpm"]
# Wed, 16 Nov 2022 07:29:47 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 16 Nov 2022 07:29:50 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 16 Nov 2022 07:29:53 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 16 Nov 2022 07:29:57 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 16 Nov 2022 07:30:00 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 16 Nov 2022 07:30:03 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 16 Nov 2022 07:30:07 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 16 Nov 2022 07:30:10 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 16 Nov 2022 07:31:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 16 Nov 2022 07:31:20 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 16 Nov 2022 07:31:23 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 16 Nov 2022 07:31:26 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 16 Nov 2022 07:31:30 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 16 Nov 2022 07:31:33 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 16 Nov 2022 07:31:36 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 16 Nov 2022 07:31:45 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 16 Nov 2022 07:31:48 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 16 Nov 2022 07:31:51 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 16 Nov 2022 07:31:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 07:31:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9733c932444d371b8ea79e4a346179de7ebf5cc08e7a02e788c2d964ba318a`  
		Last Modified: Tue, 15 Nov 2022 13:18:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e5bfa08fc491ee443691797985b59230c10d6f4c1684bf69fd790b1e11aba8`  
		Last Modified: Tue, 15 Nov 2022 13:19:28 GMT  
		Size: 71.8 MB (71813700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1c7bd207fbbf8e8defa09a29bafd9e56e40ce0a444494a7ddfd528fa9b303b`  
		Last Modified: Tue, 15 Nov 2022 13:18:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebd19e6481353df8050ebb781e5a61c118749a73ac1f812f8698effb68025a3`  
		Last Modified: Tue, 15 Nov 2022 13:21:27 GMT  
		Size: 11.8 MB (11848499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7201b79a272cb5c3428cbf57406e7a43c5f74056784862590df670d3c990554b`  
		Last Modified: Tue, 15 Nov 2022 13:21:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214ecb67ec686fc1609a24ddcb200b8edbe21d3c78efee7a1b468b83244f8968`  
		Last Modified: Tue, 15 Nov 2022 13:23:19 GMT  
		Size: 25.2 MB (25232252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505937a653d830f570e28992fe336c46471011c112dcb8e177a616f071810699`  
		Last Modified: Tue, 15 Nov 2022 13:23:03 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261ece5b5469078258e315b3140d71204530963cee79b30ac30d59635ac3147`  
		Last Modified: Tue, 15 Nov 2022 13:23:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1a2a7996fa1c0819c574e90a8ecc6809c475be267477ddb744e0688a390614`  
		Last Modified: Tue, 15 Nov 2022 13:23:03 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a79da53150b1f26df764cdbc97c970861278213bd5abcd9c65376df1fcae10`  
		Last Modified: Wed, 16 Nov 2022 07:32:59 GMT  
		Size: 148.9 KB (148948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cb319d632d80a5db81bfebfa5f99bfc0f25500c9b5d2c1d998b00b178f7884`  
		Last Modified: Wed, 16 Nov 2022 07:32:59 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571608ffa22b74104d581deb60a50634431f1bc083e1014dcab8bee5a9c305a0`  
		Last Modified: Wed, 16 Nov 2022 07:33:02 GMT  
		Size: 3.9 MB (3903414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992011ab5b2b88e2e9332fe2d67749bfe9023a49e9ba84451072f35cccf65e34`  
		Last Modified: Wed, 16 Nov 2022 07:32:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7515111d71f1bfc9944327fdc23909e416e6ca5cb8107463b1e6225a185fdf72`  
		Last Modified: Wed, 16 Nov 2022 07:32:59 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:bfd3ea37bc5047c2ee961d37c0ce128054c5d6a70ce28b3363f493ef4c13463a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165341111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c376cf112c517604cd160b39f6fd33ed1099b73bf7490c03a246f3414add1be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:28:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 05:28:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 05:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:29:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 05:29:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 05:29:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 05:29:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 05:29:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 05:47:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 15 Nov 2022 05:47:10 GMT
ENV PHP_VERSION=8.1.12
# Tue, 15 Nov 2022 05:47:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.12.tar.xz.asc
# Tue, 15 Nov 2022 05:47:10 GMT
ENV PHP_SHA256=08243359e2204d842082269eedc15f08d2eca726d0e65b93fb11f4bfc51bbbab
# Tue, 15 Nov 2022 05:47:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 05:47:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:59:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 05:59:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:59:54 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 05:59:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 05:59:55 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 05:59:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 05:59:56 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 05:59:56 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 05:59:57 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 07:57:55 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 15 Nov 2022 07:57:55 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 15 Nov 2022 07:57:55 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 15 Nov 2022 07:57:56 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 15 Nov 2022 07:57:56 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 15 Nov 2022 07:57:56 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 15 Nov 2022 07:57:57 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 15 Nov 2022 07:57:57 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 15 Nov 2022 07:58:28 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 15 Nov 2022 07:58:30 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 07:58:30 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 15 Nov 2022 07:58:30 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 15 Nov 2022 07:58:31 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 15 Nov 2022 07:58:31 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 15 Nov 2022 07:58:31 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 15 Nov 2022 07:58:34 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 15 Nov 2022 07:58:35 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 15 Nov 2022 07:58:35 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 15 Nov 2022 07:58:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 07:58:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f0beaf56e20c42dc99adac83339859a68fe21121e2a97694ccf17bb3d80a1f`  
		Last Modified: Tue, 15 Nov 2022 07:02:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb01e5ff921e5a6fdfd50966abf1a71511e1fc3d7c5b93c0f0d23c4b01bde8ad`  
		Last Modified: Tue, 15 Nov 2022 07:03:05 GMT  
		Size: 86.6 MB (86632107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b444ab201aca26c541ce9ce4732f100ccd2fd815497509f4281f39038ecdb838`  
		Last Modified: Tue, 15 Nov 2022 07:02:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e1f0311ac81df52ad5f37ebb74dcc20309a2e3fe975fda1387256083346232`  
		Last Modified: Tue, 15 Nov 2022 07:05:10 GMT  
		Size: 12.1 MB (12066480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7223bcdaa6c5abbee309fa14102a182f563a066082d6eb131e1ba55df838a96`  
		Last Modified: Tue, 15 Nov 2022 07:05:08 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ff8388c049fe1ca00a2197bd55b6e4d316972bd7a621c8625dfe51d8c9450`  
		Last Modified: Tue, 15 Nov 2022 07:07:00 GMT  
		Size: 27.3 MB (27253868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095937361c0d87ef5f7bb9c4fcb87b687ec39fca6fe8ad459699f167ed386ce`  
		Last Modified: Tue, 15 Nov 2022 07:06:54 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49719abb2dbf9f85a53323780d682d4f163530d1a8cf5960ecfefbb8258bf236`  
		Last Modified: Tue, 15 Nov 2022 07:06:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebe7c1c4e76968995ce61848ccf96d600b3370c5cf6b538c5a5c67f020d6689`  
		Last Modified: Tue, 15 Nov 2022 07:06:54 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc49705b5291c1103e3f1bc73a5cd934be81082736784296489da85f154c0f6e`  
		Last Modified: Tue, 15 Nov 2022 08:00:08 GMT  
		Size: 183.7 KB (183740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055d1f541f1f2ea0a7553c8400d363da9609ec3482928d12fde789459e7302c0`  
		Last Modified: Tue, 15 Nov 2022 08:00:08 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68276017a01d2dc564e024c14a7f804a99440066ea118333e0f1930e65236ef8`  
		Last Modified: Tue, 15 Nov 2022 08:00:09 GMT  
		Size: 3.9 MB (3903530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e518424c51cdd276a1a63d8ee11eca7aa876f33f1ede8f7d6f15d696116043b`  
		Last Modified: Tue, 15 Nov 2022 08:00:08 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c785ef6214cbdb7b9a2d38f67752e0f95e7a668110f18bf429cca9141684950`  
		Last Modified: Tue, 15 Nov 2022 08:00:08 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; s390x

```console
$ docker pull yourls@sha256:1b235f0d7c5226b3a5fd07d2beb77ff6a9750a7230466112e40cdc73c920b8f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142757870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1117e6a84e9624adfd74e68b25072420d5ad39c45b1645a7bcabdb912396a981`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 02:57:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 02:57:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 02:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:58:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 02:58:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 02:58:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:58:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:58:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 03:15:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:21:34 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:21:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:21:34 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:21:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:21:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:28:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:28:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:28:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:28:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:28:13 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:28:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Nov 2022 02:28:14 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Nov 2022 02:28:14 GMT
EXPOSE 9000
# Tue, 29 Nov 2022 02:28:14 GMT
CMD ["php-fpm"]
# Tue, 29 Nov 2022 05:56:52 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 29 Nov 2022 05:56:52 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 29 Nov 2022 05:56:52 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 29 Nov 2022 05:56:52 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 29 Nov 2022 05:56:53 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 29 Nov 2022 05:56:53 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 29 Nov 2022 05:56:53 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 29 Nov 2022 05:56:53 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 29 Nov 2022 05:57:06 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 29 Nov 2022 05:57:07 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Nov 2022 05:57:07 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 05:57:07 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 05:57:07 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 29 Nov 2022 05:57:08 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 29 Nov 2022 05:57:08 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 29 Nov 2022 05:57:10 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 29 Nov 2022 05:57:10 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 29 Nov 2022 05:57:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 29 Nov 2022 05:57:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 05:57:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71958e28a746867b0e7cb1c5f031924597b4509a233399a3a3d8968aa95f64`  
		Last Modified: Tue, 15 Nov 2022 04:44:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b409c9c2463a7e5350cae36b1e7fba6df50cfa44e169bb26a643cd299143e`  
		Last Modified: Tue, 15 Nov 2022 04:45:04 GMT  
		Size: 71.6 MB (71627303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f25a893502757c2fbf006d5887bcc16766dc523c4cac685c2dccf4af8a0ecb7`  
		Last Modified: Tue, 15 Nov 2022 04:44:53 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dcc30ad5f3c7b2edf3a3729344b4d7089ccee2cf652d94c36207bd9783b9af`  
		Last Modified: Tue, 29 Nov 2022 03:27:45 GMT  
		Size: 12.1 MB (12121890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941ab273b5194e4b08ccba2f3a871c9c48218fff45227a5a0bed456fdd5fc199`  
		Last Modified: Tue, 29 Nov 2022 03:27:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be094aa73110009080d06c7664bc0291ad08d2b48db99dfe55548534ec6fe0a`  
		Last Modified: Tue, 29 Nov 2022 03:28:46 GMT  
		Size: 25.3 MB (25286922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1720a3adb741f4b89e33a2bd6c1666bcaf1d13cf9dc69638fa4d645de2e7c41e`  
		Last Modified: Tue, 29 Nov 2022 03:28:43 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dc84616f2adc711459bdba9cb758372c031e0841e83b123ecc8268f28bc926`  
		Last Modified: Tue, 29 Nov 2022 03:28:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff526c7e4cb51bb137ce5bc06d5ef0548b444878a163c3b0dd440e919e0b90e`  
		Last Modified: Tue, 29 Nov 2022 03:28:43 GMT  
		Size: 8.6 KB (8626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61ae6f35b53c2bbc09ec7491f874bb4595e1f5b2f07b242e8632291d581c8bc`  
		Last Modified: Tue, 29 Nov 2022 05:58:42 GMT  
		Size: 158.2 KB (158193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d409a9c04ccf015c040b6fea3e244a34fedc3809d25e24387578fd6a94f59d9`  
		Last Modified: Tue, 29 Nov 2022 05:58:42 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb8ebaa97c860ffdbb2e5f0027b6f805e0ad130639120fff773ced00a6ee7fa`  
		Last Modified: Tue, 29 Nov 2022 05:58:43 GMT  
		Size: 3.9 MB (3903530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e914ef6a4e16a770cd58dcfeb0653f5366f2db861cd929312c53bde8b68097`  
		Last Modified: Tue, 29 Nov 2022 05:58:42 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bede7e67c1b961f8ff196e4454c6abf9313c9528b02b11118804d8b37a261f`  
		Last Modified: Tue, 29 Nov 2022 05:58:42 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
