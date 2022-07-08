## `php:buster`

```console
$ docker pull php@sha256:aa0d84f6af34b6818b3a472e74f79cca5078809d7524e4045009a7ba3025c706
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

### `php:buster` - linux; amd64

```console
$ docker pull php@sha256:a030afe223c7661ab95cdbee91a4cc59c14439189b6a1887193e65d8edac1608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.5 MB (151462406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8033f5292c3bde3d4b9ac38867ddf15072fc62b93027ba8b05999e78ef23e956`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 07:35:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 07:35:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 07:35:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 07:35:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 07:35:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 07:35:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 07:35:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 07:35:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:02:04 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:31:27 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:31:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:31:27 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:31:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:31:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:34:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:34:55 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:34:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:34:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:34:56 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d0f41537a4bb341b83f091698de52574e75c662ac8cb471ab039c882249ba3`  
		Last Modified: Thu, 23 Jun 2022 09:05:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6ded8da51ea293b1ab37514236d32967318d3b94f1df347f87d941d0d6e575`  
		Last Modified: Thu, 23 Jun 2022 09:05:45 GMT  
		Size: 76.7 MB (76683783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2ec4360a6f882047371245cbfceb8084bb7a9edf74f3e8953e74dc448c1d7d`  
		Last Modified: Thu, 23 Jun 2022 09:05:34 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6f49ad72b845c5c03ede72ec3572555015e9567743be1213c609bf35ab0b4`  
		Last Modified: Fri, 08 Jul 2022 00:13:57 GMT  
		Size: 12.3 MB (12276492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618948ae773fc1ff6ae9aab39c76a47d742f5c9609b9218fd63426d4b6cdd102`  
		Last Modified: Fri, 08 Jul 2022 00:13:58 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e5cf371656df270645bf11b01e4351b328a3e0ec13de5cb32f150875c199ae`  
		Last Modified: Fri, 08 Jul 2022 00:14:02 GMT  
		Size: 35.4 MB (35358400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6bf43813a23961584f1374213d91ee46c77bbe9b67b0fe6004fe3c3c94458a`  
		Last Modified: Fri, 08 Jul 2022 00:13:56 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21e755a37f9081bce2d4c767bca376e30642e0a312a6b4f2f353ed9d04764ef`  
		Last Modified: Fri, 08 Jul 2022 00:13:56 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; arm variant v5

```console
$ docker pull php@sha256:88713547c613c4cb286bc53668dcff49a648ca6561b1b4e2158ce16e99fcb721
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129001778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831140a98bff813f4d7d561ac8ae5baab5e82002fdf415a09d7193a10332913c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:51:39 GMT
ADD file:b1e035d48236f9259b8573f7b0ac432e69c0d8d42292d24b41d94cba3b942eab in / 
# Thu, 23 Jun 2022 00:51:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 23:58:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 23:58:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 23:59:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 23:59:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 23:59:46 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 23:59:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 23:59:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 23:59:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Jun 2022 00:45:35 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:00:57 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:00:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:00:58 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:01:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:01:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:07:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:07:07 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:07:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:07:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:07:10 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:e6235ec1c9144fd72693df78eccd13b2e35d15fb254f6e0e7dd5ff17a944f0e7`  
		Last Modified: Thu, 23 Jun 2022 01:07:10 GMT  
		Size: 24.9 MB (24889983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97652c4e6f12dbd2a2c7f3c9abd595fa9ebe233136cf3a378e330204b77284c2`  
		Last Modified: Fri, 24 Jun 2022 04:20:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736eca0c5e581ebe05218abdad2a37a7171c31c241acf99e75fde8d3e12bb88e`  
		Last Modified: Fri, 24 Jun 2022 04:21:33 GMT  
		Size: 58.8 MB (58827152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dea73009c526b2f97a0b7aa233a5f52b72fd093354f5874909bbb52feb3c70e`  
		Last Modified: Fri, 24 Jun 2022 04:20:51 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad577d15398c3d7d5616af6b05e329c803eb794c1d8e45b41281f3eebbcf7db`  
		Last Modified: Thu, 07 Jul 2022 23:35:23 GMT  
		Size: 12.3 MB (12258048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceb374f8e2c19f89da7e4f0f5082016e561846714e2c32a8eb6de2ec18285b8`  
		Last Modified: Thu, 07 Jul 2022 23:35:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7613c0aaaf2a727ab85f3cd05789caebedd056e124011d1157228bf03955615c`  
		Last Modified: Thu, 07 Jul 2022 23:35:38 GMT  
		Size: 33.0 MB (33022908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528db46031c41beb15a6b1f219fb643e043dabd2466ce678358a038b9a6b336f`  
		Last Modified: Thu, 07 Jul 2022 23:35:20 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac817a454e7eec1c7f2447affdf446f57a1b0d41c23da2159653de72721cf827`  
		Last Modified: Thu, 07 Jul 2022 23:35:20 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; arm variant v7

```console
$ docker pull php@sha256:07dfdd7b8bb368c7c44c0e82deb8758e76e88db2d90bdaa41ea408244d949993
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126156254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2168e6f07af960bb1d8d046562b8b3e938c8688448667811e5391221005311be`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 01:00:49 GMT
ADD file:029ce6b1d94ffab93115ec72e29b81dc578e1e506b9f17808517198fa9a93144 in / 
# Thu, 23 Jun 2022 01:00:50 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:33:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 13:33:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 13:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:34:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 13:34:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 13:34:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:34:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:34:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 14:16:15 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:36:54 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:36:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:36:55 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:37:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:37:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:41:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:41:51 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:41:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:41:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:41:54 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4a43dd1ec497b763b016923ec92796419a4f550a0b2c64b17a79c4f7f575643e`  
		Last Modified: Thu, 23 Jun 2022 01:16:47 GMT  
		Size: 22.7 MB (22748000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db582f5f0bd7b736eb381f0ee1be5bba739ff74db7bb130cf1d6b2cdca642136`  
		Last Modified: Thu, 23 Jun 2022 16:21:09 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ecca9394407ff4b630b7e2cedae363b82364c94764a0c7e08b819e7bfdc502`  
		Last Modified: Thu, 23 Jun 2022 16:21:45 GMT  
		Size: 59.5 MB (59539424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67065bf760ae6352f07ecd58a1802b8f25e7768aefbaa06a1c0cbec330d0f00b`  
		Last Modified: Thu, 23 Jun 2022 16:21:09 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d374040481ec6d048f1d54bdfd50b3a4998181770b1b051c991e180890485`  
		Last Modified: Fri, 08 Jul 2022 01:11:53 GMT  
		Size: 12.2 MB (12233624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5e86855d7a7d4d7edd3bffd8778a619eb5f42593852ce175801b1b5ee003c5`  
		Last Modified: Fri, 08 Jul 2022 01:11:49 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b713467d72db78a4ee11eb81d6f4f01a299098af83cefa1e1b0a85316d6b`  
		Last Modified: Fri, 08 Jul 2022 01:12:07 GMT  
		Size: 31.6 MB (31631516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f26347901d640725497827a76a5ac41d1dec728aa50770137359c3a85021e01`  
		Last Modified: Fri, 08 Jul 2022 01:11:49 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe700bdf049915162270a9fe1183cb9de6a3d9e772eb3814f43c762a5f8142e`  
		Last Modified: Fri, 08 Jul 2022 01:11:49 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:c6da4a0f774b6965d16488c3d27f84b6b2c812ba38887758b5515d4302801c9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.5 MB (143527242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4063b5a2111c4aff2216fd3455a31717e2253a942ff8be0bb76e63b1f71ab477`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:08 GMT
ADD file:e491c8ce913289e0c673bd14014c5506cca7b78575aa5c8303ec856525209505 in / 
# Thu, 23 Jun 2022 00:41:09 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:47:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:47:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:47:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:47:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:47:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:47:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:47:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:47:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 07:21:25 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:10:22 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:10:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:10:24 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:10:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:14:26 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:14:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:14:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:14:28 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:d8b55b2b6839f70c2ed0662b18f4d9724108500136dfd03e999a5f91c815984b`  
		Last Modified: Thu, 23 Jun 2022 00:48:15 GMT  
		Size: 25.9 MB (25914029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d034d34434f4b792ee58f249f7eb03c9d05f82341f7f71967e7abde5c0af3eef`  
		Last Modified: Thu, 23 Jun 2022 08:33:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3b7cfb9f69c9364d83c4565131c5cc6b0d74c1abea7e7058ad7b1d537257f7`  
		Last Modified: Thu, 23 Jun 2022 08:33:30 GMT  
		Size: 70.4 MB (70364322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4f50c99afb20799681c11e29b703209d91013affd60ce4f74a71d38bd122f5`  
		Last Modified: Thu, 23 Jun 2022 08:33:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef49fad6ff65d5bc5a4b483fe7dc1a9bdff96e03fbd6b2efc9f65d20f1216a`  
		Last Modified: Fri, 08 Jul 2022 00:05:09 GMT  
		Size: 12.1 MB (12063595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dc1bc5b22ccd3d9c4ad3c284a350cca3d11ca4efa7312072150e18680b4657`  
		Last Modified: Fri, 08 Jul 2022 00:05:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f1e9542400e4cf042f8dcb7aa11fe1dac8125e3b6ec12d3432d3db1c04e1e5`  
		Last Modified: Fri, 08 Jul 2022 00:05:13 GMT  
		Size: 35.2 MB (35181652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19ea9b26dabefea80af0446047c78912782aa3fa073b7324daa4990df811b44`  
		Last Modified: Fri, 08 Jul 2022 00:05:07 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b73ddb08d100ec5a2a4f5f1411feee4fea22ad09f9c7be93c0053999aee485d`  
		Last Modified: Fri, 08 Jul 2022 00:05:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; 386

```console
$ docker pull php@sha256:00f0f50f4e374d198c1da391109d8315dc705836d8beca5aef61683610b3d63a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.1 MB (157092980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d590a623e60b045c307abe40cb55a10a6877a8dead3968b8f5ed24ad1d1bc8b0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:59 GMT
ADD file:d4d6ebbe6e038ac58e266fb07bee755ccccf597fb15b3e8264165279e8fbed3b in / 
# Thu, 23 Jun 2022 00:40:00 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 11:54:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 11:54:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 11:55:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 11:55:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 11:55:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 11:55:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 11:55:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 11:55:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 12:21:16 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:39:58 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:39:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:40:00 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:40:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 22:40:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:42:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:42:56 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:42:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:42:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:42:58 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:e8877ae0470a67233ffd6b1ee842fc356ff46b5b3c594a02395801f85ccec7b4`  
		Last Modified: Thu, 23 Jun 2022 00:47:36 GMT  
		Size: 27.8 MB (27799542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5c149d286aea4ad057b015b69d3281c0af0efce4aa4e8285433721af2b9eb7`  
		Last Modified: Thu, 23 Jun 2022 13:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82160afe245a35bfb9dce3c758338e3f6667bcef318602ee2d815e07bf8051a`  
		Last Modified: Thu, 23 Jun 2022 13:29:09 GMT  
		Size: 81.2 MB (81228465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc126f6acc245f7df92152a426f111932f4cf4a526b092893121f08d3b9e7acd`  
		Last Modified: Thu, 23 Jun 2022 13:28:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06221f68d76647ffbdc5cff90965289783da2329bcd23e6d957983cd9c1bbd6`  
		Last Modified: Fri, 08 Jul 2022 00:23:05 GMT  
		Size: 12.1 MB (12089163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2afcbac645aceeab1a3425c0c4402b8ee21b58bc95c9dc75fe60bd5d948407`  
		Last Modified: Fri, 08 Jul 2022 00:23:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972853b050577d0014c82b70522330283a6b5b720f331fbf96fc4c48b6eb9ed1`  
		Last Modified: Fri, 08 Jul 2022 00:23:09 GMT  
		Size: 36.0 MB (35972175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f09d6d89cc2c5555b67102794a101127cdf2c7d08c44131186ae0c26936fcc3`  
		Last Modified: Fri, 08 Jul 2022 00:23:04 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b06104f786c0842a80b519c00ce0c47549917e4b9ea3708e61f42f8da1c90f2`  
		Last Modified: Fri, 08 Jul 2022 00:23:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; mips64le

```console
$ docker pull php@sha256:dcbe5186fa367cb3e2b60c94ea88991719626435b42f253428b8bb55be767ea4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131110531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8816be242d1b443e5d71a28717c1c903d76de994a9e1c4916a71b86dac80c1a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 01:11:27 GMT
ADD file:ef55fe42f292a3671fe1772cf96e3559101dea308e79974d1ca92103cb6c7b9c in / 
# Thu, 23 Jun 2022 01:11:31 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 04:48:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 24 Jun 2022 04:48:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 24 Jun 2022 04:50:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 04:50:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Jun 2022 04:50:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Jun 2022 04:50:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Jun 2022 04:50:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Jun 2022 04:50:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Jun 2022 06:45:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 24 Jun 2022 08:38:30 GMT
ENV PHP_VERSION=8.1.7
# Fri, 24 Jun 2022 08:38:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.7.tar.xz.asc
# Fri, 24 Jun 2022 08:38:37 GMT
ENV PHP_SHA256=f042322f1b5a9f7c2decb84b7086ef676896c2f7178739b9672afafa964ed0e5
# Fri, 24 Jun 2022 08:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jun 2022 08:39:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jun 2022 08:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 24 Jun 2022 08:52:18 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Fri, 24 Jun 2022 08:52:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jun 2022 08:52:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jun 2022 08:52:33 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4490dc714fa293f64fe0693aa619f1baee9db64f30c00558cfbe5bc798ba1a30`  
		Last Modified: Thu, 23 Jun 2022 01:21:44 GMT  
		Size: 25.8 MB (25814612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c37e4d9e78039bb5a651655f64ba7f5f7a2b5128a58211aa427810b92b3cfa4`  
		Last Modified: Fri, 24 Jun 2022 14:49:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5205ea28bd5bfad4468792ced7b0ef727cfd3c80ddc5c9cc55e14044c6aecdab`  
		Last Modified: Fri, 24 Jun 2022 14:50:10 GMT  
		Size: 61.4 MB (61409402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858c3bbba6f77fb1a745598f9e0fece9b2e77022125354f5c29506cf2096a73`  
		Last Modified: Fri, 24 Jun 2022 14:49:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa59095db8e12c59682ba335ff8875e409c223edcb6ba5e1f3899887b6a4bb54`  
		Last Modified: Fri, 24 Jun 2022 14:59:28 GMT  
		Size: 11.8 MB (11825441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b005ab65fc17606a788ae140ed85ba7ce8b81fed17a8e9c271bae176cbdf2064`  
		Last Modified: Fri, 24 Jun 2022 14:59:26 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e757f315a944d37499d7cc2bb419077b0efec04a97691bfb4f22231f744bd68a`  
		Last Modified: Fri, 24 Jun 2022 14:59:47 GMT  
		Size: 32.1 MB (32057432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e156ea9d48e6b293fadc9da7e10aeca4bb68cec3fba8b78d1465aafad09626`  
		Last Modified: Fri, 24 Jun 2022 14:59:25 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ca3b657aaa8bf6739dafa65979a482032f291aeac918fb099cda88215fb27e`  
		Last Modified: Fri, 24 Jun 2022 14:59:25 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; ppc64le

```console
$ docker pull php@sha256:2e99eeb500d948e84335833b828cb4254f63ce0a632198f5101d99e7b2442102
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.4 MB (162369193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf1b82fab70c172e7133583eda8034a5afcf770be18d3787b1fcda8bc6d6412`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 02:03:29 GMT
ADD file:72c3739ee19c484811115caacd1b2bf903a764246b77af65c098817e5a13f8ca in / 
# Thu, 23 Jun 2022 02:03:32 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:57:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 13:58:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 14:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:02:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 14:02:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 14:02:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 14:02:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 14:02:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 14:59:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 23:50:07 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 23:50:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 23:50:17 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 23:52:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 23:52:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 23:57:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 23:57:27 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 23:57:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 23:57:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 23:58:01 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:18188ef7804b6b81fced393814287e8c6e18656751108acdbbd364d57775a243`  
		Last Modified: Thu, 23 Jun 2022 02:17:52 GMT  
		Size: 30.6 MB (30560321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2877e8479db46f29bb54ac758acfe651da84aefe1b9543a13838915d6800465`  
		Last Modified: Thu, 23 Jun 2022 17:37:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30446a3cc0e690c09fe51389b94fa6f6ffbf5e2f269541d2b70de4db3a1019a3`  
		Last Modified: Thu, 23 Jun 2022 17:37:58 GMT  
		Size: 82.3 MB (82294473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9b735ef7ac827069c9f2f3ccc59e8da89b92f9a15d2f5c2f6c2cde756c73b1`  
		Last Modified: Thu, 23 Jun 2022 17:37:37 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1333afcc6324daa54205c130002119bc3cbd3e1eca4484c35db5b78d0cfcb71`  
		Last Modified: Fri, 08 Jul 2022 03:20:21 GMT  
		Size: 12.3 MB (12324992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d72795644691287698fac4fc0f549a0bed6cfb5bf1caa4628eda0b8d1bf7b2`  
		Last Modified: Fri, 08 Jul 2022 03:20:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e6014eccd8185d7ed644e3555bb60436754dd754c94d3d90899bce8f6273fb`  
		Last Modified: Fri, 08 Jul 2022 03:20:27 GMT  
		Size: 37.2 MB (37185713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a38095fded8c165433c54c231391bdfb039013ea8116741c8a245c0b2f1703`  
		Last Modified: Fri, 08 Jul 2022 03:20:20 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70b83edeb3dd107bdf2a32013e69c47fee96907c5996905b8a1981bb9e011de`  
		Last Modified: Fri, 08 Jul 2022 03:20:20 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:buster` - linux; s390x

```console
$ docker pull php@sha256:ec4c028c5d9f06df3bf39c2a2204a942564ccdadb95cf4cef48b1c0fd4667eda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136294658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd7ce5adf1d6a712bc50a56694d8d58a980c61358355800cd625924b37abd4e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Jun 2022 00:44:04 GMT
ADD file:b5735387132c5d35278da27339d76ef4a166c7ea012cfe13bd542fd5f0055fb4 in / 
# Thu, 23 Jun 2022 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:34:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:34:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:35:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:35:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 06:54:45 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 21:30:27 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 21:30:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 21:30:27 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 21:30:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jul 2022 21:30:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:32:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 21:32:40 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:32:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 21:32:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 21:32:41 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:34b063f6640cedaaed5292721bedcce5039c2e2c11d3168badb2d90259505d49`  
		Last Modified: Thu, 23 Jun 2022 00:52:35 GMT  
		Size: 25.8 MB (25758710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8357c4b02deef8ecce801495e93f5c4242cf7900e112d6776b08a230c274552`  
		Last Modified: Thu, 23 Jun 2022 07:58:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3169fc154c33291175b971afc7c65958bb32d8b8f165c05bee593b6c64258b`  
		Last Modified: Thu, 23 Jun 2022 07:58:24 GMT  
		Size: 64.7 MB (64727022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685acc3dbe56641d8296e5a22dc5a29b1e35bfe270094fec5f843ecfe07ee64a`  
		Last Modified: Thu, 23 Jun 2022 07:58:14 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dea21acea7133ee2df8a9e559a0bfb4bad91b59c225c5c66a5327c0a9f0a85`  
		Last Modified: Thu, 07 Jul 2022 23:09:55 GMT  
		Size: 12.3 MB (12265138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c93cbc1058994d40c3611c92b1e85a7a8bd343a0a8f38cd0d296b468ae72d3`  
		Last Modified: Thu, 07 Jul 2022 23:09:54 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d922f184d9ef58e77488cbc3204d694804d297a8feda8f1060c7771db176b4b7`  
		Last Modified: Thu, 07 Jul 2022 23:09:59 GMT  
		Size: 33.5 MB (33540102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1f7201ce5822787997a3664de4ca5a6ccab6e847016d4e7d03b71275deaa1e`  
		Last Modified: Thu, 07 Jul 2022 23:09:54 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea40d06bc4539bd7627c71e498a6fd9ccbe97e7e66be1507bdd8ed9baf6dd11`  
		Last Modified: Thu, 07 Jul 2022 23:09:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
