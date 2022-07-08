## `php:8-zts-bullseye`

```console
$ docker pull php@sha256:cda61b044b79ce4774a4265d0bdd5236b40baa08d0601b1abb18723092e9831d
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

### `php:8-zts-bullseye` - linux; amd64

```console
$ docker pull php@sha256:bd7fcfc51bf01f1cb0704d2e5a05802965cb29cb22dfc5f0a511da818e4ea80c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.4 MB (163412347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac416051fdf0d6568767be224de6d20087fc6090e780aab8a401fe9f3804f8b5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 07:22:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 07:22:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 07:22:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 07:22:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 07:22:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 07:22:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 07:22:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 07:22:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 07:49:02 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:17:24 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:17:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:17:24 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:17:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:17:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:31:13 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:31:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:31:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:31:14 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fdfd2598e0ffdaa39011b909e2a79a75a60a0a87998f1072ec5d9256f19868`  
		Last Modified: Thu, 23 Jun 2022 09:03:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26769c8659f467675c0f34948c16e051ea7aab69ec3198c65063c299b9771a05`  
		Last Modified: Thu, 23 Jun 2022 09:04:05 GMT  
		Size: 91.6 MB (91603711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd105fadbe34a7e12eb66c424bd0de4b9c2c5c2daf01063eef044ff10e5e437`  
		Last Modified: Thu, 23 Jun 2022 09:03:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d425b2b4fa0fec78c0afdd0893888871ae48799f1da08f4d93d22922e94ffa`  
		Last Modified: Fri, 08 Jul 2022 00:11:29 GMT  
		Size: 12.3 MB (12274138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2b86cc115e2483be9d4d34577b41e9642953c23811df483c888d691f47a434`  
		Last Modified: Fri, 08 Jul 2022 00:11:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12fa4dfcbc89748527e6c40b9783e61a819433c5ea3de3dd7a5522dc03a2a47`  
		Last Modified: Fri, 08 Jul 2022 00:13:30 GMT  
		Size: 28.2 MB (28151402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac70a0aa745b2fa36b849324d689627818f6334215a2021caefeb961f34667`  
		Last Modified: Fri, 08 Jul 2022 00:13:25 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436910c9914ef704f02a3ce6641be50bace0d8d78c25ad8b61d2fbf02f8f5246`  
		Last Modified: Fri, 08 Jul 2022 00:13:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; arm variant v5

```console
$ docker pull php@sha256:65e58839e2e299ced174e8ecff58b1656a6eb858344b096ac42acb0fd4b51e60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141412832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6405f3e1bdf0edcfc2372d59f5484b8c05ff8247e20e79f71c6c0c5bbbcbf91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 23:35:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 23:35:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 23:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 23:36:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 23:36:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 23:36:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 23:36:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 23:36:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Jun 2022 00:23:23 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 21:37:50 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 21:37:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 21:37:51 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 21:38:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 21:38:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:00:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:00:36 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:00:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:00:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:00:38 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e09f88f3062c4ac137aceba98450d079bdce7152b5329623464a6542325584`  
		Last Modified: Fri, 24 Jun 2022 04:17:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe814f0e772803c6ff5bfa73308b751c597dd457ec3c64cd244b3ae64d384ce`  
		Last Modified: Fri, 24 Jun 2022 04:18:27 GMT  
		Size: 73.7 MB (73685507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b36f773d9748a4a3dd653209f9309cf65790c131a8f74000a5c238b404656fc`  
		Last Modified: Fri, 24 Jun 2022 04:17:37 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5f7d9d192d7314a43dfbd133212ac2c777630bcf14d5ade26ee0a59bf4e5f9`  
		Last Modified: Thu, 07 Jul 2022 23:31:23 GMT  
		Size: 12.3 MB (12257884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89352987c434e6b35ca185649fde7c786ad787173e9f2c6ef20c2cc84ece14a2`  
		Last Modified: Thu, 07 Jul 2022 23:31:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567b3235a94ab300107a9efa76a5ef5e88856a692654587bd287ddb16504298`  
		Last Modified: Thu, 07 Jul 2022 23:34:44 GMT  
		Size: 26.5 MB (26544201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64813936bf26c5facd54ea27392d05a449012a9561945582a00f946dd25c05e`  
		Last Modified: Thu, 07 Jul 2022 23:34:28 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d40e0b17f25bbc02fbaeca2e5c4bed68f4c7521be4f48d25a4fa05f8add2ca`  
		Last Modified: Thu, 07 Jul 2022 23:34:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; arm variant v7

```console
$ docker pull php@sha256:d6624f84bef182bca86895c15cf90f34162eb819852591b9f26f1151101f5e2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133731366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61171c77fb92bc26fb62ddc2cd6d83bc1c97a8cf0bb61ce9df992c8696b01bb8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:12:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 13:12:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 13:13:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:13:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 13:13:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 13:13:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:13:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:13:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 13:56:05 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:14:24 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:14:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:14:25 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:14:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:14:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:36:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:36:33 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:36:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:36:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:36:36 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23fbd5354dced767ae1b15eb7910f2d11403b9f411ecda74c37c1f1876fc3c9`  
		Last Modified: Thu, 23 Jun 2022 16:18:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d1a1cf7d4658893bc3638769043fcfd521db95f086c1a37d4397c7a843c780`  
		Last Modified: Thu, 23 Jun 2022 16:18:50 GMT  
		Size: 69.3 MB (69319118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcb3f8e4edb07e8f7231fa39923f2ff418333f8e22e3d61de7f525394de026e`  
		Last Modified: Thu, 23 Jun 2022 16:18:07 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b0dc956de1cfc4367cd9439e79c7cd6dc17c143e30c07a7c5805d76da2ab9f`  
		Last Modified: Fri, 08 Jul 2022 01:07:54 GMT  
		Size: 12.2 MB (12234205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8242cd1dcd1bbdee516a5d0385268b7b138afaa505d70cdd65de8a72eab8fe`  
		Last Modified: Fri, 08 Jul 2022 01:07:51 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690392a7b4156cc1a8c0d8a387271cccd002c6b86b4ae0449ba026fe7fecd50b`  
		Last Modified: Fri, 08 Jul 2022 01:11:13 GMT  
		Size: 25.6 MB (25598246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a8def12fb0d055d7097b3124b17b2f55f7d5c3b0f870e52fce7294afbd8f2c`  
		Last Modified: Fri, 08 Jul 2022 01:10:58 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32f291158fe26faed730eb30a6474eb2d8fd13f4fddce59f1ff885075010a5`  
		Last Modified: Fri, 08 Jul 2022 01:10:59 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; arm64 variant v8

```console
$ docker pull php@sha256:92139818fbc364462ddc8e1951c08302c833d0dc819a9df803eec099a5eac4ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156935153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5449d287592528f566d3c8344f2bb13414a7b2b356a6bd3e3fa15d936561b93`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:31:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 07:04:51 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 21:54:24 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 21:54:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 21:54:25 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 21:54:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 21:54:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:10:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:10:12 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:10:13 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:10:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:10:14 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c46306a633482421e7613b18cbb6c9317a1b99cb75b58c9f5c736ad195477b`  
		Last Modified: Fri, 08 Jul 2022 00:02:18 GMT  
		Size: 12.1 MB (12057064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b2f931df9dd6d05c17de44c0060044cdc3cf6b6e56812ca8b0e2157b2614d2`  
		Last Modified: Fri, 08 Jul 2022 00:02:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd38016cf6c8e8f55c33a131c5c7ee143479a47dcc6fe0e006ce5ab5d557698d`  
		Last Modified: Fri, 08 Jul 2022 00:04:35 GMT  
		Size: 28.1 MB (28089308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04bd969a62e31cd715d2aa7790f996720a2c69d088176ec0570993b9cf76b11`  
		Last Modified: Fri, 08 Jul 2022 00:04:30 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2fa252bb797787e7b32aa7e6e2c8a05f929246cc80e160da236c6a72419f7b`  
		Last Modified: Fri, 08 Jul 2022 00:04:30 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; 386

```console
$ docker pull php@sha256:8827c41dd59449689e4a2e2799cedbe6e8bdd39cbc9460d59048b92e29d283a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165609598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffaeecc2ad2b96c9698c45bbc22fdaecbac691036e5212164b6bef370e55ec41`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 11:41:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 11:41:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 11:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 11:42:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 11:42:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 11:42:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 11:42:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 11:42:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 12:08:29 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:27:36 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:27:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:27:38 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:27:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:27:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:39:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:39:43 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:39:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:39:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:39:45 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1090d3a60d1d6fdda24dfc39bebc748986624eb6704d50fec74f24f9d02bd359`  
		Last Modified: Thu, 23 Jun 2022 13:26:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42ca7953461e2d2ec71f3f7b3be3185bbef10580cc04d8b2dd05333e08ae016`  
		Last Modified: Thu, 23 Jun 2022 13:26:59 GMT  
		Size: 92.5 MB (92512688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26af2ccf84cef54d7640e15316beaa5cd504fe5d633458a7c2abbc8339c8279e`  
		Last Modified: Thu, 23 Jun 2022 13:26:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e96920d3c0190ee22ab3569f3b9a235456e660a0b26e2a06d8559dba9bfcf66`  
		Last Modified: Fri, 08 Jul 2022 00:20:10 GMT  
		Size: 12.1 MB (12083675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb1b707e7b0bce4495803a0326ff8f52030c7721b204835b42fd107fdf931b1`  
		Last Modified: Fri, 08 Jul 2022 00:20:09 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b469f05aa6cff9ac40ff8a248ffd3ed5685c7ac3e8afa3950893a7204a0e71da`  
		Last Modified: Fri, 08 Jul 2022 00:22:32 GMT  
		Size: 28.6 MB (28619401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463fc00a60229dc05cfa541e038957bef406d951d1ad91c016bd0e101ac16af3`  
		Last Modified: Fri, 08 Jul 2022 00:22:27 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6195940a56d22f674837d7297b1a8f0bfb6c91417ca33fed30d36e87b644aa6`  
		Last Modified: Fri, 08 Jul 2022 00:22:27 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; mips64le

```console
$ docker pull php@sha256:b4318eb1e7977e380f8d44c855670cd99fb17d0fe3b6d2a0a3322d6f3cb19373
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138509209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11d80c698fe6ba5ef95ec26789d5decad91c9a36f8e94e261932b3497e5f4ed`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:47:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 24 Jun 2022 03:47:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 24 Jun 2022 03:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 03:49:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Jun 2022 03:49:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Jun 2022 03:49:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Jun 2022 03:49:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Jun 2022 03:49:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Jun 2022 05:48:42 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 24 Jun 2022 07:41:50 GMT
ENV PHP_VERSION=8.1.7
# Fri, 24 Jun 2022 07:41:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.7.tar.xz.asc
# Fri, 24 Jun 2022 07:41:56 GMT
ENV PHP_SHA256=f042322f1b5a9f7c2decb84b7086ef676896c2f7178739b9672afafa964ed0e5
# Fri, 24 Jun 2022 07:42:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jun 2022 07:42:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jun 2022 08:37:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 24 Jun 2022 08:38:01 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Fri, 24 Jun 2022 08:38:08 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jun 2022 08:38:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jun 2022 08:38:15 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f219682e174ec0c8db99a95eec28f5669883b8b982d59924a9aa4648117eba3`  
		Last Modified: Fri, 24 Jun 2022 14:46:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd4e08b696ca5edf71d1b9226615be2f8b1c935a3f6220277a5fb0d2cec9661`  
		Last Modified: Fri, 24 Jun 2022 14:47:16 GMT  
		Size: 71.8 MB (71812340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986b34928c503914317f3c0f3531599a9879a790be54ae08039f7b7d16b8af98`  
		Last Modified: Fri, 24 Jun 2022 14:46:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc83395cff17c684631fb58f5f96e00e853ce09c561cae1f9f2f58d9e3bf948`  
		Last Modified: Fri, 24 Jun 2022 14:56:03 GMT  
		Size: 11.8 MB (11820333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c58ce0c3cb0327470cf57685317f75c420a09c18f66b8f67229b14fc50fd0`  
		Last Modified: Fri, 24 Jun 2022 14:56:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987c3c9bcdb7b59df3582a42b67f3aadbb4b884538c22c7057105b5d1d8c458`  
		Last Modified: Fri, 24 Jun 2022 14:58:58 GMT  
		Size: 25.2 MB (25231861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db00e6779173ec7c0369834046c6cb0e965e236c74e00174923d38012d49e59`  
		Last Modified: Fri, 24 Jun 2022 14:58:41 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53185c66393483cb132806d47c82d694f5688bfbf91257cdb445b9fc73ee83c3`  
		Last Modified: Fri, 24 Jun 2022 14:58:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; ppc64le

```console
$ docker pull php@sha256:0e955ee5d7a8ee97b81a5c3ae12a9776190bda79d11219ee7e25ec7fef5f3e59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163518230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f6069b6cc7c0c24d3043aa799b12e1aaf66a909d59cda6486b5a4b0ebd17ee5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:19:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 13:19:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 13:21:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:21:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 13:21:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 13:21:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:21:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:22:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 14:31:40 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 23:18:12 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 23:18:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 23:18:19 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 23:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 23:20:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 23:49:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 23:49:26 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 23:49:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 23:49:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 23:49:51 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618065a0bfa6328b4fa8bfa229184683290183358ab149e3cef6f7df5bd46640`  
		Last Modified: Thu, 23 Jun 2022 17:34:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653612b565ca7461d374ea3a3a41e762b8a5cb9feb9a82568ac1630fb1fd7a93`  
		Last Modified: Thu, 23 Jun 2022 17:35:14 GMT  
		Size: 86.6 MB (86628379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1e1e66d25ba24674f96f2e04415857aac883817afbcf72ae287832b06683a7`  
		Last Modified: Thu, 23 Jun 2022 17:34:36 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc36220f193ca31901b483068c83f479481d184309b248bfea51176c8f928e3`  
		Last Modified: Fri, 08 Jul 2022 03:16:58 GMT  
		Size: 12.3 MB (12316961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875fe8658482f4f43a6cd66d413b139115fb5e2c0c31b19b5502ab9f2f8b5ab2`  
		Last Modified: Fri, 08 Jul 2022 03:16:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d493f92d77dc72db713baca956e93002185dfafb15c2b2251b41c9919a62ca`  
		Last Modified: Fri, 08 Jul 2022 03:19:44 GMT  
		Size: 29.3 MB (29282375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a8af05d1013c38adbe44007ab6e74cd5415c1cb7afe3bcbd63e69a38d8a8e0`  
		Last Modified: Fri, 08 Jul 2022 03:19:39 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9819fc4651f5b9abe2c246d72182d03e63d00e98a9ccc064393c55b0a01c0585`  
		Last Modified: Fri, 08 Jul 2022 03:19:39 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-bullseye` - linux; s390x

```console
$ docker pull php@sha256:83ec03f0c1f494e331b398d98b9961ec31ca848f6635d687c198eff86154671e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140509909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb14af7d7a714d26a926a87f844182545d7408bbc2e78076a2498a5a24101c1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:23:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:23:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:23:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:24:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:24:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:24:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:24:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:24:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 06:45:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 21:21:05 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 21:21:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 21:21:06 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 21:21:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 21:21:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:30:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 21:30:07 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:30:08 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 21:30:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 21:30:08 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac3dc014d550bf03a1729b039a5f18fc36ee17be3dd0416bb30c3b4a7535c1`  
		Last Modified: Thu, 23 Jun 2022 07:57:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4014f31e7ed528e757a0a6304c23851740d7fc224ebc60a432fe29fcfe7d22d9`  
		Last Modified: Thu, 23 Jun 2022 07:57:10 GMT  
		Size: 71.6 MB (71623880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69abfac73dadc0771e03f979a0317fbbd77e330ec2249b29ff7fe9b1847a7c6`  
		Last Modified: Thu, 23 Jun 2022 07:57:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e433392c2f6717d5c6c701c9b998e41492e07506358cc010d8da0cf69395c`  
		Last Modified: Thu, 07 Jul 2022 23:07:41 GMT  
		Size: 12.3 MB (12264791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c8ef21c89bd36bfe3ec956c860275c79d71414b3e4eb18970243a1b786cc43`  
		Last Modified: Thu, 07 Jul 2022 23:07:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce72ef6fe89de366489c56d63e7a9ba85cfe7fecd572e39c24f9311394fb6edc`  
		Last Modified: Thu, 07 Jul 2022 23:09:35 GMT  
		Size: 27.0 MB (26962290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31ea5f0406bd4ec250957ee14b37f062d62821149f7a6c780971fa9722a6c89`  
		Last Modified: Thu, 07 Jul 2022 23:09:31 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f17cf4ec8987414a704407c8591c9e96156eaefe8809b801410c1d229c653a`  
		Last Modified: Thu, 07 Jul 2022 23:09:31 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
