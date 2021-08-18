## `php:8-zts-buster`

```console
$ docker pull php@sha256:abe738e3d41906fe39888c5dfcaf85ea7d11a5079777ab6fb0a9fe3a03f4f8e6
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

### `php:8-zts-buster` - linux; amd64

```console
$ docker pull php@sha256:ce571ca50fa0e938e5262bd1bdbcf2753b548c519e81ce82078d7c89f18f67f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140397365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7adab806e4cf93c317b4981e23c9918c69c529982801d03e3b2d7903451cdb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:15:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 12:15:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 12:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:15:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 12:15:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 12:35:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 12:35:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 12:35:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 12:35:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 12:57:57 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 12:57:57 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 12:57:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 12:57:57 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 12:58:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 12:58:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 13:03:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 13:03:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 13:03:11 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 13:03:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 13:03:11 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4909824c2d9e8528562a0eeab6573b4553f598555dd0a29f6f3fb2c28f6e4f2`  
		Last Modified: Tue, 17 Aug 2021 14:14:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d250e5f539524d16c1024cbbc0ba50cbde53f2ffce91a99088af37712f9e89`  
		Last Modified: Tue, 17 Aug 2021 14:14:48 GMT  
		Size: 76.7 MB (76680781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8ea4156ce7c000260f63ef26989a499cb20b8aea4f2d8a4cd0da0e79903b07`  
		Last Modified: Tue, 17 Aug 2021 14:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8238f132d97d206a69023c5f34782a5238f2ec526deb9574457f270afcb5957`  
		Last Modified: Tue, 17 Aug 2021 14:18:49 GMT  
		Size: 11.0 MB (11000190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37521c9e39d9c2b15c7c1a3c355adec64329d806db98293703be261dadce1829`  
		Last Modified: Tue, 17 Aug 2021 14:18:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792a5a2330633b614666c6611550fcaf77dbdfc204233f7c9efcf58b8e0fc947`  
		Last Modified: Tue, 17 Aug 2021 14:18:52 GMT  
		Size: 25.6 MB (25566909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15578197aa7da090733f50a74b339b721a17e0bad7370875ffc60fc5c946915f`  
		Last Modified: Tue, 17 Aug 2021 14:18:48 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb4373e0e51850912e8f420c05e0debe446648f7174aa453041e7ab44c173a`  
		Last Modified: Tue, 17 Aug 2021 14:18:48 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; arm variant v5

```console
$ docker pull php@sha256:fdc5b7c3881d8ad0036e9f33c2bb691e5c25ade29b071c305041fb9e7cad0c2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118958244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac1e810e225a7ddc723ce4e3ad39bded16c74f1902f5ebb988cad0d584017121`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:50 GMT
ADD file:f29260935f1f8b3eef5eb0d5e49dd4cf5370e8731a3f4006d6023724bce09601 in / 
# Tue, 17 Aug 2021 01:56:51 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:50:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 09:50:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 09:50:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:50:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 09:50:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 10:08:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 10:08:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 10:08:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 10:08:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 10:31:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 10:31:44 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 10:31:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 10:31:45 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 10:32:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 10:32:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 10:36:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 10:36:52 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 10:36:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 10:36:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 10:36:54 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3dfab4a5b2accf2d709d8c7d14a42715948ecf2d6da4943a6e2c0de8ae7536a0`  
		Last Modified: Tue, 17 Aug 2021 02:12:42 GMT  
		Size: 24.9 MB (24879063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d321d8f4d7296db7b3f84788c07d175b2504e3cb238dcf6d902c00d2f767c7d`  
		Last Modified: Tue, 17 Aug 2021 11:53:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9034c2264011ba14ef8ccef384c6f6af0f92c68e0c9712c91ed2e172eb0bc1c6`  
		Last Modified: Tue, 17 Aug 2021 11:54:39 GMT  
		Size: 58.8 MB (58820510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c3914b89d903a4a841688fa553ea06173ed81ef703b0421fb8b8c8c37223d0`  
		Last Modified: Tue, 17 Aug 2021 11:53:57 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73716e9c8281d2e87ad19a8276aca6d5cd378f00988e2286fae7d71de8d6fa`  
		Last Modified: Tue, 17 Aug 2021 12:00:25 GMT  
		Size: 11.0 MB (10998086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c76ec91b555b54859e8eedad465f85c3aa70f3d7998c7971d3c76c9c7d01c`  
		Last Modified: Tue, 17 Aug 2021 12:00:22 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d840c6934bd924bed2c39fe7fae68987f24b3ec8aec340b277be6db2db9899`  
		Last Modified: Tue, 17 Aug 2021 12:00:38 GMT  
		Size: 24.3 MB (24257083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645854139f84135f903286139f6d5f8ca376fee95ba4a7af6347e0e62c40c0d2`  
		Last Modified: Tue, 17 Aug 2021 12:00:22 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232efeef0cb9ba1d5ec4cc3a31af2400ed568b4f4beab650e7e4788de98deab`  
		Last Modified: Tue, 17 Aug 2021 12:00:22 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:3edc3f7ddddbeab4030c868e7c3cc56cb65027dcf0649cfaf6348e2aa6ef0411
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116708324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbadce99d59f23837ced2460e1553689bcdc681382f6a50c4bdc9a5350e10043`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:42:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 21:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 21:42:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:42:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 21:42:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 22:03:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 22:03:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 22:03:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 22:03:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 22:49:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 22:49:27 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 22:49:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 22:49:29 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 22:49:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 22:49:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 22:54:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 22:54:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 22:54:18 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 22:54:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 22:54:19 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33c060d8eec1708da27f0a9a76b0a314310580ed93439479c9ae092af343369`  
		Last Modified: Wed, 18 Aug 2021 00:43:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525ebb74853898f10007afc7de780282b21a9ea0a864beded94ab9ad168eac5`  
		Last Modified: Wed, 18 Aug 2021 00:43:56 GMT  
		Size: 59.5 MB (59513282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890c2ff8fc03c934f3f2800273f710d7816ef3874597613e207973b7ef71188a`  
		Last Modified: Wed, 18 Aug 2021 00:43:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f9f78842a5fd57c98f59cfcca42395476cf1ec7821d401fa78141fd54a63ec`  
		Last Modified: Wed, 18 Aug 2021 00:52:21 GMT  
		Size: 11.0 MB (10998061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c71b0dc9b1bc6385b9d2c439e44b68ad7e1c09c0bcc2667cd7a94f7091f9201`  
		Last Modified: Wed, 18 Aug 2021 00:52:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28856654e33eca7370270d6d4133539bef4936ea41ceb8b93fd3e044b6111dbe`  
		Last Modified: Wed, 18 Aug 2021 00:52:33 GMT  
		Size: 23.4 MB (23447221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5f7449b977050fbf4c6063e5a444b3e4a4ffe9671f59b6193a34b03d4b3513`  
		Last Modified: Wed, 18 Aug 2021 00:52:18 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321c2194558181bf0e1a468decb95639b700740ab0727a068dac0c6f62ade584`  
		Last Modified: Wed, 18 Aug 2021 00:52:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:712e50bec1e42c4c1f631b18683811d2fd166678efccba6581cbc3d6d8114d2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132366100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca376990f6a7f9115ff2b8fc5036c08ee4119d5d69ae3d0273f02670971d47e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 09:22:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 09:22:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 09:22:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 09:38:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 09:38:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 09:38:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 09:38:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 09:55:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 09:55:34 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 09:55:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 09:55:35 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 09:55:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 09:55:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 09:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 09:59:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 09:59:17 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 09:59:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 09:59:17 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2900799337938aef6f721ade2a9bd22c057d46c83eb42ff623555b6eb4b1e9e9`  
		Last Modified: Tue, 17 Aug 2021 10:48:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22e74ac47771369d7c92bd6f47d92fcf96086e1d641c9d87462359bbda7d65e`  
		Last Modified: Tue, 17 Aug 2021 10:48:49 GMT  
		Size: 70.4 MB (70356766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1783e2b14bb08062d9096cd548d94f9327c5ba658efb80d09669f3ff2fc4d5a`  
		Last Modified: Tue, 17 Aug 2021 10:48:38 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb64238a92cd8ce29f8154ff4bc495b4eca89e522d16cce4de655945ad5460`  
		Last Modified: Tue, 17 Aug 2021 10:53:16 GMT  
		Size: 11.0 MB (10998747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddd5c49cf6bb1d3ba16edf8ab32c3b2876ed95e86d9be80a7ac49090e5b51c9`  
		Last Modified: Tue, 17 Aug 2021 10:53:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdffad4ac98a0f7ab9ec8cd8113fea276650349f072dfa010b37f9b0cec5395d`  
		Last Modified: Tue, 17 Aug 2021 10:53:19 GMT  
		Size: 25.1 MB (25092013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c7179b241105b100a56871fcd1d11cfedb520ba9da1a8eb00dcae3020d474d`  
		Last Modified: Tue, 17 Aug 2021 10:53:15 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38648fc9398c3daae3175d7c800123e48350f7d2cd1885cfe3a5cddf434441e1`  
		Last Modified: Tue, 17 Aug 2021 10:53:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; 386

```console
$ docker pull php@sha256:664a66413c9c2109e1a33e78e1006abf8b7fe499781924cb8175dc8a28f0da21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146094302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee9a2081fff6a8e9f687421b6ec6a6ddcc363d424ca0a3a81276f30f3d8edd4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:50:01 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 17:50:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 17:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:50:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 17:50:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 18:08:13 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 18:08:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 18:08:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 18:08:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 18:32:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 18:32:49 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 18:32:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 18:32:49 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 18:33:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:33:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 18:38:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 18:38:38 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 18:38:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 18:38:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 18:38:39 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e9eeed7bb21b82111b77c53bee07740bd5cd6dbfdf8b4f7184f37223efbe3b`  
		Last Modified: Tue, 17 Aug 2021 19:44:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e06f2ca62ad9d4559e5f42075c39284a2344543f09b27ba2335228b2d85a187`  
		Last Modified: Tue, 17 Aug 2021 19:44:27 GMT  
		Size: 81.2 MB (81230104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31f4ca0fa0ea804356df67cb3c353fbe8208878ec45ffbb9164eb9aa8bede35`  
		Last Modified: Tue, 17 Aug 2021 19:44:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be1ad4a1daad2a2cdb832fb763a26cce9763695400c4673b5f12b0013c32802`  
		Last Modified: Tue, 17 Aug 2021 19:49:17 GMT  
		Size: 11.0 MB (10999433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73a91c585e71ad9f7183133738c2b4c1ab149a54b542d45c19014d84ec4d3b`  
		Last Modified: Tue, 17 Aug 2021 19:49:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bebf0eec83774029fff891229471840156e72073d498259430e007e5aba5d4f`  
		Last Modified: Tue, 17 Aug 2021 19:49:22 GMT  
		Size: 26.1 MB (26063634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0249135cbf0e0e051a32771d04fe636b4772e28bdc3ef94b5312c788370e15`  
		Last Modified: Tue, 17 Aug 2021 19:49:16 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3d0ae1d0d0cf05c1c943ccf0f437dc3de436d2e6635e669a3e601c377acf12`  
		Last Modified: Tue, 17 Aug 2021 19:49:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; mips64le

```console
$ docker pull php@sha256:aad12cfe56224dcd1c3beb4bccf85a81815da516c700e018e84f84de73941296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123028992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781c3cea99814e5b1da7ff3ee8706095e40e941fb7978a1028eb523afa30844`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:26:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 06:26:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 06:27:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:27:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 06:27:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 07:07:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Thu, 22 Jul 2021 07:07:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 07:07:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 07:07:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 07:59:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 29 Jul 2021 21:46:32 GMT
ENV PHP_VERSION=8.0.9
# Thu, 29 Jul 2021 21:46:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Thu, 29 Jul 2021 21:46:33 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Thu, 29 Jul 2021 21:46:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Jul 2021 21:46:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Jul 2021 21:59:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Jul 2021 21:59:48 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 29 Jul 2021 21:59:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Jul 2021 21:59:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Jul 2021 21:59:51 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb76462e8360f1f5fff3b0d7916c87ab70e0bbd21e9c5d8bd295d716e936d11`  
		Last Modified: Thu, 22 Jul 2021 09:42:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec5c433242b6ed428599424c77a781f34a977b90bea14ac3510767faa7f11ee`  
		Last Modified: Thu, 22 Jul 2021 09:43:04 GMT  
		Size: 61.4 MB (61404113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6864500bb103f2e00dfcdfde3d5550d0f3d21a02b6cbd85a051712f0fcd37d2`  
		Last Modified: Thu, 22 Jul 2021 09:42:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cf415d13cc0e4aeb9e930ca9cb0f30d55daa25bd7e84bbaa73a8ab9ab16cb7`  
		Last Modified: Thu, 29 Jul 2021 22:47:38 GMT  
		Size: 11.0 MB (10997292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f9219a433c7eb0bb32b4497d070b75e5abf6ad00c6df53dac2dfe23ae1492`  
		Last Modified: Thu, 29 Jul 2021 22:47:35 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f9468713304cc2d44b4e8a55b593e61c1bad987af31fc016ae3c9cf5bedc8`  
		Last Modified: Thu, 29 Jul 2021 22:47:53 GMT  
		Size: 24.8 MB (24811362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7025d34ac6b480d2b251bf69c1c61d317690374878af5ee45860de749fffe9fa`  
		Last Modified: Thu, 29 Jul 2021 22:47:35 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c9bff9d81b1f124e4f77c9798c467d06512a37e3730e6c5f0092a683e6b527`  
		Last Modified: Thu, 29 Jul 2021 22:47:35 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; ppc64le

```console
$ docker pull php@sha256:5069ff0804fe06c7bc9509d82748cae4c604a34e3d1636733521eed7c82b264f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150482767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7764b50c70aebfb8c1c65fbf5344c13432cb82c9b3abf97d9bd13b32b2391413`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:07:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 20:08:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 20:12:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:12:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 20:12:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 20:50:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 20:51:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 20:51:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 20:51:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 22:08:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 22:08:47 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 22:08:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 22:08:54 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 22:10:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 22:11:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 22:15:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 22:15:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 22:15:58 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 22:16:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 22:16:05 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbb63881ed3aea74b5666bddbed760e2efb176d46887dffeaaad47865b97e86`  
		Last Modified: Wed, 18 Aug 2021 01:00:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99be8a44948af202f4c13e5f1ac9bca6d60ee898dd4fb70b92f36cfd380de14a`  
		Last Modified: Wed, 18 Aug 2021 01:01:26 GMT  
		Size: 82.3 MB (82290875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd90ce4a2fb80614fa9611ab92d7169578640316dfda1eabf6a877dcd89f487`  
		Last Modified: Wed, 18 Aug 2021 01:00:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033ff50223f08ed67f6d4f9bdea10bdebd5f48a99853b0da0d87c6cc47ed3368`  
		Last Modified: Wed, 18 Aug 2021 01:09:39 GMT  
		Size: 11.0 MB (11000071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e5ecb1c878523b2d482620c24b11cb145c8b22688e34dd0ea4adc6cfb96953`  
		Last Modified: Wed, 18 Aug 2021 01:09:34 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cc21d5d26da9ba60b25a8c66067d8574a758b60a3b49baab4d6f0c2cf286f6`  
		Last Modified: Wed, 18 Aug 2021 01:09:49 GMT  
		Size: 26.6 MB (26634591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbc02109412838bff2ed53519b5242d7c799c23fe676be144020396564cec7e`  
		Last Modified: Wed, 18 Aug 2021 01:09:34 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57292c121e90ea1b85ec8c57d687df95476154c18f6f417fef72ab70cb3c6a4`  
		Last Modified: Wed, 18 Aug 2021 01:09:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-buster` - linux; s390x

```console
$ docker pull php@sha256:c03aae9789b034480c3f2ef836b16134c1a94f1cea445378b96b5b4d5c1c60b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126141162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96cb24db7d46b885140fcf92a5f03aa41031ff9b6dfb8b17ae292da7da0cbe72`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:14:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 08:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 08:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:15:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 08:15:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 08:24:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-zts --disable-cgi
# Tue, 17 Aug 2021 08:24:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 08:24:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 08:24:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 08:46:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 17 Aug 2021 08:46:06 GMT
ENV PHP_VERSION=8.0.9
# Tue, 17 Aug 2021 08:46:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Tue, 17 Aug 2021 08:46:07 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Tue, 17 Aug 2021 08:46:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 08:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 08:49:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 08:49:37 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 17 Aug 2021 08:49:38 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 08:49:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 08:49:39 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b509377d804e99fd3d8c5eb11fdcb06ac0592b467e1a5d34f296426a6cec6a14`  
		Last Modified: Tue, 17 Aug 2021 09:47:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef8dd0e3b36bc333683aafc6e422e5b3a9294feb703deb0a71a749175c45da6`  
		Last Modified: Tue, 17 Aug 2021 09:47:10 GMT  
		Size: 64.7 MB (64710852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b280bc6a9cfb9647c076d519d4cb4187708961862386bd0840ea7453ef0e7992`  
		Last Modified: Tue, 17 Aug 2021 09:47:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393f667c5b75362dadbba0c3ce61c050adda3799fa3120351f64609fc0146a81`  
		Last Modified: Tue, 17 Aug 2021 09:49:58 GMT  
		Size: 11.0 MB (10998297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40b57ca9a88f3dbe154b9c53b9e52a24506cfe2cc55665d95484c3d845bf9fe`  
		Last Modified: Tue, 17 Aug 2021 09:49:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ccf1a7b5439f7cc8bc42cc7486be351632cf4c0ab00f56a2becce97e8aea94`  
		Last Modified: Tue, 17 Aug 2021 09:50:01 GMT  
		Size: 24.7 MB (24667662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8486d6f915585b29a5ddaca2ba7198b2c52973baa7cf267556cceae1dab24156`  
		Last Modified: Tue, 17 Aug 2021 09:49:57 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f03c19fe2ed7919b6ca26a82012f7d8fb9bb2bcb15bf29e1e680c4845f5442`  
		Last Modified: Tue, 17 Aug 2021 09:49:57 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
