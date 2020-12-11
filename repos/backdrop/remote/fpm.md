## `backdrop:fpm`

```console
$ docker pull backdrop@sha256:62f8233b37663cc275d3473001e98d8f85e6ba069144c94833bf07b0228c2a77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:7d4a2a2cbcf4dea069af67b02f6672a788c1b9e070e7537961eff87cad7945ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156117992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fc4372f2dae97b16824720a6200decbe32bc831d4f26e5747906826625b4f9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 07:15:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 07:15:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 07:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 07:16:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 07:16:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 07:35:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 07:35:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:35:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:35:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 10:52:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 11 Dec 2020 10:52:15 GMT
ENV PHP_VERSION=7.2.34
# Fri, 11 Dec 2020 10:52:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Fri, 11 Dec 2020 10:52:16 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903
# Fri, 11 Dec 2020 10:52:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 10:52:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:57:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 10:57:49 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:57:50 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 10:57:51 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 11 Dec 2020 10:57:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 10:57:52 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 10:57:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 10:57:53 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 10:57:53 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 10:57:53 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 22:55:18 GMT
RUN apt-get update && apt-get install -y libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 11 Dec 2020 22:55:18 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 22:55:18 GMT
ENV BACKDROP_VERSION=1.17.3
# Fri, 11 Dec 2020 22:55:18 GMT
ENV BACKDROP_MD5=907ae2978936d525626dd4c981afd0d2
# Fri, 11 Dec 2020 22:55:22 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 11 Dec 2020 22:55:23 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 11 Dec 2020 22:55:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 22:55:23 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db606474d60ce31604505c7d6dad9a66cb42f3818fca738832db2f2091cf89c9`  
		Last Modified: Fri, 11 Dec 2020 12:04:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb30f0cd8e0ff78b5eecdc2d9365a50441ad83c5db5f1e87942d6426237fa56`  
		Last Modified: Fri, 11 Dec 2020 12:04:17 GMT  
		Size: 76.7 MB (76652169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2e805159413e5278b859f7fbb86ddfc99e667cb705d5d5aec0a7c8ffcf1b5`  
		Last Modified: Fri, 11 Dec 2020 12:04:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d71313b39b0bf6a31d8ac0081687e1b68045d1f268a1c991ad7973078ee68bd`  
		Last Modified: Fri, 11 Dec 2020 12:12:42 GMT  
		Size: 12.6 MB (12631759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381de550657f80e39c092c9359d094862a0d9c04d20651b8d26ef289b0b0bd1f`  
		Last Modified: Fri, 11 Dec 2020 12:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e671c4250cc8ce3fedc7f6d1bdc28d810432776ba87ffab3c1ba639836a461ce`  
		Last Modified: Fri, 11 Dec 2020 12:12:46 GMT  
		Size: 28.5 MB (28532397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111da53eb201f96a019a6aeb54581a70b3a3d882aa0f2b1662f3bbeb5f588312`  
		Last Modified: Fri, 11 Dec 2020 12:12:39 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e126978923725af4cb0ce0e656dbfc52217de49e18888b59b2e9363755db9232`  
		Last Modified: Fri, 11 Dec 2020 12:12:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0540b5ed3310ea4b4b7da080fd41498df528f2828559e67e14a0c80d0aeff768`  
		Last Modified: Fri, 11 Dec 2020 12:12:39 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0461cc2270a717d486d5955182d7bff374347d50b91d62de7c57ed045c5ea749`  
		Last Modified: Fri, 11 Dec 2020 12:12:39 GMT  
		Size: 7.8 KB (7789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c7b64b4b82fcfaef48d922736339e9355556a65d3489adf098b4a4d83ca7ba`  
		Last Modified: Fri, 11 Dec 2020 22:55:57 GMT  
		Size: 2.6 MB (2576173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb93223881ff0af667632f6ad582a57cd375bac131557e3313889c4b2f7ce0e`  
		Last Modified: Fri, 11 Dec 2020 22:56:01 GMT  
		Size: 8.6 MB (8613798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a7a1e2e37d703414068cd9896b39dc494c2b84ebf7165038b6037d66be1b2`  
		Last Modified: Fri, 11 Dec 2020 22:55:57 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:0330bef0d29d31d8bd846b3c2afcf1d913e5ff388a7fc6dd0bb37919bc615446
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.2 MB (148204568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb7766a64ebea12814384c1f51d3eeb66a4206fe6a5fb6b357f8bf853c93c61`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 18 Nov 2020 04:09:39 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 18 Nov 2020 04:09:41 GMT
ENV PHP_VERSION=7.2.34
# Wed, 18 Nov 2020 04:09:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Wed, 18 Nov 2020 04:09:44 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903
# Wed, 18 Nov 2020 04:10:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 04:10:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 04:13:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 04:14:01 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 04:14:03 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 04:14:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 18 Nov 2020 04:14:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 04:14:07 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 04:14:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 04:14:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 04:14:10 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 04:14:11 GMT
CMD ["php-fpm"]
# Thu, 19 Nov 2020 01:09:32 GMT
RUN apt-get update && apt-get install -y libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 19 Nov 2020 01:09:33 GMT
WORKDIR /var/www/html
# Thu, 19 Nov 2020 04:50:26 GMT
ENV BACKDROP_VERSION=1.17.3
# Thu, 19 Nov 2020 04:50:28 GMT
ENV BACKDROP_MD5=907ae2978936d525626dd4c981afd0d2
# Thu, 19 Nov 2020 04:50:41 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Thu, 19 Nov 2020 04:50:45 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 19 Nov 2020 04:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 04:50:48 GMT
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
	-	`sha256:570b62dc7f75c248e5abbb97a4f53f56969ed3665fd126bf892e5f0c810cc533`  
		Last Modified: Wed, 18 Nov 2020 04:44:41 GMT  
		Size: 12.6 MB (12630735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d623c724e8e90f66d2c38383ef0df967fcf45cc915bc317665a7d3828513e649`  
		Last Modified: Wed, 18 Nov 2020 04:44:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fffc7c3b8c54152614bd63d38342ac8ee361d883d5e0b98b15d46016d103a36`  
		Last Modified: Wed, 18 Nov 2020 04:44:45 GMT  
		Size: 28.2 MB (28204635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8504af707e302ab63e65814faf1ecbdd30807bfe95ee9ad831fb1f850b1f1ad`  
		Last Modified: Wed, 18 Nov 2020 04:44:37 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d508657fb41ce20d30d8251a5bf776ffe6dee18c123b9876fb6ba2a6e1bfd52`  
		Last Modified: Wed, 18 Nov 2020 04:44:37 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788248d581c2e19df6f62236f354ee0f28d73113a6d41269ed145f234ed8e362`  
		Last Modified: Wed, 18 Nov 2020 04:44:38 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2039432341c451f51d9cbaf3261740afc65d815d15d4ae36a5ea9564517b8126`  
		Last Modified: Wed, 18 Nov 2020 04:44:37 GMT  
		Size: 7.8 KB (7787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fd9fa01fe163ca75704f9a23f640212f3cf2a11121918654544c5fee9c5081`  
		Last Modified: Thu, 19 Nov 2020 01:10:24 GMT  
		Size: 2.5 MB (2542392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f7b1938d10f8d32f250bf032242d7ab4fce93b67f36ca85742ff5f67e16d59`  
		Last Modified: Thu, 19 Nov 2020 04:51:28 GMT  
		Size: 8.6 MB (8614189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42fd6f0050c535d60144583f2e56bfb91c5ce1cd46f564a1ae827b1d7c7fb3c`  
		Last Modified: Thu, 19 Nov 2020 04:51:25 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
