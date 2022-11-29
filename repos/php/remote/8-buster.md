## `php:8-buster`

```console
$ docker pull php@sha256:68421c745e22b34310aa7b613ba13cce32f6219d1b11ec3584b218be7c2f6d4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `php:8-buster` - linux; amd64

```console
$ docker pull php@sha256:a955e5b54122930bff58327b6b990e61d3f6dd98262ebe6054235ad4661ba955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149432476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7cc8a6a03b2a694ca90f9ed343d8b8ccb3d88bdce7c1685adeab9aa9f30676c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Tue, 29 Nov 2022 02:43:02 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:43:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:43:02 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:43:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:43:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:46:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:46:14 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:46:15 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:46:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:46:15 GMT
CMD ["php" "-a"]
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
	-	`sha256:6697a8918294941108b98d4080936ee6edc291e3a23ccc282b5afede724bbb95`  
		Last Modified: Tue, 29 Nov 2022 04:18:46 GMT  
		Size: 12.1 MB (12125907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aece69c2bb547daad759ce625233a93a4f58c271c0e20bdb4b2649a33f7ccaa`  
		Last Modified: Tue, 29 Nov 2022 04:18:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854672326fa757ac964e4e4b4e5c53b65ea8e112d4cb74350e584317054b32c2`  
		Last Modified: Tue, 29 Nov 2022 04:18:50 GMT  
		Size: 33.5 MB (33475225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8dd3e1f3a832b12a9a12ce8820a67bb0f23bdf2721bee4da8e3f79aace46bc`  
		Last Modified: Tue, 29 Nov 2022 04:18:45 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d42015e8dc859158a1c1c6390889a31a7577d14d9dc932a21342436fc3fa35`  
		Last Modified: Tue, 29 Nov 2022 04:18:45 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:288101379a6829d213c362af5824e21e6e0d48675591769d1c972be925795b94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124548840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4889ee9a2de64c8ee57cee84be8513791e66e46d8cc9b00539c16ed0f1d30b01`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Tue, 29 Nov 2022 03:42:30 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 03:42:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 03:42:30 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 03:42:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 03:42:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 03:45:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 03:45:27 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 29 Nov 2022 03:45:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 03:45:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 03:45:28 GMT
CMD ["php" "-a"]
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
	-	`sha256:0bc590fdbb039d701aba2126be63b5ec3da8a92771753fb477d5f82c3dddd5ea`  
		Last Modified: Tue, 29 Nov 2022 05:25:48 GMT  
		Size: 12.1 MB (12124045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1e1aebac0dc4aab0f820fe888a91f6831835c6b4e0466f0446dc8f0dcddaeb`  
		Last Modified: Tue, 29 Nov 2022 05:25:46 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1684abdf119d997cc7edd17967ecf61dd99a6767dd51ba13d8a0b42b99b7f9`  
		Last Modified: Tue, 29 Nov 2022 05:25:52 GMT  
		Size: 30.1 MB (30129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2e96c4ffd9538bbeebc0f90e00e71b7b3f3dd822ec312828c8a35d2ee4796f`  
		Last Modified: Tue, 29 Nov 2022 05:25:46 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd2a57d98fc9cc760e08203b9aa71f0b48eb058f6514ccbb6078a3596d74304`  
		Last Modified: Tue, 29 Nov 2022 05:25:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:d9184961fe40c3f288570b55526131ad792856ff04ae91cd9ac48ac632220f74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141815828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c3fd789622fcb6667b81df1f67db0c83df2c5dfeb94b07cca04e5dc70fbae5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

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
# Tue, 29 Nov 2022 02:54:10 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:54:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:54:10 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:54:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:54:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:57:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:57:09 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:57:10 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:57:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:57:10 GMT
CMD ["php" "-a"]
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
	-	`sha256:b943ca992c09f5f2acee782316e30e7211c472648bc060e0e800d17865b8c8db`  
		Last Modified: Tue, 29 Nov 2022 04:15:22 GMT  
		Size: 12.1 MB (12124783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9de192e979edb7dc25d3f497139ec661dd7b0cfd848b7f1793585269ff74323`  
		Last Modified: Tue, 29 Nov 2022 04:15:21 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3b2a4209272a76d2d6db192da480807928801b5121af71b939af55b92aff0a`  
		Last Modified: Tue, 29 Nov 2022 04:15:25 GMT  
		Size: 33.4 MB (33409351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379b5c01179b2ef633fd765f0fa196361f0f8dad7cb8ccb0a0b73ead5323fba3`  
		Last Modified: Tue, 29 Nov 2022 04:15:21 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80406dd0ba80f3ba5eb45b761f33c6d99493fdc14300c7cea18f10e9415a7b`  
		Last Modified: Tue, 29 Nov 2022 04:15:21 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-buster` - linux; 386

```console
$ docker pull php@sha256:20760826fa614837a78f5f66e9431856f312d1145ab393f465fdecfe65e0c247
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154841629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b494953075f03b5ba8ed4a9ea9735dbe2c32e19b104b954552317b312105f5c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:54 GMT
ADD file:0d8bf61c363b36e7073c9fd91c34181d2b278068a38749faee0d3c7ec654bda6 in / 
# Tue, 15 Nov 2022 01:41:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 02:05:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 02:05:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 02:05:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:05:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 02:05:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 02:05:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:05:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:05:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:31:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:55:46 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:55:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:55:48 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:56:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:56:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:58:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:58:44 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:58:44 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:58:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:58:46 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:f3d13e168342b55b3a1ab5df56e84f077449ec7563d80bd1eca07424d641822e`  
		Last Modified: Tue, 15 Nov 2022 01:47:52 GMT  
		Size: 27.8 MB (27798392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9f9b55022def290d7385afd7f02bea8e46735656bbdc1b657fd52e1a729f1f`  
		Last Modified: Tue, 15 Nov 2022 04:27:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59b870ea5c5d69ab613073ce709a2a4285056b90ec18245efeb4deba1f7d93`  
		Last Modified: Tue, 15 Nov 2022 04:27:59 GMT  
		Size: 81.2 MB (81234677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3232370cfacefa6f5b824c6441090d1c2825f4bb04e661d17b79f47f1f985621`  
		Last Modified: Tue, 15 Nov 2022 04:27:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4628c8b68e6b8c0055efde60b032c2474f24457c6e4376173180e4e24099cb75`  
		Last Modified: Tue, 29 Nov 2022 04:37:07 GMT  
		Size: 11.9 MB (11911304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c878e791967da0cc0285ab723afd714641d01184a7c7c7cc4efd652552935b6a`  
		Last Modified: Tue, 29 Nov 2022 04:37:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da94e2d329bcf5c2c778508c6d8d45314c2e26e3d2534b625386cefebeb0da54`  
		Last Modified: Tue, 29 Nov 2022 04:37:10 GMT  
		Size: 33.9 MB (33893617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923df1962b9437a8d241f9f378a91e8a430dae8511e3585c7be406538ff4d468`  
		Last Modified: Tue, 29 Nov 2022 04:37:05 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a177741567663801e3c9c95e2236e8e6fcfe3e02b65ff2b4e4f8ddea86254d97`  
		Last Modified: Tue, 29 Nov 2022 04:37:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
