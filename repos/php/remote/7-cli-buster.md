## `php:7-cli-buster`

```console
$ docker pull php@sha256:aa32e02ff5e21d18981f6f3f2cd427ba114a24ae40c3cd08690430d9a6998b60
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

### `php:7-cli-buster` - linux; amd64

```console
$ docker pull php@sha256:c51d37e6aabcd7c2914442c30590dc74f340d1e1a1f4065df63b785335fafcc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147581740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c115b40286e269ba238b757a694acd3f16469255411388ba7871fc794ee380c0`
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
# Tue, 28 Sep 2021 14:10:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 28 Sep 2021 14:10:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 14:10:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 14:10:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 16:07:12 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 16:07:12 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 16:07:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 16:07:13 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 16:07:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 16:07:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:12:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 16:12:35 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:12:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 16:12:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 16:12:37 GMT
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
	-	`sha256:ccb4d4d6b0a95a5ca661becf695a747e9d54b1d5c8e12c99d06485a445f3fb70`  
		Last Modified: Tue, 28 Sep 2021 17:24:14 GMT  
		Size: 10.7 MB (10694537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfdbb8df0816b8298254f9280691138c75246d92cee692878c3d57caf7beaf9`  
		Last Modified: Tue, 28 Sep 2021 17:24:13 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a40390e27aa3a7f57f6aeb3598ec69be232d9508010311bf2583aceead9f273`  
		Last Modified: Tue, 28 Sep 2021 17:24:19 GMT  
		Size: 33.1 MB (33056556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7190fdde58a67010877718f7bc7fcaf80ec143d7c15fa8537ed982446a109d6`  
		Last Modified: Tue, 28 Sep 2021 17:24:13 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0450a53f4597b9a71fe8630ca2083ccfec022d1b9e3fde637391d7a774df642`  
		Last Modified: Tue, 28 Sep 2021 17:24:13 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; arm variant v5

```console
$ docker pull php@sha256:41ff06469a5c31ce204953afa3838958410357d5b4d8c48e763229a93b1f3137
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125844474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40758a429c163f7d9af8f5a64c746992cb5e812cb42c1d7b8ddcf21cfc90e165`
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
# Tue, 28 Sep 2021 15:07:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 28 Sep 2021 15:07:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 15:07:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 15:07:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 16:38:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 16:38:49 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 16:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 16:38:49 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 16:39:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 16:39:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:43:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 16:43:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:43:24 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 16:43:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 16:43:25 GMT
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
	-	`sha256:82d265e7010fbabd2f08f6745c32878f618dd5c5ae24072ffcc49e65c9edc545`  
		Last Modified: Tue, 28 Sep 2021 18:15:21 GMT  
		Size: 10.7 MB (10692266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293ca2d2794147d272c4bbd95de6d864387073d473903e94bafbb0f9b16b465`  
		Last Modified: Tue, 28 Sep 2021 18:15:18 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8092c87bb7872541208b81daacf9465d6f057d3e55eb998416d203038c1745`  
		Last Modified: Tue, 28 Sep 2021 18:15:38 GMT  
		Size: 31.4 MB (31448415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52581aeaba7ba11f14fe9849c85fe0c7c28afa049e85e5693fd91314b60452f2`  
		Last Modified: Tue, 28 Sep 2021 18:15:18 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02e52d570e0d0b1ff8ae827aeb3dc9a4a3acf2bbd08688a558594b6d7176ed8`  
		Last Modified: Tue, 28 Sep 2021 18:15:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:66a6980798f2c98b6669f42dddeecfd490a1f97e0510f0043f4e0082b7e623ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123205439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76928b1584ee705bcf4f163992c2f36574e49cfb0cb5585968f3e179f2ed514c`
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
# Fri, 01 Oct 2021 07:33:41 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Fri, 01 Oct 2021 07:33:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Oct 2021 07:33:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Oct 2021 07:33:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 01 Oct 2021 09:17:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 01 Oct 2021 09:17:58 GMT
ENV PHP_VERSION=7.4.24
# Fri, 01 Oct 2021 09:17:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Fri, 01 Oct 2021 09:17:59 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Fri, 01 Oct 2021 09:18:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 01 Oct 2021 09:18:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:22:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Oct 2021 09:22:25 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:22:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Oct 2021 09:22:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Oct 2021 09:22:28 GMT
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
	-	`sha256:e2fb7315db5aea7f4e3af9635be7abfd6faec94c3ffbbbb13a39fd2d40f5d83c`  
		Last Modified: Fri, 01 Oct 2021 11:01:14 GMT  
		Size: 10.7 MB (10692259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a47416e31aabab22eec3e4b5fc3d93b851a6192b15ea97cdd192afcb9cb45c`  
		Last Modified: Fri, 01 Oct 2021 11:01:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219667de2e07ea8625f7003fefcf382c173e90ffac0085d320f21b064a356900`  
		Last Modified: Fri, 01 Oct 2021 11:01:30 GMT  
		Size: 30.2 MB (30247780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac0807e606681d096bd9ebc96b4420196c53cba51df006cd41822276ce3dbf0`  
		Last Modified: Fri, 01 Oct 2021 11:01:11 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e889ef985da05f311c2024ccd9ccc3e554b0ac55659565d62246aefa8ac665a0`  
		Last Modified: Fri, 01 Oct 2021 11:01:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:71b0a02ad12e65de373aa0218f1b558c3cbf635381c188a4fdce735634474ce1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139608765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4ea81fc8c13e90d5a7cfc4ffdf54a1be660cd2d6cdab6aadf7c27955b9eec5`
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
# Tue, 28 Sep 2021 09:03:36 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 28 Sep 2021 09:03:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 09:03:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 09:03:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 10:12:15 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 10:12:15 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 10:12:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 10:12:15 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 10:12:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 10:12:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:14:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 10:14:49 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:14:49 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 10:14:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 10:14:50 GMT
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
	-	`sha256:3f83ee2e4338b9136868f24dee402d5ffeb1f3245c6e55b01c47b021f2162344`  
		Last Modified: Tue, 28 Sep 2021 11:15:08 GMT  
		Size: 10.7 MB (10692987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1407b62d0fe6f2daa1fea6a10bdaf12690a2ad2135e85d3b4f2c9b306be8510a`  
		Last Modified: Tue, 28 Sep 2021 11:15:08 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4979dea18a3b8cc00605cd55797504ea6600656fd9169ee286016a5a8f99a541`  
		Last Modified: Tue, 28 Sep 2021 11:15:13 GMT  
		Size: 32.6 MB (32640519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ecbde140b53a5e55a06a6290f4dd5e576753263c4cd320afed7156dc7607df`  
		Last Modified: Tue, 28 Sep 2021 11:15:07 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fb9548338816203d4c55ef56992a157c2401539c51c7141f41b0c2fa81b2c9`  
		Last Modified: Tue, 28 Sep 2021 11:15:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; 386

```console
$ docker pull php@sha256:2cbe013395229a453d786aa9b47ed3e7af6f1e6d0c96c0f0e9d0d8b4fa239a3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153593571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dc890cb84c9f88527db54da291801521f2fafc6aa5c7826a72c2446d3a0c6b3`
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
# Tue, 28 Sep 2021 13:20:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 28 Sep 2021 13:20:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 13:20:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 13:20:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 15:21:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 15:21:02 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 15:21:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 15:21:02 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 15:21:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 15:21:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:26:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 15:26:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:26:42 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 15:26:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 15:26:43 GMT
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
	-	`sha256:fae941ab072ec3b3fa2bd7687fc96b40244d5991b245d961811f5c10c3345798`  
		Last Modified: Tue, 28 Sep 2021 17:08:08 GMT  
		Size: 10.7 MB (10693699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8349c90127afc331946b8ef1b22f1641309da9fe05adcc640fbeb62b585076d`  
		Last Modified: Tue, 28 Sep 2021 17:08:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a40df6ec134692849bf3338d4230b393ae96529484f4c3eab288b6c8333b6`  
		Last Modified: Tue, 28 Sep 2021 17:08:18 GMT  
		Size: 33.9 MB (33869405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b6f28a38cae4b83f5e877a7dc7b81fb9fae4e11dd60b2ca72e51a7d6d040c`  
		Last Modified: Tue, 28 Sep 2021 17:08:06 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779fb98b11d4655887dd252f62bef600f3e5854b087e3ae682077c76853db5f6`  
		Last Modified: Tue, 28 Sep 2021 17:08:06 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; mips64le

```console
$ docker pull php@sha256:83facb4e0bb71b01bf64ed0af69d557b2d8f366a5fd443ed4288350cc7b6f146
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129984340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe768122171c60d46fc6cd97d88b10fbceac311f39a2c477675238389320217`
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
# Tue, 05 Oct 2021 19:04:00 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 05 Oct 2021 19:04:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 19:04:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 19:04:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Oct 2021 22:27:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Oct 2021 22:27:48 GMT
ENV PHP_VERSION=7.4.24
# Tue, 05 Oct 2021 22:27:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 05 Oct 2021 22:27:49 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 05 Oct 2021 22:28:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 22:28:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Oct 2021 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Oct 2021 22:36:06 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 05 Oct 2021 22:36:08 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Oct 2021 22:36:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Oct 2021 22:36:09 GMT
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
	-	`sha256:66d6081a419fee0ef5ddf25e506cc64f9dc4c70e17c6583167316eec33936e57`  
		Last Modified: Wed, 06 Oct 2021 00:59:55 GMT  
		Size: 10.7 MB (10691548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e26c78b9577ba51fc6550f4943ec3e6d8d4b16599f02d8f2bd9432b4eb814e`  
		Last Modified: Wed, 06 Oct 2021 00:59:52 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72485bce5978e3d8f11789db63a1346e21f974d4522822b5b5620744a6f981da`  
		Last Modified: Wed, 06 Oct 2021 01:00:15 GMT  
		Size: 32.1 MB (32072673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e5371444388a8e14976306d5c086148155f034c2d1120e4b9e7553a3f72892`  
		Last Modified: Wed, 06 Oct 2021 00:59:52 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de758b164ff8c17ffa4cd38b2f135ab7a815158cba2efd3af1ba6cfc32b147d`  
		Last Modified: Wed, 06 Oct 2021 00:59:52 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; ppc64le

```console
$ docker pull php@sha256:8cd31a16e19d556c36859e627d334d8d486d7a40af678c5369dc2bdd6cb69bc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.5 MB (158505531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89cc2aa4da791a9e23db150600a078c06afb3b573daad68e4888124b448bede8`
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
# Tue, 05 Oct 2021 02:33:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 05 Oct 2021 02:33:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 02:33:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 02:33:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Oct 2021 05:43:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Oct 2021 05:43:29 GMT
ENV PHP_VERSION=7.4.24
# Tue, 05 Oct 2021 05:43:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 05 Oct 2021 05:43:38 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 05 Oct 2021 05:44:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 05:44:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Oct 2021 05:48:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Oct 2021 05:48:46 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 05 Oct 2021 05:49:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Oct 2021 05:49:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Oct 2021 05:49:11 GMT
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
	-	`sha256:9771a558ed1eabbf3706b62e1ae25608d10a236d0d20a3f27d14bd800bf246ad`  
		Last Modified: Tue, 05 Oct 2021 07:47:30 GMT  
		Size: 10.7 MB (10694262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3d62ab71017d36bffeeb41fc19a3505d2ef51a37d62d0aacb200a6c295134e`  
		Last Modified: Tue, 05 Oct 2021 07:47:29 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e0d78a84c027b2c45f2ec9c5075cc8d3acd396b530aa6041181dce5a7ba2f5`  
		Last Modified: Tue, 05 Oct 2021 07:47:36 GMT  
		Size: 35.0 MB (34962031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ef1193295a10de2aa1d712bcfd8ad54cc8c193b4f70afbf9332688778fd980`  
		Last Modified: Tue, 05 Oct 2021 07:47:29 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b848c62992eb97a11c7243bb22f43866d692cea5718b5dae6f723d390019cc7e`  
		Last Modified: Tue, 05 Oct 2021 07:47:29 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-buster` - linux; s390x

```console
$ docker pull php@sha256:8fb8ff22b3aef4740a1a4136f949f599aae24264fdc7020e8fc6f21ebf20b7d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (133036348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ad9bf23db9d2f0439d481d847ce9cc1c624edcd8d903abc089becb7e132878b`
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
# Tue, 28 Sep 2021 05:54:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-embed
# Tue, 28 Sep 2021 05:54:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 05:54:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 05:54:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 06:35:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 06:35:24 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 06:35:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 06:35:25 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 06:35:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 06:35:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:36:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 06:37:00 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:37:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 06:37:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 06:37:00 GMT
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
	-	`sha256:c23b361bf4ef9e33645349b8d07202e880196b157daaed831e958e0c216ba1b2`  
		Last Modified: Tue, 28 Sep 2021 07:19:50 GMT  
		Size: 10.7 MB (10692493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e04ffa48749545d7362024288817620a683183288c9763a16966c41f9d3ba`  
		Last Modified: Tue, 28 Sep 2021 07:19:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f14c9ce376d4564d72a0d4cb080b10498025c57f8d9b5f2ae5d5e40734569e`  
		Last Modified: Tue, 28 Sep 2021 07:19:54 GMT  
		Size: 31.9 MB (31867650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad13a3d3369b767806a96c97f9b4ef7d376ab3f46cd767fba502ec1db30de9e0`  
		Last Modified: Tue, 28 Sep 2021 07:19:50 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3dab0d0a482d4ecbd1b0e850831570c81b622f82db631ccfb413a9a6aa7fe8`  
		Last Modified: Tue, 28 Sep 2021 07:19:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
