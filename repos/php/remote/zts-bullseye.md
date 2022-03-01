## `php:zts-bullseye`

```console
$ docker pull php@sha256:89dfa684bb0540beb082082df584e5f185b3c2e1f56a40664dac50c67b796698
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

### `php:zts-bullseye` - linux; amd64

```console
$ docker pull php@sha256:a6a6779eeacd2b46ebae49e526de7caa047f78c51b7cebcd669bd7082cd03e0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165270689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187cb5505b210ae89a361e1ceb7362b67d0643a36babc29d149a3ebde1ed0cac`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:17:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 16:17:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 16:18:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:18:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 16:18:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 16:18:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 16:18:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 16:18:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 16:18:35 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Feb 2022 19:20:09 GMT
ENV PHP_VERSION=8.1.3
# Fri, 18 Feb 2022 19:20:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Fri, 18 Feb 2022 19:20:10 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Fri, 18 Feb 2022 19:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Feb 2022 19:22:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Feb 2022 19:45:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Feb 2022 19:45:12 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 18 Feb 2022 19:45:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Feb 2022 19:45:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Feb 2022 19:45:13 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1ad84cf10194e2130f05599fcf95721234f2e72aeb9b2c7341719a0a736e41`  
		Last Modified: Wed, 26 Jan 2022 19:09:25 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c937dadeb7e3e4f156ed8bf156bc07d09c18d255475f602ae6e7c94ad0efc5`  
		Last Modified: Wed, 26 Jan 2022 19:09:41 GMT  
		Size: 91.6 MB (91604421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2f1dc96e597c811b3e8c3d0332b71dd64989ff1f972ffbc477edbc479062f7`  
		Last Modified: Wed, 26 Jan 2022 19:09:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24b294127d92277bee717f595f09adecd28827a26b46d866a69990ac8e1f76b`  
		Last Modified: Fri, 18 Feb 2022 22:55:55 GMT  
		Size: 12.1 MB (12070871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1d71e395855daef1b9117df54e4c14e676c846be666fd0a15d6e4086b52589`  
		Last Modified: Fri, 18 Feb 2022 22:55:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6222d0a4290aa25a18dc00864b327fb194456fb1ac9776eb178c8cc397fed21`  
		Last Modified: Fri, 18 Feb 2022 22:58:12 GMT  
		Size: 30.2 MB (30225588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e83ce2feb0444a072bf7360b5fc525298aaf9c68b40f0c4211a76875602209`  
		Last Modified: Fri, 18 Feb 2022 22:58:06 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abbf0de72b3a8047be4d4d0025d4e0c4d29d801979376ea30ea3662fe38e720`  
		Last Modified: Fri, 18 Feb 2022 22:58:06 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; arm variant v5

```console
$ docker pull php@sha256:a4089b55d740263a03091a119608f7a205d0a0543aa49867e8c0ca192aed5bc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143363501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dca772923fa173b7746bfda41cd67def557217b3b4189fe4d191460f4515740`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:53 GMT
ADD file:eb61ee802e5118b26e1fec2c7fc58e34de0de54a5fd47dc6318c11a039ef528f in / 
# Tue, 01 Mar 2022 02:02:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:18:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 13:18:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 13:18:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:18:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 13:18:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 13:18:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:18:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:18:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 13:18:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 01 Mar 2022 13:18:58 GMT
ENV PHP_VERSION=8.1.3
# Tue, 01 Mar 2022 13:18:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Tue, 01 Mar 2022 13:18:59 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Tue, 01 Mar 2022 13:19:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 13:19:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Mar 2022 13:41:54 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:41:55 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Mar 2022 13:41:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Mar 2022 13:41:56 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4aa6e26b4dfdac27e5b5e15b7ebf4366149755a79dd653a5b68d9d93dd94c695`  
		Last Modified: Tue, 01 Mar 2022 02:18:33 GMT  
		Size: 28.9 MB (28909528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdad6916f037c9d7d3da52a99d3452d403d5845deeb12407caed60f3503c379`  
		Last Modified: Tue, 01 Mar 2022 16:26:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64502c70688d4183009eb799afb394a7ffc43bc7abfab2e2dd3fc4f8a30b268`  
		Last Modified: Tue, 01 Mar 2022 16:26:57 GMT  
		Size: 73.7 MB (73684127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467221c05730cce61a7bc60465100a949657a85c508404a806ab9b6d86305497`  
		Last Modified: Tue, 01 Mar 2022 16:26:08 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9ccb3496151d20c6df571ca1a4ec699500632729b61d03b689a2b56a4e6dc2`  
		Last Modified: Tue, 01 Mar 2022 16:26:10 GMT  
		Size: 12.1 MB (12069119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf1f85295a3fe0aa718bb7e1ec1cc55d77e908088ee18b6a1840db2a91ce4e0`  
		Last Modified: Tue, 01 Mar 2022 16:26:07 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9af564e3c4703374a8523f1d35a995b36d91ca7252095e851e463678e2c4174`  
		Last Modified: Tue, 01 Mar 2022 16:30:07 GMT  
		Size: 28.7 MB (28697194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393b268c0ca2ea411d7848c69903d0c7b5a5390ba213fbd819a168e26aa94af`  
		Last Modified: Tue, 01 Mar 2022 16:29:48 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab8002c4036eb302c0df547ad297669ccf34abbaaf57aa60c894018213802d`  
		Last Modified: Tue, 01 Mar 2022 16:29:48 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; arm variant v7

```console
$ docker pull php@sha256:d69b86b99ec7f06b8a814e1aa8767ebbd28d4e00be3b25a2b8b55a940283e043
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135512923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d11d26167fe71990b6568737259c7afaf4de2b05fafa30aaee8fbf83472f8c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:27:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 03:27:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:28:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 03:28:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 03:28:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:28:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:28:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 03:28:43 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Feb 2022 19:59:24 GMT
ENV PHP_VERSION=8.1.3
# Fri, 18 Feb 2022 19:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Fri, 18 Feb 2022 19:59:25 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Fri, 18 Feb 2022 20:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Feb 2022 20:00:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Feb 2022 20:19:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Feb 2022 20:19:51 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 18 Feb 2022 20:19:54 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Feb 2022 20:19:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Feb 2022 20:19:55 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc9a20cd165cc34bba0c0bab277b6fbf5b727eb38c1b902e577a6f91bdd4980`  
		Last Modified: Wed, 26 Jan 2022 06:36:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e7063615e6e2b8aee21d5be918dc091b1ed4a0792197b96205dcb419f7115b`  
		Last Modified: Wed, 26 Jan 2022 06:37:29 GMT  
		Size: 69.3 MB (69315436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed49ea1bd88a9bbfafb4155619fe90383f2f713205f8bb810a75902408f0d1de`  
		Last Modified: Wed, 26 Jan 2022 06:36:46 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fa05d73dea79137e74bbc6203e6dd5122afa603e7fd9c956e3b714e67ad84`  
		Last Modified: Fri, 18 Feb 2022 22:30:36 GMT  
		Size: 12.1 MB (12069221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01d633f33390bf1060ef67c072b6f6c48fe7e39db31becf08b97b546f29d5c3`  
		Last Modified: Fri, 18 Feb 2022 22:30:33 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13511ab49da3eaf5a010ae1be2f38591066c21fe80e16e0f0b056d9741d1591c`  
		Last Modified: Fri, 18 Feb 2022 22:34:04 GMT  
		Size: 27.6 MB (27559783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a866d5e17b9b5abb74f2e0ba0391fc72f2bb7b542beff06767f0fc98be825d9d`  
		Last Modified: Fri, 18 Feb 2022 22:33:47 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb362be1e6f181fac271720b4362bc89a709e431f0aa9c19625820e6f20e5fd`  
		Last Modified: Fri, 18 Feb 2022 22:33:47 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; arm64 variant v8

```console
$ docker pull php@sha256:564950148c0db767fa70b616c424b3ec481af415989982246df3855356f284ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158883584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddeef798965918a65a24b3b3080222bb0870151c598eabc168c1e87577dd343e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 16:21:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 16:21:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 16:21:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 16:21:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 16:21:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 16:21:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 16:21:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 16:21:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 16:21:54 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 01 Mar 2022 16:21:55 GMT
ENV PHP_VERSION=8.1.3
# Tue, 01 Mar 2022 16:21:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Tue, 01 Mar 2022 16:21:57 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Tue, 01 Mar 2022 16:24:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 16:24:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Mar 2022 16:41:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Mar 2022 16:41:44 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 01 Mar 2022 16:41:44 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Mar 2022 16:41:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Mar 2022 16:41:46 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33762069c180ac7a2bd850df459df42f7dac21d9a3ca6d6b138bd972ceb3b2`  
		Last Modified: Tue, 01 Mar 2022 18:17:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94fc40547e2c4be338f062fc29bcd2c7f19345badf0ff429726978f764df45e`  
		Last Modified: Tue, 01 Mar 2022 18:17:39 GMT  
		Size: 86.9 MB (86920736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63844f2b3ed82fda7e922caee6208b748ab2244bc614e0c7e140f8d6401b15e6`  
		Last Modified: Tue, 01 Mar 2022 18:17:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615f62f8e823cc33dc134c3bc47e3229e70b6c2a218a46f64d802b5cdcc57f7b`  
		Last Modified: Tue, 01 Mar 2022 18:17:26 GMT  
		Size: 11.9 MB (11854474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd416631266a83e62767cbef5e5fdd40a2e771808db989150747aed26294909`  
		Last Modified: Tue, 01 Mar 2022 18:17:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ecd508cbacadcac909cc1c13f40e4e1eca77776c78feeb5f36913bb3602e21f`  
		Last Modified: Tue, 01 Mar 2022 18:19:54 GMT  
		Size: 30.0 MB (30047872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72771c695bb534b0029bc55fac4138285d39cd9f23927d115d4076a6ad7c7`  
		Last Modified: Tue, 01 Mar 2022 18:19:49 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4fad6cdb7080a9d7a3411a65a0830d730a21acb279ba8dfb6f83e2a5703b32`  
		Last Modified: Tue, 01 Mar 2022 18:19:49 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; 386

```console
$ docker pull php@sha256:ac878ffd66f8b0ea1d71c2f3c096b91d7bd31281dcd2d32b5cdd188230e854fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167961164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c0f4a102dbbaecf24034192a499c0f968ed3e87f9d78238246ee3641d43db1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 14:14:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 14:14:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 14:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 14:14:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 14:14:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 14:14:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 14:14:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 14:14:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 14:14:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Feb 2022 19:39:30 GMT
ENV PHP_VERSION=8.1.3
# Fri, 18 Feb 2022 19:39:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Fri, 18 Feb 2022 19:39:31 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Fri, 18 Feb 2022 19:41:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Feb 2022 19:41:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Feb 2022 20:13:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Feb 2022 20:13:57 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 18 Feb 2022 20:13:59 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Feb 2022 20:14:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Feb 2022 20:14:00 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682cda5f75565c6258e6085d20fe17517c28479908d154cff4821d10d2740372`  
		Last Modified: Wed, 26 Jan 2022 17:29:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42ce37ddcafbb43a3972e8a050e538f5b29f470467f9583b9ac7f89c788b90b`  
		Last Modified: Wed, 26 Jan 2022 17:29:59 GMT  
		Size: 92.7 MB (92716286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6499046669fefe00a8c534270eb6528ba2251f36f2953b662450bab9b83a144`  
		Last Modified: Wed, 26 Jan 2022 17:29:35 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a91a0477159387881dda7b009dd74aae492871b9bf1b024bb3f07ff7750771`  
		Last Modified: Fri, 18 Feb 2022 23:30:52 GMT  
		Size: 12.1 MB (12069993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc7f440a34aba47000db05aee9ff7d35bedf3ffeba61d1c340778bad108d41b`  
		Last Modified: Fri, 18 Feb 2022 23:30:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e25799d37cdbea262cc621fbc48f86192bd854126a4973a7aa5f48aac4d602`  
		Last Modified: Fri, 18 Feb 2022 23:33:31 GMT  
		Size: 30.8 MB (30793925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6570fe45c64ed8bf3bad26b3cb2167f231bd830d3e2f064dc27525e69f3ee312`  
		Last Modified: Fri, 18 Feb 2022 23:33:22 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add064d8922227e0a7290a5b6df84b5f86f8d20ee10cc1c9fe0d5ef4e4f2dcd5`  
		Last Modified: Fri, 18 Feb 2022 23:33:22 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; mips64le

```console
$ docker pull php@sha256:f9b0093c6c21ed7c0ed0584776076b6cdac77399653e190718239f3d18b3517c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (142978423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8466cde8ecc0f6c872a9c0507383a49ed37e4a68b7fb7019fc5c54133811ed`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:45:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 12:45:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 12:46:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 12:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 12:46:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 12:46:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 12:46:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 12:46:58 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 01 Mar 2022 12:46:58 GMT
ENV PHP_VERSION=8.1.3
# Tue, 01 Mar 2022 12:46:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Tue, 01 Mar 2022 12:46:59 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Tue, 01 Mar 2022 12:47:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 12:47:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:39:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Mar 2022 13:39:34 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:39:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Mar 2022 13:39:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Mar 2022 13:39:37 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41be42534e478eca62c97e8bdd95d9bb1a5dc902c8ed37895780075718202e65`  
		Last Modified: Tue, 01 Mar 2022 18:54:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b2fc3519286d5ed0d22f002cb6d11887a35f02425c9a63e2ba552baf581e7f`  
		Last Modified: Tue, 01 Mar 2022 18:55:13 GMT  
		Size: 72.0 MB (72014288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cc3e1f5f30f40fb7c8498122710eb5cd05c2f82d6ae2c5a2163897f775363c`  
		Last Modified: Tue, 01 Mar 2022 18:54:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dd45a9fe6a16d7c7dfc95a675d049f4530316e27fc25e6753aa4b3e3ed2641`  
		Last Modified: Tue, 01 Mar 2022 18:54:23 GMT  
		Size: 12.1 MB (12068344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540fb720b9e972296d24e6cca591eceb8a6d2d96903e6146700b43f81aa3ba04`  
		Last Modified: Tue, 01 Mar 2022 18:54:20 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea7bfdd809e1369c377a9f01c9c3f52097f1ba1efc7221a3d325e01b1384ab0`  
		Last Modified: Tue, 01 Mar 2022 18:57:50 GMT  
		Size: 29.3 MB (29259334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867cece67eac41adf37f499605c48d6d96a40bc49d2fed07f575c5c48ef61ab3`  
		Last Modified: Tue, 01 Mar 2022 18:57:31 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2979800c9458c12712a295b115bec0e59c82aacec7c29fdb935c8f6dcd64482`  
		Last Modified: Tue, 01 Mar 2022 18:57:31 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; ppc64le

```console
$ docker pull php@sha256:64c3241d6c0eaf384119a15b52ac8411c32252050914df388bc8e2014d1d2513
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165617918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deabeaecc3c21349c3e3725b17d9837ed4cf1b44f4f034ef7e00cb1892716136`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:29:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 10:29:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 10:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 10:31:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 10:31:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 10:31:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 10:32:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 10:32:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 10:32:05 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Feb 2022 19:17:29 GMT
ENV PHP_VERSION=8.1.3
# Fri, 18 Feb 2022 19:17:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Fri, 18 Feb 2022 19:17:44 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Fri, 18 Feb 2022 19:21:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Feb 2022 19:21:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Feb 2022 19:47:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Feb 2022 19:48:02 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 18 Feb 2022 19:48:12 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Feb 2022 19:48:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Feb 2022 19:48:23 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6353566d57126497241a2d1359b8e40a4aa82b31a4fb89b70b71f25028296b7d`  
		Last Modified: Wed, 26 Jan 2022 13:46:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1c3a5c5a3593cebdd72b812ae7ebe3522a05b2d5522abf096556c638af718`  
		Last Modified: Wed, 26 Jan 2022 13:47:18 GMT  
		Size: 86.6 MB (86624458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824b5fa25d786f0ce5c69716c3b8b6ed693840142dbc489273cfd54b9bf7cd3`  
		Last Modified: Wed, 26 Jan 2022 13:46:29 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a6895117a370713b5bef238edbc6a1acf069507900c5bd3947aca2e7467e6b`  
		Last Modified: Fri, 18 Feb 2022 22:19:55 GMT  
		Size: 12.1 MB (12071188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5bf9b3f1d753223271bd9183f60a3c0d1a6f8e2ac469b77aae5cfd0bf378f6`  
		Last Modified: Fri, 18 Feb 2022 22:19:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f2a96f48ff01ff695065cbb3bf67fba42de0f0eb95bea2bd4d3629962e42f4`  
		Last Modified: Fri, 18 Feb 2022 22:23:10 GMT  
		Size: 31.6 MB (31645695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c309cb2994ac350c46704e85c686ee68b691e9ace110e6ec90a6e028e2c0b0c`  
		Last Modified: Fri, 18 Feb 2022 22:22:50 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e13c6dacff09a39bba635f509eff94006e5261271ff1f543438c486c62a72`  
		Last Modified: Fri, 18 Feb 2022 22:22:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-bullseye` - linux; s390x

```console
$ docker pull php@sha256:dcfcd4b2cd427e15fe4eef8759d3796830613cff469f1c5c02f474c0b1af8f49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142477213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b3789b7ba5b432f48276fc5fda18839da7aa093a7409866462a970f4cc6268`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:33:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 13:33:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 13:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:34:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 13:34:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 13:34:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:34:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:34:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 13:34:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 01 Mar 2022 13:34:13 GMT
ENV PHP_VERSION=8.1.3
# Tue, 01 Mar 2022 13:34:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.3.tar.xz.asc
# Tue, 01 Mar 2022 13:34:14 GMT
ENV PHP_SHA256=5d65a11071b47669c17452fb336c290b67c101efb745c1dbe7525b5caf546ec6
# Tue, 01 Mar 2022 13:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 13:35:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:46:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-embed 				--enable-zts 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Mar 2022 13:46:21 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:46:21 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Mar 2022 13:46:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Mar 2022 13:46:22 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36e768b2f62ca9db79fc8204f94fabef165bdb7951c4ecdc3161e42c72b599`  
		Last Modified: Tue, 01 Mar 2022 15:09:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33e437f967c6f0d1b201253e1e22ce9112d55070778d806c5e693166688bfc7`  
		Last Modified: Tue, 01 Mar 2022 15:09:45 GMT  
		Size: 71.6 MB (71618545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9901cb4d6a8d6e06176baa29aea61892e9441218ce09d660d1bf74bbbf2821`  
		Last Modified: Tue, 01 Mar 2022 15:09:35 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5f1b9ec6fecc04f93cd95216afc66f6cf22351836fd0c926d29eeeb2034cc1`  
		Last Modified: Tue, 01 Mar 2022 15:09:35 GMT  
		Size: 12.1 MB (12069427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8da984ecde47b1de57d83422fdb8172a9115b6c0a3f4d4661c4f15307fd1443`  
		Last Modified: Tue, 01 Mar 2022 15:09:34 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6936ac54abaa69108d90ee7ae4f062423478a42d20a825100cef2724ad0908`  
		Last Modified: Tue, 01 Mar 2022 15:11:32 GMT  
		Size: 29.1 MB (29138574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887ef3410b148bd8727fbb6d46da7fcab492d197d300754dd78585df99b39e2c`  
		Last Modified: Tue, 01 Mar 2022 15:11:29 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea4dbb5efae6047c82c2ad76375bba58f7875200977bf9a71533556d470f47d`  
		Last Modified: Tue, 01 Mar 2022 15:11:29 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
