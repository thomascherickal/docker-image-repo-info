## `php:rc-zts`

```console
$ docker pull php@sha256:59dc5fab28b2516329efabe8e2301a43a0b06044867878f370f7084b9c055cf7
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

### `php:rc-zts` - linux; amd64

```console
$ docker pull php@sha256:833ffca52ea38443c87f02c9e9668eb691f62da080995076c6a50a80151b16da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139885492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e174c26c6d0b063593806db4726d5c0fadd0665b9ab50f74a2189d25c96b86`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 09:12:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 09:12:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 09:12:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 09:12:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 09:12:22 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 19 Nov 2020 19:53:08 GMT
ENV PHP_VERSION=8.0.0RC5
# Thu, 19 Nov 2020 19:53:08 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz.asc
# Thu, 19 Nov 2020 19:53:09 GMT
ENV PHP_SHA256=fa2e98d8b42e497a45f491c4714f0a67f7d817ff2f7ab9aad09efb72d2a8c60b
# Thu, 19 Nov 2020 19:53:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 19:53:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Nov 2020 19:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 19 Nov 2020 19:59:42 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 19 Nov 2020 19:59:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Nov 2020 19:59:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Nov 2020 19:59:43 GMT
CMD ["php" "-a"]
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
	-	`sha256:530eab7002c20071c100d6653abd4a70abc1855562909936a6335df39a4911c7`  
		Last Modified: Thu, 19 Nov 2020 20:27:31 GMT  
		Size: 10.9 MB (10949258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2ac33a15b98e046f1ce88dbeac8581c5f0db1dff8395f65415b7cdf521d43a`  
		Last Modified: Thu, 19 Nov 2020 20:27:29 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e502a359403e2fc395d10bac11f903efdd5419083e3e89be211a0d819ec497`  
		Last Modified: Thu, 19 Nov 2020 20:27:35 GMT  
		Size: 25.2 MB (25174890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f619f1670c440fedd8801785d7d6c95027891d495289d780496f07ca1041c59`  
		Last Modified: Thu, 19 Nov 2020 20:27:29 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4294e762545833d97f8fd712520ad4566a75f014fabbeaae95e15b2da9705d`  
		Last Modified: Thu, 19 Nov 2020 20:27:29 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; arm variant v5

```console
$ docker pull php@sha256:566c2ba069b48cb9c62f28dfa90a26b9243b895a31ba33f400da64298503effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118468746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:465454aecc178452218f4325b2ef12cbe0ec1d042490dda2f95b09fa438395e2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 01:33:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 01:33:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 01:33:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 01:33:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 01:33:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 19 Nov 2020 20:46:35 GMT
ENV PHP_VERSION=8.0.0RC5
# Thu, 19 Nov 2020 20:46:37 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz.asc
# Thu, 19 Nov 2020 20:46:41 GMT
ENV PHP_SHA256=fa2e98d8b42e497a45f491c4714f0a67f7d817ff2f7ab9aad09efb72d2a8c60b
# Thu, 19 Nov 2020 20:47:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 20:47:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Nov 2020 20:52:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 19 Nov 2020 20:52:12 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 19 Nov 2020 20:52:22 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Nov 2020 20:52:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Nov 2020 20:52:31 GMT
CMD ["php" "-a"]
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
	-	`sha256:2a713d099e930e14c98177ea894d0ee41b29ece3a12d2c036fa6b11b64a15d60`  
		Last Modified: Thu, 19 Nov 2020 20:57:12 GMT  
		Size: 10.9 MB (10947439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d26654bd8e6e135ecde2109b1ddc6c7f1bc9717ffaa2bb589051b0937b4d24`  
		Last Modified: Thu, 19 Nov 2020 20:57:11 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ea28aa96402ec35822c61466355d0bdec36f541e4252993737e0591319b2a`  
		Last Modified: Thu, 19 Nov 2020 20:57:17 GMT  
		Size: 23.9 MB (23866376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70f7f4aeefed5848134abd194716d25bcba7b6a501d2ae1c85742f86dd72e2a`  
		Last Modified: Thu, 19 Nov 2020 20:57:10 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf03c964e8b730ee7bfc8402c393c409ffb1802842ef46f552ce61962c59bf77`  
		Last Modified: Thu, 19 Nov 2020 20:57:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; arm variant v7

```console
$ docker pull php@sha256:3facd9ea3e35e1a282cd25a83168f87d845821801d058ff365f67eca6c618e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116221368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586a062d6f41ce74e997f9c66775797ddd453126d3742e76d12a138b8726e59f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 00:00:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 00:00:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 00:00:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 00:00:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 00:00:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 18 Nov 2020 00:00:11 GMT
ENV PHP_VERSION=8.0.0RC4
# Wed, 18 Nov 2020 00:00:12 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz.asc
# Wed, 18 Nov 2020 00:00:13 GMT
ENV PHP_SHA256=b6bd9cc1859e15de85c44d207e7a3d2fcc4ec4ed987e7b15346b89d96066db4f
# Wed, 18 Nov 2020 00:00:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 00:00:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 00:03:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Wed, 18 Nov 2020 00:03:21 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Wed, 18 Nov 2020 00:03:24 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 00:03:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 00:03:26 GMT
CMD ["php" "-a"]
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
	-	`sha256:0865a573510bc8f3bfad9cb6da7e6d7c13c03b97f5705e52d04a79e92d0a1004`  
		Last Modified: Wed, 18 Nov 2020 01:35:54 GMT  
		Size: 10.9 MB (10943357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3cfced3dccdf29d44806e0034944e4ec7cf43d985fad7979ba961805358ef8`  
		Last Modified: Wed, 18 Nov 2020 01:35:52 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd723ff8c5f5e57756b35fa3ecc7cee0c8a419163e1206d5e38f911a892ca3b`  
		Last Modified: Wed, 18 Nov 2020 01:35:59 GMT  
		Size: 23.1 MB (23052536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ed4072ebdab2d962e91f080760ca9e6f9b61046697a45bba971f2335db5eb5`  
		Last Modified: Wed, 18 Nov 2020 01:35:52 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62266caa8c858508722421e5ad34581955b9908659d0642b33c1cf5e5b61f5c`  
		Last Modified: Wed, 18 Nov 2020 01:35:52 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; arm64 variant v8

```console
$ docker pull php@sha256:593c1c35f8a2af346623ab553c5e7f6b4194204d9bd48336ac22c2bd1bd70beb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131853731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbbea0f47d1c866776dd6a1ce5ced0cad0d66b6ba2636add2ccb5ba2d9a8879`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 03:08:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 03:08:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:08:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 03:08:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 18 Nov 2020 03:08:42 GMT
ENV PHP_VERSION=8.0.0RC4
# Wed, 18 Nov 2020 03:08:42 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz.asc
# Wed, 18 Nov 2020 03:08:43 GMT
ENV PHP_SHA256=b6bd9cc1859e15de85c44d207e7a3d2fcc4ec4ed987e7b15346b89d96066db4f
# Wed, 18 Nov 2020 03:08:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 03:08:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 03:11:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Wed, 18 Nov 2020 03:12:02 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Wed, 18 Nov 2020 03:12:04 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 03:12:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 03:12:06 GMT
CMD ["php" "-a"]
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
	-	`sha256:3eb0e876498f3e3bca1b33734c32e9a0403220fb159cb245071e0f7171390f33`  
		Last Modified: Wed, 18 Nov 2020 04:38:47 GMT  
		Size: 10.9 MB (10944162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c0ee12206d1797501a25360a8bb7f0642d8cc20a9c59e1ddeb77b12003b189`  
		Last Modified: Wed, 18 Nov 2020 04:38:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc96b6c3bf6ba9549930b96232f8645dbe16997ba2421fbe8f2aa1078fdd106`  
		Last Modified: Wed, 18 Nov 2020 04:38:52 GMT  
		Size: 24.7 MB (24705897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425f745001f0688665e08891ae3363de1d344fadc6754980643c59a6e4a796f`  
		Last Modified: Wed, 18 Nov 2020 04:38:46 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb571f0c2101eb5a9772f9b93e82a92fef025cfa59aa43c18eb3b9847b07d825`  
		Last Modified: Wed, 18 Nov 2020 04:38:46 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; 386

```console
$ docker pull php@sha256:33765737dd721eb30f7cb03eecc499cbfd7990404d9a5f279a58c22d696ef665
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.3 MB (145262626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:431629460299fd9179df60e486aaef0bf1c78d82a83890d5bf244fcd9e9c431d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 03:52:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 03:52:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:52:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:52:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 03:52:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 19 Nov 2020 20:25:34 GMT
ENV PHP_VERSION=8.0.0RC5
# Thu, 19 Nov 2020 20:25:34 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz.asc
# Thu, 19 Nov 2020 20:25:35 GMT
ENV PHP_SHA256=fa2e98d8b42e497a45f491c4714f0a67f7d817ff2f7ab9aad09efb72d2a8c60b
# Thu, 19 Nov 2020 20:25:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 20:25:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Nov 2020 20:31:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 19 Nov 2020 20:31:37 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 19 Nov 2020 20:31:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Nov 2020 20:31:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Nov 2020 20:31:38 GMT
CMD ["php" "-a"]
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
	-	`sha256:aed86adbf4241f15aafd9dd936a78334b429c552dc1d0cc2be5d07e851d90f2d`  
		Last Modified: Thu, 19 Nov 2020 20:51:46 GMT  
		Size: 10.9 MB (10948525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad59dbc291f18d38c73109caa51168226b2ce1d5c27af5ee8bb1083f382d398`  
		Last Modified: Thu, 19 Nov 2020 20:51:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa22d345ce34325d754721471331d3cf7fd5b0e5d18036e80215581fff15319`  
		Last Modified: Thu, 19 Nov 2020 20:51:53 GMT  
		Size: 25.3 MB (25348553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b57e77f50de20183f1527aed66b7fb6001139a97cf70e475de7c03ab50b22ff`  
		Last Modified: Thu, 19 Nov 2020 20:51:45 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fcfc8f9a081ab0d1d97b54180800f7bb6738df8ff16ade808cd056fa6a8f57`  
		Last Modified: Thu, 19 Nov 2020 20:51:45 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; mips64le

```console
$ docker pull php@sha256:ec36de23ff339a166e5405ada9a8a30cd6518c084beb841a5dda2f6f57d5819b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122532962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85522e6da57cefddd12aaf99353e5540a7c8f2de3ba02914dd7e3cb36498461e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 07:55:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 07:55:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 07:55:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 07:55:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 07:55:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 19 Nov 2020 19:46:15 GMT
ENV PHP_VERSION=8.0.0RC5
# Thu, 19 Nov 2020 19:46:15 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC5.tar.xz.asc
# Thu, 19 Nov 2020 19:46:15 GMT
ENV PHP_SHA256=fa2e98d8b42e497a45f491c4714f0a67f7d817ff2f7ab9aad09efb72d2a8c60b
# Thu, 19 Nov 2020 19:46:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 19:46:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Nov 2020 19:59:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 19 Nov 2020 19:59:27 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 19 Nov 2020 19:59:29 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Nov 2020 19:59:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Nov 2020 19:59:29 GMT
CMD ["php" "-a"]
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
	-	`sha256:f04f2497f73e4353ec979d75a44a1c3a3c326228507fa902226468083505a693`  
		Last Modified: Thu, 19 Nov 2020 20:06:42 GMT  
		Size: 10.9 MB (10946539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55630c4f1691f5bae1d5d74f974f2283e67193e09a72867fa40b6375876e245e`  
		Last Modified: Thu, 19 Nov 2020 20:06:39 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3157147298380249fd4750fe12c2409a5f32cd6b2c1f898a9374299b6ccb89`  
		Last Modified: Thu, 19 Nov 2020 20:06:56 GMT  
		Size: 24.4 MB (24416729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79e53b3f4569307b0d7b25342b0e5ee32c54acc28324a922972b6adbde7260e`  
		Last Modified: Thu, 19 Nov 2020 20:06:39 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc8a2de3d32ae85248e902a5468172002486c2dcbc39b4c263e63c691fdbfa`  
		Last Modified: Thu, 19 Nov 2020 20:06:39 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; ppc64le

```console
$ docker pull php@sha256:13b5816809387129d673f0150ca2e15c94d9ee9efbc19570964ebae8300d233e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.0 MB (149976234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e925599f138fc824d456d7f56de36c234edd18c6d4d8ae2b90f67367a4482cee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Wed, 18 Nov 2020 13:57:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Wed, 18 Nov 2020 13:57:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 13:57:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 13:57:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 13:58:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 18 Nov 2020 13:58:09 GMT
ENV PHP_VERSION=8.0.0RC4
# Wed, 18 Nov 2020 13:58:12 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz.asc
# Wed, 18 Nov 2020 13:58:16 GMT
ENV PHP_SHA256=b6bd9cc1859e15de85c44d207e7a3d2fcc4ec4ed987e7b15346b89d96066db4f
# Wed, 18 Nov 2020 14:01:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 14:01:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 14:06:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Wed, 18 Nov 2020 14:06:38 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Wed, 18 Nov 2020 14:06:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 14:06:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 14:06:59 GMT
CMD ["php" "-a"]
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
	-	`sha256:96e7073873813c5775f6cbfc9b1258b8f7537a901ab43d2bd428e2541677d91e`  
		Last Modified: Wed, 18 Nov 2020 15:48:52 GMT  
		Size: 10.9 MB (10945244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac0d1c5789f044eb503eb8fe97646b8e6d8f3d8f54f63735309463d36fd5b0b`  
		Last Modified: Wed, 18 Nov 2020 15:48:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cdb881e5c3f7c8b3962cfb7678e388487612fd567989024b261f05e5bb42a5`  
		Last Modified: Wed, 18 Nov 2020 15:48:56 GMT  
		Size: 26.2 MB (26236301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286238695251ccd53c012e50055c6eb8fcc88d8f752d52bd9e9b423ae319469`  
		Last Modified: Wed, 18 Nov 2020 15:48:51 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8993627f7bdf27cdf2ac810d83bebc340bd4aa7ecdead23803d2309ee2bef120`  
		Last Modified: Wed, 18 Nov 2020 15:48:51 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-zts` - linux; s390x

```console
$ docker pull php@sha256:1b3c912b561608a08b5c83d78a3bbb33cd775eddca07d1593bd8fda5c3074db4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125646787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b1b7e99bea41c9bd14383db73c85f83ee5168690e4c22d1b140a4c2c5be59`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:05:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Nov 2020 22:05:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Nov 2020 22:06:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:06:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Nov 2020 22:06:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Nov 2020 22:28:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Nov 2020 22:28:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 22:28:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 22:28:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Nov 2020 22:28:20 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Nov 2020 22:28:21 GMT
ENV PHP_VERSION=8.0.0RC4
# Tue, 17 Nov 2020 22:28:22 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0RC4.tar.xz.asc
# Tue, 17 Nov 2020 22:28:23 GMT
ENV PHP_SHA256=b6bd9cc1859e15de85c44d207e7a3d2fcc4ec4ed987e7b15346b89d96066db4f
# Tue, 17 Nov 2020 22:28:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Nov 2020 22:28:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:34:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Tue, 17 Nov 2020 22:34:43 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:34:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Nov 2020 22:34:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Nov 2020 22:34:47 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee323c0bdcb822c2cb3d1bd93141d6d29b8940a6180a88839cd68c80fbd106c2`  
		Last Modified: Wed, 18 Nov 2020 00:07:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec8f1576a5517595c8a7a530526f62d922496f66584f9dbd8e4d72690c136ad`  
		Last Modified: Wed, 18 Nov 2020 00:07:28 GMT  
		Size: 64.7 MB (64706676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9ccf205c352e00231140d9f5c3f826695eb3a553ccbd4ffd9cfbee2b8411f`  
		Last Modified: Wed, 18 Nov 2020 00:07:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dee3934d7e44836cef46466cf954e61781501e7c98eae94b81afc90df3a4e15`  
		Last Modified: Wed, 18 Nov 2020 00:08:36 GMT  
		Size: 10.9 MB (10943731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dad34f57e425b670a5022f6abf41fdc4dbfc833f3190d84d92046ae56e1ce7`  
		Last Modified: Wed, 18 Nov 2020 00:08:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3beaf03ca14c34e22bca50c14783ba4da52625bc9e7a0be0afd836466897e2`  
		Last Modified: Wed, 18 Nov 2020 00:08:39 GMT  
		Size: 24.3 MB (24271737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d53a092700f2e1a41140078964d24b3ed0653096d26f967d849660a633455`  
		Last Modified: Wed, 18 Nov 2020 00:08:34 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e50eddb359fda358a7c4668fb57df1d23dcdbfa302f93e58182ee826492e8`  
		Last Modified: Wed, 18 Nov 2020 00:08:35 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
