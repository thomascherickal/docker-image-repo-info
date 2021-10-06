## `php:7-zts-buster`

```console
$ docker pull php@sha256:9fcbf32eb3db4ccd4258354c961b720e22b3731fee2adc5beb54e90a6e795aef
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

### `php:7-zts-buster` - linux; amd64

```console
$ docker pull php@sha256:8259923a61c8eb1984e3a00ba900d4e0af6a30c7777ac8e845831dc14f3a8387
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140048702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd5a809837320d9a3bc1cf47d23407ae00b3e16930361d45cd084ab90df43df`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 14:09:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 14:09:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 14:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 14:10:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 14:10:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 16:23:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 28 Sep 2021 16:23:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 16:23:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 16:23:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 16:23:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 16:23:21 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 16:23:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 16:23:22 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 16:23:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 16:23:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 16:30:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:30:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 16:30:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 16:30:17 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815fd546abc9ddfff4d51c04a1a23dd4dfaeb7cc97bd3bfd2ff16c29efa926dc`  
		Last Modified: Tue, 28 Sep 2021 17:16:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860ed1b5b2bd43b112c3f76d417cbc0a8e56856076eeed83e30453f0ca5cb2d`  
		Last Modified: Tue, 28 Sep 2021 17:16:37 GMT  
		Size: 76.7 MB (76681149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7cb65357dc94c36bd249a314d8a60031a13dca9ab7a33bad789de68e0fe910`  
		Last Modified: Tue, 28 Sep 2021 17:16:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18b67d9e4c7e114a8da7610e2462859981b872fa0ce4a41582ea5002d1661fb`  
		Last Modified: Tue, 28 Sep 2021 17:25:17 GMT  
		Size: 10.7 MB (10694516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dda73d6cf89ab35514418f9cd1cfd160e751c1c744bc75ee54d0eb40a82343`  
		Last Modified: Tue, 28 Sep 2021 17:25:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aad6d48d02b48bd35a2c92b46c3e4fcc4ef7f22b0cca607e760af7fdc92e7c`  
		Last Modified: Tue, 28 Sep 2021 17:25:20 GMT  
		Size: 25.5 MB (25523537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d93131ed3f647cdfb154992fc9715b47d30cbcbba91464c2d09f46a442310a`  
		Last Modified: Tue, 28 Sep 2021 17:25:16 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb8ecadfc97aff6b22da611c8796595043008ad5883e833ba87705d7367c7d7`  
		Last Modified: Tue, 28 Sep 2021 17:25:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; arm variant v5

```console
$ docker pull php@sha256:cf863a1912c695fe16f7c46bc8f332630639e348746fd5c13de8752a567eb4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118943847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5086cabfab8a912958fafc4b60b84fe5c9c44166d1c158073c0d8900326d2b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:42 GMT
ADD file:6524935705c59a0eda67f61fe1005a28b4b388258e2d5636dd5b831333200dc8 in / 
# Tue, 28 Sep 2021 01:51:43 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:06:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 15:06:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 15:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:07:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 15:07:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 16:54:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 28 Sep 2021 16:54:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 16:54:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 16:54:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 16:54:40 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 16:54:40 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 16:54:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 16:54:41 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 16:55:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 16:55:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 17:00:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 17:00:20 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 17:00:22 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 17:00:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 17:00:22 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:85d14771cf32dc23d1c8e99a9aad844b3db9d67f4781455c81749ffe43b05513`  
		Last Modified: Tue, 28 Sep 2021 02:08:05 GMT  
		Size: 24.9 MB (24879067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac47101a1ea177a2844f3bf9238e07c44ef5b41cf0419c4a2591cd0b080a200`  
		Last Modified: Tue, 28 Sep 2021 18:00:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8744e3acdc9cec2d0248cd31a3489c41bbdce73f967ae1f71ded9cb228e1349`  
		Last Modified: Tue, 28 Sep 2021 18:00:43 GMT  
		Size: 58.8 MB (58821224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a48f114b54f24bf5a5c00d0f673f755ce42b6e201edb2520018225c7afa25f8`  
		Last Modified: Tue, 28 Sep 2021 18:00:02 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7fbf8e74fdc1cef35b0fb45e4b88a13fa693e79036ada9071b554a3c3624f`  
		Last Modified: Tue, 28 Sep 2021 18:17:14 GMT  
		Size: 10.7 MB (10692277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfbd0c0114dc0b4c332ddb1f4dae94226a9c581daa614e4004f44c52a93bf6c`  
		Last Modified: Tue, 28 Sep 2021 18:17:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018be87e006fb24c9e31c9e0d4b59b03d0ce160961fddb810818f7148a0e0c0a`  
		Last Modified: Tue, 28 Sep 2021 18:17:27 GMT  
		Size: 24.5 MB (24547774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47b41f33e38a9ced41a04704d871c90a39a07eaff72cd3d9127f5c6d52eb293`  
		Last Modified: Tue, 28 Sep 2021 18:17:12 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b9d6976bad79a592e0545fec34d15953ce55e03f721116f2d4d1a784d7c5e2`  
		Last Modified: Tue, 28 Sep 2021 18:17:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:1eddc4dfce668755645a5f9ba69e7e1dd7b3889ae1a6916b2c2428b23d579c4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116713408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5532b425c4469bcb3d621a9f3147b3996d11441d18f5a90613b59b70ab10542d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:11 GMT
ADD file:e71f315aa894d483f75b32109fff32974c43ce2e684cd28eb6492bc6fc450931 in / 
# Thu, 30 Sep 2021 18:04:12 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 07:32:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 01 Oct 2021 07:32:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 01 Oct 2021 07:33:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 07:33:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 01 Oct 2021 07:33:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 01 Oct 2021 09:33:15 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Fri, 01 Oct 2021 09:33:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Oct 2021 09:33:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Oct 2021 09:33:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 01 Oct 2021 09:33:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 01 Oct 2021 09:33:17 GMT
ENV PHP_VERSION=7.4.24
# Fri, 01 Oct 2021 09:33:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Fri, 01 Oct 2021 09:33:18 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Fri, 01 Oct 2021 09:33:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 01 Oct 2021 09:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:38:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Oct 2021 09:38:29 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:38:31 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Oct 2021 09:38:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Oct 2021 09:38:32 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:421f17c521234da0c5b07d4f6e44314149dc3790ef12134e85e61741452c9f96`  
		Last Modified: Thu, 30 Sep 2021 18:20:50 GMT  
		Size: 22.7 MB (22746246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5641096c59071429c7049e0a56b96248a9c5b5a0602ce5a6ba2759e4aa2c6834`  
		Last Modified: Fri, 01 Oct 2021 10:45:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34d253e914adbe6836b8bb6d270843021c149273390997f6f27515250a1ffe`  
		Last Modified: Fri, 01 Oct 2021 10:46:36 GMT  
		Size: 59.5 MB (59515650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8c9a413d0316c765600e4964f6ac594e9f6b6e07bb8aa09e8ee94c3bd04ea0`  
		Last Modified: Fri, 01 Oct 2021 10:45:59 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccba2b7acc2575daa48cd8376ee34f3f64a925e1b1706b3c433f91a998d765c`  
		Last Modified: Fri, 01 Oct 2021 11:02:59 GMT  
		Size: 10.7 MB (10692268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8d743c1d1355e6eb45db9b87b332520e313c00aa6fdebcd8c0f836fbca011b`  
		Last Modified: Fri, 01 Oct 2021 11:02:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a134b14480ff41d43cdeef88a72673b964c68e8b3a52301428cae6337e48508`  
		Last Modified: Fri, 01 Oct 2021 11:03:11 GMT  
		Size: 23.8 MB (23755739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c837cac2c1aa3856c43d697ad8b60d21f851261a8c71b412373cf4c450c967ee`  
		Last Modified: Fri, 01 Oct 2021 11:02:56 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f7e359b5fd3cdb717b2cd228b784fecfba5e82243031f448982c853124d69c`  
		Last Modified: Fri, 01 Oct 2021 11:02:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:9443af4e1fdc3979564cd5f94cecdd77ac4d60ce4751bec14591e42f47dad28a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132275074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0445686739325b0e0a99f8464e21b6620cad5eff911f58386dea594b8ce69646`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:03:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 09:03:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 09:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:03:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 09:03:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 10:22:07 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 28 Sep 2021 10:22:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 10:22:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 10:22:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 10:22:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 10:22:08 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 10:22:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 10:22:08 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 10:22:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 10:22:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:26:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 10:26:05 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:26:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 10:26:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 10:26:06 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b35a86ab1457a11a2b4250ccd7fc7d2055bca36ae4977bb4ca142a6ccc282a9`  
		Last Modified: Tue, 28 Sep 2021 11:05:50 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58411526b4c384b02c019d7de41d51086a2bcc8a27082f904e905478b1ae523`  
		Last Modified: Tue, 28 Sep 2021 11:06:01 GMT  
		Size: 70.4 MB (70356720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4637358d71d7946b8a93b46f810bf3a92817cce3132b12e12de9cd3e0b9d7b0`  
		Last Modified: Tue, 28 Sep 2021 11:05:50 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d195f7ed13f01c1b7d67f3703c2342101dcc7481821e7716788e328e0e05d318`  
		Last Modified: Tue, 28 Sep 2021 11:16:21 GMT  
		Size: 10.7 MB (10693008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fb32df461a000fd9c9ce370321a700844274a31cf6acc3a5a736746ba23623`  
		Last Modified: Tue, 28 Sep 2021 11:16:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088047ea9a729c6ae29f12b8c9dbb8fb4de1d91a13e3899f0387556ec615c477`  
		Last Modified: Tue, 28 Sep 2021 11:16:25 GMT  
		Size: 25.3 MB (25306809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860820cae2b78f50a38269539882e60ecf18ecfa5305f94abce5d780ceddb766`  
		Last Modified: Tue, 28 Sep 2021 11:16:21 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a2eb8e12b0652786411e33c797f32ec0180bb7956369fddad8496e5389b20b`  
		Last Modified: Tue, 28 Sep 2021 11:16:20 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; 386

```console
$ docker pull php@sha256:f44d75ce35b4fa52151090f5204c08ab57be3ff6216921ab21fc46b85cffffcf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.8 MB (145798158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51de9bfbabdf5ef1de8bb1b894dac97a8ea960d58a64866241a1f95bbfa0a7b5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:49 GMT
ADD file:c090abbb3afcfebf797e06e2ac4b778acb4e97d5dca79c29d1927f43cf14b23e in / 
# Tue, 28 Sep 2021 01:40:49 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 13:19:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 13:19:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 13:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 13:20:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 13:20:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 15:39:05 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 28 Sep 2021 15:39:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 15:39:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 15:39:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 15:39:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 15:39:07 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 15:39:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 15:39:08 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 15:39:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 15:39:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:45:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 15:45:59 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:46:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 15:46:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 15:46:01 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:82f7c8b98609aee82696182c03cb09ae62ceab1b17f8eec1e233a68180876d41`  
		Last Modified: Tue, 28 Sep 2021 01:50:06 GMT  
		Size: 27.8 MB (27797629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede349f021642655631250b04dbc18b6b8ecca6cf158e90bdbb94e31cabf201`  
		Last Modified: Tue, 28 Sep 2021 16:55:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78136b891d9a1d22d9233d2f5448cb1557a37e0bf8d062a9f9b61f68141939f2`  
		Last Modified: Tue, 28 Sep 2021 16:56:18 GMT  
		Size: 81.2 MB (81229337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eede2d4a61188f319e769095f2738a68eafdb2300f4a88fb0cf6becf68c22021`  
		Last Modified: Tue, 28 Sep 2021 16:55:56 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976287100f3100f2bc4ced3a62039836eab46ac45448011227e826d506cef19c`  
		Last Modified: Tue, 28 Sep 2021 17:09:35 GMT  
		Size: 10.7 MB (10693720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2fdc699565ac9c414bf8792cff2503faaf8f71b106d762f0f2a289bc87fb3e`  
		Last Modified: Tue, 28 Sep 2021 17:09:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3bb54b736bb10bcec2ac4b101bff2ec4e7986f8e2df7dbd530d03f2aacb34d`  
		Last Modified: Tue, 28 Sep 2021 17:09:40 GMT  
		Size: 26.1 MB (26073972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833acba338a4c9d54ac0f3a9f4a08f185b888afe89419f7d59cb23cb1e1d6402`  
		Last Modified: Tue, 28 Sep 2021 17:09:34 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3c1482bcb8e2ddab51e6baad522d0451b1372a60ed110886bfb7dbca70357`  
		Last Modified: Tue, 28 Sep 2021 17:09:34 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; mips64le

```console
$ docker pull php@sha256:49c8a73def27d1df9b9eeb6fbaf495c1d454ca4e5e72f6b4634aa5496d1f6791
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122918228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16c223ffa3d596759f2528f110f257e889b6bb62e82f5a376c481396ffcd7d9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 19:03:01 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 05 Oct 2021 19:03:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 05 Oct 2021 19:03:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 19:03:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Oct 2021 19:03:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Oct 2021 22:58:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 05 Oct 2021 22:58:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 22:58:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 22:58:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Oct 2021 22:58:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Oct 2021 22:58:32 GMT
ENV PHP_VERSION=7.4.24
# Tue, 05 Oct 2021 22:58:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 05 Oct 2021 22:58:32 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 05 Oct 2021 22:58:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 22:58:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Oct 2021 23:12:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Oct 2021 23:12:02 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 05 Oct 2021 23:12:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Oct 2021 23:12:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Oct 2021 23:12:05 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97482b9702e94158168dfe828302e0e07d5941e445bf5649a223dd9f41ece0b`  
		Last Modified: Wed, 06 Oct 2021 00:47:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0ee1bf02fb39d0d73992f19f8aa1ace60e779c8e9029bc2ba75a1c0ab4b27`  
		Last Modified: Wed, 06 Oct 2021 00:48:45 GMT  
		Size: 61.4 MB (61403659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a6516d24ec030d1b47ecdeca599f905cafe5db8651377c07964b70ee0036e`  
		Last Modified: Wed, 06 Oct 2021 00:47:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f97d44f0b7d1b242877519f77164dd279f07660dd5dfc540593b27ce9abecb`  
		Last Modified: Wed, 06 Oct 2021 01:01:40 GMT  
		Size: 10.7 MB (10691543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364b147b655d29b682d7a6ea68fc2be2fc6e23f1cbe5bccf7f0ddb96d4bbc078`  
		Last Modified: Wed, 06 Oct 2021 01:01:37 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81efea211e0c9ab9f85059b537939111cee4122a5426b1951c469ed037e2e8e7`  
		Last Modified: Wed, 06 Oct 2021 01:01:54 GMT  
		Size: 25.0 MB (25006566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5823c0e580caaee01dd77a62027005c7474ea7c0ff7f19591665d67b76eaf`  
		Last Modified: Wed, 06 Oct 2021 01:01:37 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7148d7f78eae94fff829dc5aa1d691f361888cb92a10cd0239a4b1b8884f08d6`  
		Last Modified: Wed, 06 Oct 2021 01:01:37 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; ppc64le

```console
$ docker pull php@sha256:71c676debfd401fbdac0aa95cfddd6bb9e702f0e71d26f661ca01f33dc5fbf3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150347561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f16b79ddff2ac681295ec8e416482c50623453a43ab42adbd401acad6206497`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 02:27:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 05 Oct 2021 02:27:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 05 Oct 2021 02:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 02:32:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Oct 2021 02:33:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Oct 2021 06:11:26 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 05 Oct 2021 06:11:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 06:11:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 06:11:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Oct 2021 06:11:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Oct 2021 06:11:44 GMT
ENV PHP_VERSION=7.4.24
# Tue, 05 Oct 2021 06:11:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 05 Oct 2021 06:11:54 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 05 Oct 2021 06:13:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 06:13:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Oct 2021 06:19:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Oct 2021 06:19:08 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 05 Oct 2021 06:19:22 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Oct 2021 06:19:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Oct 2021 06:19:35 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5bb0e399334e40c90da8aea82dee066d6b56d1d6141ea84ff56062903ac086`  
		Last Modified: Tue, 05 Oct 2021 07:37:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0076a8ad1cfe3f9dd6fc7c53ff5948a137e948063b5c59aeb48186024acc8eff`  
		Last Modified: Tue, 05 Oct 2021 07:37:18 GMT  
		Size: 82.3 MB (82292002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93b47eab4c8230fa6b2d3c4ef1f6b3575b09e3264c579d088c920a88e6f12e`  
		Last Modified: Tue, 05 Oct 2021 07:37:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e777e2d44f919b0a11d6d451aacdda53a84e8bb19db45aecdbd1672ad519fd2b`  
		Last Modified: Tue, 05 Oct 2021 07:48:42 GMT  
		Size: 10.7 MB (10694298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874646db252afae1480daa79aec6f824d49fbdfc25f620dc441b638e268c6ca7`  
		Last Modified: Tue, 05 Oct 2021 07:48:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8837b480c611d785c37d592c9b8b0865f36fc78f4054855a56cfbffcd34e948`  
		Last Modified: Tue, 05 Oct 2021 07:48:45 GMT  
		Size: 26.8 MB (26804022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab67c9e5219d4a4282dcb94a13da905dc35517ae11ea41d5b45d7982299b8a`  
		Last Modified: Tue, 05 Oct 2021 07:48:40 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f423d5157ba278bca008a4546bdbd1487125e55a23036613284d9cd9bc552e`  
		Last Modified: Tue, 05 Oct 2021 07:48:40 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-buster` - linux; s390x

```console
$ docker pull php@sha256:879c94e3b3bece6fdc804484920ea789e6ee5222a4458f356cbee5ecc21cff21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126122181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c49cb21f14cef6bf6a0cb9c4fee34c4b92ac23b243f56e7b9a49946e1a5bcbfe`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:54:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 05:54:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 05:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:54:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 05:54:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 06:41:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Tue, 28 Sep 2021 06:41:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 06:41:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 06:41:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 06:41:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 06:41:33 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 06:41:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 06:41:33 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 06:41:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 06:41:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:43:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 06:43:52 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:43:52 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 06:43:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 06:43:52 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b76cd23951c492c8e2173a040e37c99137663c238bb4676be1b20cd0aa79a23`  
		Last Modified: Tue, 28 Sep 2021 07:13:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ecfc599bf380f4f380b456fd0f21d532486d8c06bcca669ff770fabbed286`  
		Last Modified: Tue, 28 Sep 2021 07:14:05 GMT  
		Size: 64.7 MB (64711834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa51e922d4723fd053e815145ccb1fdb121a98e1e7023f9d0f45afdcc1a800e`  
		Last Modified: Tue, 28 Sep 2021 07:13:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48718b50e9c67341d8751ee449756d6515d0a6fa786e70190c0559cd64c14d41`  
		Last Modified: Tue, 28 Sep 2021 07:20:32 GMT  
		Size: 10.7 MB (10692513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa866a341f668c96ea11e618944dfa7e5272a047243f07011d4d0005d950c59`  
		Last Modified: Tue, 28 Sep 2021 07:20:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd379d77c7648a636913a484c4fe3948c91b03847a5d05faaef00edc0a3d95d`  
		Last Modified: Tue, 28 Sep 2021 07:20:34 GMT  
		Size: 25.0 MB (24953461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937528b8f881952dfae3c93376d2069edab88f29226782bc9e4722c410710ec5`  
		Last Modified: Tue, 28 Sep 2021 07:20:31 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bc62a3ec2b5c2f4471e147c7a37f9202e0f10b83754a31fe0a05b8a9319101`  
		Last Modified: Tue, 28 Sep 2021 07:20:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
