## `php:7-buster`

```console
$ docker pull php@sha256:2ab76fa5b5751e4f7efed5a0431ced868ad6d017828863678597288cf07174bd
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

### `php:7-buster` - linux; amd64

```console
$ docker pull php@sha256:68b6ba0799a960692e6f035ef327371450291d943244a66827c484df175c1c3a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146687008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8071336a5840802fe093057853e54f8a243e28ade23d7bcd9cea245465df83`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:39:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 12:39:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 12:39:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:39:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 12:39:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:39:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:39:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:39:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 14:34:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 22:04:46 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 22:04:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 22:04:46 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 22:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 22:05:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:09:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:09:36 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:09:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:09:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:09:37 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13522578ad9c68f9a771d9dfc2a14315b97c7ee6690853b02cd9c261046d8b7`  
		Last Modified: Thu, 02 Dec 2021 15:31:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027e794f2380b6fb5275c0b6c78e9cbcc29821b043c51ad81ca54eb46a801a7`  
		Last Modified: Thu, 02 Dec 2021 15:32:07 GMT  
		Size: 76.7 MB (76681131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003069fe633e007e207bfc0b2084e0d3b19cabd7d7a308367946cd858fabcc6`  
		Last Modified: Thu, 02 Dec 2021 15:31:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac995548def85224446c5a84091ab6692760b68a403e6d9bb4c058fd1f7adc8b`  
		Last Modified: Thu, 16 Dec 2021 23:29:21 GMT  
		Size: 10.7 MB (10740733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd055bd152c367601b451f4c9315a885704bc272e0c7e0a09db13fe4a9c119d`  
		Last Modified: Thu, 16 Dec 2021 23:29:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be56c46590554a20943ff7ea4d830462738cdead69127c5c383c608ef9f9b99`  
		Last Modified: Thu, 16 Dec 2021 23:29:25 GMT  
		Size: 32.1 MB (32107873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996fb737fa199e9160f50949687f0f8ee94fa86a5ae611522a7300a7fd9a2869`  
		Last Modified: Thu, 16 Dec 2021 23:29:20 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49aed71785151b452cbe6c83835ab699f513a7e712daf72f17d4a71ba887cac4`  
		Last Modified: Thu, 16 Dec 2021 23:29:19 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; arm variant v5

```console
$ docker pull php@sha256:1ab66aef6771d59849c0e4e458380c69f779c9ff7ce4a4abdb018aa30540e740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124881245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d99837d3e31a55f45bec332370dfa2f5c91011cd4971311f9d8455dda4dfef`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 04:24:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 04:24:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 04:24:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 04:24:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 04:24:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 04:24:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 04:25:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 04:25:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 05:52:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 21 Dec 2021 05:52:37 GMT
ENV PHP_VERSION=7.4.27
# Tue, 21 Dec 2021 05:52:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Tue, 21 Dec 2021 05:52:38 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Tue, 21 Dec 2021 05:53:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 05:53:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 05:57:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 05:57:32 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 21 Dec 2021 05:57:34 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 05:57:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 05:57:35 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9b9eb6bf9c1835420d93b2eaaf3e145fed569844213261b1856d86a95215e8`  
		Last Modified: Tue, 21 Dec 2021 07:11:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb71c5036287658e4188420d6e1d87c59ed2230b1ee75015ff1f8ffb2574a773`  
		Last Modified: Tue, 21 Dec 2021 07:12:04 GMT  
		Size: 58.8 MB (58820825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f97f23af12b0b8b39475548019d21ed3a481c0c630c8c72c95860bcaf5bcfe`  
		Last Modified: Tue, 21 Dec 2021 07:11:23 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb5545df12ad34506ff5e53ae9b4c4124a591d42261f25a39b45e665dcca71f`  
		Last Modified: Tue, 21 Dec 2021 07:22:48 GMT  
		Size: 10.7 MB (10738886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f817b4cca5cf23661d57ccac510b8cfaae4c41cb32e88949401d241a8f971b`  
		Last Modified: Tue, 21 Dec 2021 07:22:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158e4fef9e188c944b87d210cd2b00ec9f3870f6e44b8b5cd2c71d126304f09d`  
		Last Modified: Tue, 21 Dec 2021 07:23:04 GMT  
		Size: 30.4 MB (30431733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7223bb74059befa01c3e7a96e2d2d3b6da4e4be0da2fb3ef216f5e2d99a81e9`  
		Last Modified: Tue, 21 Dec 2021 07:22:45 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f7795ba068004c9ce92fad7c85ca2fd1cf29ea3ea5f35ca3b6644dde2dc5d2`  
		Last Modified: Tue, 21 Dec 2021 07:22:45 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:7ca1df6760ad7e8dfff41bdc840dacaada72e3790f64f9d22a386c5ee84502bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122216304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:572b0bc31b01a26f6c455dfd7fb69459660383fcebddf5a7c665950561a96ee7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:21 GMT
ADD file:7b30d743b30e84b21888f23cb7f266caba09db98b7a4c8800abebcf03d28c01d in / 
# Thu, 02 Dec 2021 09:06:22 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 23:58:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 23:58:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 23:59:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 23:59:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 23:59:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 23:59:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 23:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 23:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 01:21:12 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 21:50:14 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 21:50:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 21:50:15 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 21:50:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 21:50:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:54:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 21:54:44 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:54:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 21:54:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 21:54:47 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:2aa85085c98821a25a3058f7fc2c6427064f2228ea8eac904e9e7db4dbdaa01a`  
		Last Modified: Thu, 02 Dec 2021 09:22:26 GMT  
		Size: 22.8 MB (22754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f7b26d2bc1ea192fde28dc60f9092d2eadaf1e04e05945429f62d96552e0e0`  
		Last Modified: Fri, 03 Dec 2021 02:46:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f9859f8a5d4053d7bd3ae9a71a62280361871b77958dab4197d6fd56498d71`  
		Last Modified: Fri, 03 Dec 2021 02:47:00 GMT  
		Size: 59.5 MB (59515834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c958a15ac5e569b340965c772589a7dbfe8eb545048b2bf874e7c24d99639`  
		Last Modified: Fri, 03 Dec 2021 02:46:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385821decbe1f1f552b16cdc0cefc09a5ae0e2fc357f06a28c037f8cd7986943`  
		Last Modified: Thu, 16 Dec 2021 23:05:54 GMT  
		Size: 10.7 MB (10738876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160ea819d4031742447ecfe30888f28de782a0bd12ccd9a58b985755fe845b9`  
		Last Modified: Thu, 16 Dec 2021 23:05:52 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2ad16856abc6c2cfc39c7e7ddb951c4f597bd95243ac3f1873c71f0e00a182`  
		Last Modified: Thu, 16 Dec 2021 23:06:09 GMT  
		Size: 29.2 MB (29203689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba402d6d9e815d3dc00e5dcd219f42c59079c4b203ac346be471470730a864`  
		Last Modified: Thu, 16 Dec 2021 23:05:52 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0d44200cf293e903dcc4d836befe1a244ee5d676953b7b86aa80fdb98fe79`  
		Last Modified: Thu, 16 Dec 2021 23:05:52 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:b24f6608fb26494f6825892dd28d4fed5400d10ca48411e37613a696f4511564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138390212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1601d74710f02cb06c649128158ffeec9d6f295ca9cbf625bd134dd517d81aec`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:52:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 03:52:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 03:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:52:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 03:52:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 03:52:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:52:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:52:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 04:43:46 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 21 Dec 2021 04:43:47 GMT
ENV PHP_VERSION=7.4.27
# Tue, 21 Dec 2021 04:43:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Tue, 21 Dec 2021 04:43:49 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Tue, 21 Dec 2021 04:44:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 04:44:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:45:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 04:45:55 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:45:55 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 04:45:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 04:45:57 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399cd382f74b9333921ab9450361ddfc29e07826cfb4906582618a1665ba6ba0`  
		Last Modified: Tue, 21 Dec 2021 05:25:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978dcfbedcedd2e259c7988f1c18e962e16d5ca4aaf0371c8d53e57eeb7411b6`  
		Last Modified: Tue, 21 Dec 2021 05:25:19 GMT  
		Size: 70.4 MB (70359361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f787b5a5e5d17b19845cd143a04fc6d2bc76cc9432e2ef888079bcf12142b6`  
		Last Modified: Tue, 21 Dec 2021 05:25:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6c0de8f32f3a1214cb96c2ad38969b7e27f11ea13f86c28227b5137d39af36`  
		Last Modified: Tue, 21 Dec 2021 05:32:42 GMT  
		Size: 10.5 MB (10527898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1b126544ced7a9ff4d1c61db1529bd44281e9784000fc0172907542ed6775f`  
		Last Modified: Tue, 21 Dec 2021 05:32:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41268c8aa201239f750d1194cc2bd9a7229b3ffe964b85ef700222fe51410298`  
		Last Modified: Tue, 21 Dec 2021 05:32:51 GMT  
		Size: 31.6 MB (31576307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1825f6bf8fbb5cf970e081df7a9810207dd65622850cf3a204c06606940a40cb`  
		Last Modified: Tue, 21 Dec 2021 05:32:41 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f04b400bf98c61c845099652265901a4d71e6963f65209cac358b1efe8aa49`  
		Last Modified: Tue, 21 Dec 2021 05:32:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; 386

```console
$ docker pull php@sha256:9d7fc761c1237c8e65da5de11b95cae15b813133804564350894829392f4622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.5 MB (152528999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:498148ea56801c7eae0f6697614afd9f4a946134527f96b38bf162b9fe4c59dd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:00:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 16:00:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 16:01:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:01:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 16:01:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 16:01:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 16:01:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 16:01:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 17:53:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 22:04:52 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 22:04:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 22:04:52 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 22:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 22:05:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:09:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:09:50 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:09:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:09:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:09:51 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3bec8390a3fb9cacde110dff928f03c6bfbf4c67380782be7bc2ec468bad44`  
		Last Modified: Thu, 02 Dec 2021 19:05:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374e03f2cbaf2599705aba5989e4c2f0610646764f4b510df4d65fd56cdb13bb`  
		Last Modified: Thu, 02 Dec 2021 19:06:06 GMT  
		Size: 81.2 MB (81229810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8020b07a62641f451efc11a0c44d8280cb3c444a9a40c5d31cd6d56577eed4e4`  
		Last Modified: Thu, 02 Dec 2021 19:05:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30507bee6f40c56b413311eb9e1a1ddb274749f72a9ee2b703838d92422f2fe8`  
		Last Modified: Thu, 16 Dec 2021 23:40:12 GMT  
		Size: 10.7 MB (10739948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97b65cfb15b8b45112c491fb8ec0f1ac57109dfbaa6aab7f1dd024a6b7acf08`  
		Last Modified: Thu, 16 Dec 2021 23:40:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb78d08ad29493a8ff1c0615ea43e570b860e08c0542e0460e24990716c47cde`  
		Last Modified: Thu, 16 Dec 2021 23:40:20 GMT  
		Size: 32.8 MB (32751139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc12b1cb5745095ace2bde8867464cf32be864e3dd3495b2e48b660f93d015`  
		Last Modified: Thu, 16 Dec 2021 23:40:11 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff5d3e91d11cf4882fb8a8e2091f8df30d1a6b4e83be5f01a3a070334f7027f`  
		Last Modified: Thu, 16 Dec 2021 23:40:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; mips64le

```console
$ docker pull php@sha256:60b2508ae5a6e91c5af19119b8dfe7196483897be78ab281d472769cad9a5508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129210753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cafddabeec35c7e1ee40bfcbfc6b00f4a9343533331b6a9495a0024d6ce616e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 02 Dec 2021 03:10:02 GMT
ADD file:8c95ae1f84ca959b3714f55dc11bf2655dbe383f4aa06564e3f0f5386a8602b9 in / 
# Thu, 02 Dec 2021 03:10:03 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 13:27:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 13:27:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 13:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 13:28:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 13:28:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 13:28:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 13:28:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 13:28:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 16:42:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 21:47:05 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 21:47:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 21:47:05 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 21:47:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 21:47:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:55:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 21:55:30 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:55:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 21:55:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 21:55:32 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:d19557eca39adc90542589f749291953b676e4201aa77d093caf4a98b87fb79b`  
		Last Modified: Thu, 02 Dec 2021 03:19:22 GMT  
		Size: 25.8 MB (25820168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1eacf510c82b7260a2ce08fb07e0d0ff74d07980524153b40ae9fda2cd51379`  
		Last Modified: Fri, 03 Dec 2021 18:45:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaf8e0b9c3688aed43bab352fca9dd5d922ef1c0f4b6f7461318525d9ad424a`  
		Last Modified: Fri, 03 Dec 2021 18:46:47 GMT  
		Size: 61.4 MB (61403775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acc5ff4ea4c6d24caac8bd856a6c02c3233b7db449241eb9898c7d9f85e58c9`  
		Last Modified: Fri, 03 Dec 2021 18:45:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee1f9e86030eaf1ce5b2a1b0885b2e0fc23139c7915b1922eb3aa5b251c12c5`  
		Last Modified: Thu, 16 Dec 2021 22:31:19 GMT  
		Size: 10.7 MB (10738320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4897f6492c62ee74b968a3e19d1c149b048b907fa4a3962349aaab2e8ea31fb1`  
		Last Modified: Thu, 16 Dec 2021 22:31:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d7eb4c150ed14f2d10958ab97f710f0b4826221933aed9df122c39e8180719`  
		Last Modified: Thu, 16 Dec 2021 22:31:38 GMT  
		Size: 31.2 MB (31244996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62943efce2a3812c2b31e4ba298f94e52847582e12721e6db7c27a93ba674c20`  
		Last Modified: Thu, 16 Dec 2021 22:31:16 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dc045dc00d7bec38a39d92f1fca7a09631a3ea1b4ba9a62c65b035c8cd7445`  
		Last Modified: Thu, 16 Dec 2021 22:31:16 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; ppc64le

```console
$ docker pull php@sha256:85a69fa4fe5b9719b5f87dbda1f38c660ce58d1ebf90000f9f5f36c6b2d41bd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.7 MB (157680303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbd96c7b131fc7d32d1dfaa5c55dd2227be83b032fd20450288e7c1224f5e88`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:12 GMT
ADD file:b9b5697bc2dd3ded7a158d973abc939cc5d197f1f0d9ff1fa8b3db3b7906de7a in / 
# Thu, 02 Dec 2021 07:22:18 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:53:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:53:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:54:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:55:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 01:55:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:55:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:55:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 03:21:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 21:57:03 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 21:57:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 21:57:07 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 21:58:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 21:58:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:02:43 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:02:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:02:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:02:54 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:da5263f5d65ecaf2dcd9400908302b4c477c13afa707110e4d85b4b946e9a3ae`  
		Last Modified: Thu, 02 Dec 2021 07:32:41 GMT  
		Size: 30.6 MB (30562306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8f6c7bf36c9a359b779def1339d11fe1d9c1422d6a518b6431c941f70bb683`  
		Last Modified: Fri, 03 Dec 2021 04:38:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3507a81e5d8123871a651605ea2edc67d3b3faaa82eb682639d539c385e14e0a`  
		Last Modified: Fri, 03 Dec 2021 04:39:34 GMT  
		Size: 82.3 MB (82291748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ec8b19b49c5228741833ff588ab20a7146158440b5a7ff46d9b99b10a861ae`  
		Last Modified: Fri, 03 Dec 2021 04:38:58 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74bf300353cbb6a2225a049a7b919ba9d81029abc81acf599a0d91c07fc55b6`  
		Last Modified: Thu, 16 Dec 2021 23:11:31 GMT  
		Size: 10.7 MB (10740299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac00b9d57c603edeea5b1cb2564c969d9a8230e2a466b4129785a7985b6af4da`  
		Last Modified: Thu, 16 Dec 2021 23:11:29 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99faf1da326b319ff06c3f31f0539bbba5385b0085da0f581eaa5770bf17391`  
		Last Modified: Thu, 16 Dec 2021 23:11:36 GMT  
		Size: 34.1 MB (34082406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed06b3009354d379fb3a18a589a2acb01eb4d9b0610a5ce481d7dfd4e187953`  
		Last Modified: Thu, 16 Dec 2021 23:11:29 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c234b5039eb4249cd5aef785c47db7085bd9a6f655898249c89b6536a4df64a`  
		Last Modified: Thu, 16 Dec 2021 23:11:29 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-buster` - linux; s390x

```console
$ docker pull php@sha256:38702167ccdfc09a623be01163dd7ccc3b05f930e1c6240d4beb5c2796173f6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132215228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3268c1e0867386905d5cff54ad1cb5a98e333240464c83784f60fc754db07c63`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:58:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 05:58:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 05:58:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:58:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 05:58:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 05:58:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 05:58:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 05:58:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 06:35:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 21 Dec 2021 06:35:45 GMT
ENV PHP_VERSION=7.4.27
# Tue, 21 Dec 2021 06:35:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Tue, 21 Dec 2021 06:35:45 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Tue, 21 Dec 2021 06:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 06:36:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:37:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 06:37:23 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:37:24 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 06:37:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 06:37:24 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf65a5687afc4442eac857ae3da34458abafddf748d5a3d9376ee70037c14a7`  
		Last Modified: Tue, 21 Dec 2021 07:10:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffc077076230c4b93f115982fd907a1402d52434473293959fa276ef6e4259`  
		Last Modified: Tue, 21 Dec 2021 07:10:16 GMT  
		Size: 64.7 MB (64712203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cf03affd681931ff0470cc97f0f64f0a59940bcc65cbab96c7cad075c21b65`  
		Last Modified: Tue, 21 Dec 2021 07:10:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad22453614ec38ddc078d019c5a58459fe7c1dba838f014e22603ea879b24f5`  
		Last Modified: Tue, 21 Dec 2021 07:15:23 GMT  
		Size: 10.7 MB (10739079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acaaaf7515e7e572a49ac8888fdab6deb148f46e89059ea3f495092d95b4c69`  
		Last Modified: Tue, 21 Dec 2021 07:15:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dba7112036b5f0f52b8a54e89b1c687135ff859ee84678826e3752e796ecc1`  
		Last Modified: Tue, 21 Dec 2021 07:15:27 GMT  
		Size: 31.0 MB (30991352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569f3f0ea3dcb9c208e6b752ddd6b428bd014ff01f2d16f1075e48bff865a463`  
		Last Modified: Tue, 21 Dec 2021 07:15:23 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dc88aed86d135054e221c387dcfb799e25587ec09e6634d998e75a8114b43c`  
		Last Modified: Tue, 21 Dec 2021 07:15:23 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
