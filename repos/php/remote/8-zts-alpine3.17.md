## `php:8-zts-alpine3.17`

```console
$ docker pull php@sha256:64fccb11d0d9eb25653c1dd11766114592e3f83d7cfc8c410378e2e59c20c14d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `php:8-zts-alpine3.17` - linux; amd64

```console
$ docker pull php@sha256:09454117c6a2f0a57f22b178fb16db0f7d8430e275dd52a61cfc0120b854464f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30145961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6163eae367e0bd38d6fe792c93325bd996d30e72f3704a15df04c8bfd9017395`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:42:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 00:42:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 00:42:37 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 00:42:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 00:42:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 00:42:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:42:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:42:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 01:05:45 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 01:05:45 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 01:05:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 01:05:45 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 01:05:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 01:05:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:16:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 01:16:51 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:16:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 01:16:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 01:16:53 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2d0e53cae4fa9e99bf4244568126b8df6d69fe6ee06580fe987d0ac9bc1c51`  
		Last Modified: Thu, 15 Jun 2023 02:07:56 GMT  
		Size: 1.9 MB (1891710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0018871e86ff704c651cf77f534a17074a5da1002810199a8bcd197e0f2b7e3`  
		Last Modified: Thu, 15 Jun 2023 02:07:56 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399c2bf9de3aced3bdb63485e296ec23ab7f52a54441ccb6d70b52fd4dd30e02`  
		Last Modified: Thu, 15 Jun 2023 02:07:55 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebe2f5a71117a5b67a614fc99c517f324c023c28b18e28d937d790d5b16dd17`  
		Last Modified: Thu, 15 Jun 2023 02:10:19 GMT  
		Size: 12.0 MB (12037641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5f070c40eeadd51819a509e4a84762ff6a50ca96a3c9c2a14025adc926317c`  
		Last Modified: Thu, 15 Jun 2023 02:10:19 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95ec4e5428ca7249e089729f8de0fd446e5b3f5940f900f8903e0ac92496`  
		Last Modified: Thu, 15 Jun 2023 02:10:58 GMT  
		Size: 12.8 MB (12818456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4424750f6150c6ad3831d283c2a04cd554b5a8f07c6a87bd4ac9a7bd38bd8b30`  
		Last Modified: Thu, 15 Jun 2023 02:10:56 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59afc1d11d0018b05e279422c8ed59c9bfbca269a6b632960ef5333b067c222`  
		Last Modified: Thu, 15 Jun 2023 02:10:56 GMT  
		Size: 19.0 KB (18967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-alpine3.17` - linux; arm variant v6

```console
$ docker pull php@sha256:c1f57293bc27ed277ebd9a888f19977b80d18b5994255aab1e7ffdab5580ece4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28727794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5e4584e3aeaa44662c10c0f05414339316380e2a233865a42dad2e2c380f84`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:12:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 00:12:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 00:12:22 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 00:12:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 00:12:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 00:12:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:12:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:12:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 00:30:04 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 00:30:05 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 00:30:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 00:30:05 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 00:30:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 00:30:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:39:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 00:39:44 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:39:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 00:39:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 00:39:45 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf22d1d692138b9e57071d39851f829f232b8f3852af079a2961453ba31c5c`  
		Last Modified: Thu, 15 Jun 2023 01:18:03 GMT  
		Size: 1.9 MB (1878933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0857b1d531af3d47422625dae6d0da81a3c69a1d8124d4756481afd3f4b05485`  
		Last Modified: Thu, 15 Jun 2023 01:18:03 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ee0b1458dcd2b82cfe16e510b5edfb32836b137345c314aedd96c772c9e2fd`  
		Last Modified: Thu, 15 Jun 2023 01:18:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4822d7dc009d49f45ed6b97a52f46fd8974c41fd2afb1f3b813d8495739ae48d`  
		Last Modified: Thu, 15 Jun 2023 01:20:10 GMT  
		Size: 12.0 MB (12037631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe7680164c9256b851b2e6bab7988b70305c1c056441cda6973387a024ba7e4`  
		Last Modified: Thu, 15 Jun 2023 01:20:09 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a57f8df5111e4e44a7d7de769cc75d42bd30976d8f56eaebfdc6dcf6ea1ce5`  
		Last Modified: Thu, 15 Jun 2023 01:20:49 GMT  
		Size: 11.7 MB (11677093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b610bbd0efd8e90f5a3e6348e6d71576c8cc063cce8d38befeb8d84238ac12e`  
		Last Modified: Thu, 15 Jun 2023 01:20:47 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4116eefb7c8e6d010f6ced5a24711880876e3957d6972f691df1f113f6ac46bd`  
		Last Modified: Thu, 15 Jun 2023 01:20:47 GMT  
		Size: 18.7 KB (18749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-alpine3.17` - linux; arm variant v7

```console
$ docker pull php@sha256:126847fc146f73b8bd47512896a1ead815b707200983d2396ae29acd28ed8d93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29948689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11fd19b3ddaf2716a45f99470ece5c02c2aa5d6324a4d7aebc93936e879b86d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:56:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 29 Mar 2023 22:56:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 29 Mar 2023 22:56:33 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 29 Mar 2023 22:56:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 29 Mar 2023 22:56:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 29 Mar 2023 22:56:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 22:56:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 22:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 29 Mar 2023 22:56:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 09 Jun 2023 01:58:44 GMT
ENV PHP_VERSION=8.2.7
# Fri, 09 Jun 2023 01:58:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Fri, 09 Jun 2023 01:58:44 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Fri, 09 Jun 2023 01:58:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 01:58:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 05:50:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 05:50:25 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 14 Jun 2023 05:50:26 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 05:50:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 05:50:26 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d801477645c6152bedd176a48dd4cd43848b4628df963f29190ca396a08cda1b`  
		Last Modified: Fri, 31 Mar 2023 23:09:11 GMT  
		Size: 1.7 MB (1715928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bf14e8ce70e4d5b9dc80eefdce167d1b7c565c34eace0f6282428b4ed6ac44`  
		Last Modified: Fri, 31 Mar 2023 23:09:10 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba08b30181e8a0fd2e9555d9f184958e0cf2b0ac3ad5d11f50dc8a534fd0208`  
		Last Modified: Fri, 31 Mar 2023 23:09:10 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49b20fcd7c6711f08f73893176f32f07b7313545ddf07bf9d4535b7ea125dc`  
		Last Modified: Fri, 09 Jun 2023 03:36:49 GMT  
		Size: 12.0 MB (12037603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e55f31f183749ce2419c67dae145f3348e5125da7e7eec796e6342b02224f42`  
		Last Modified: Fri, 09 Jun 2023 03:36:48 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30af7515ac15f73f42f053940180ab0c6a1779d83ffee22c84e2631fee87d8f`  
		Last Modified: Wed, 14 Jun 2023 06:42:11 GMT  
		Size: 13.3 MB (13303288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4369b067b2e0fd0589cf3b11baf863d2a180e79a9fe5340833745618b492752c`  
		Last Modified: Wed, 14 Jun 2023 06:42:09 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941c1ac30157a646a67fbf1345026bc0911773d6cd8e1c4232e112faa2659a14`  
		Last Modified: Wed, 14 Jun 2023 06:42:09 GMT  
		Size: 18.9 KB (18881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull php@sha256:0366210884bd739a297962c5901a4b37e3f286c3ab43d8e3918f0db7caad25ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30037882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817a6411fb506db67d4171b43efa6737f7f651625016f017e6672a41563bddc9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:17:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 03:17:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 03:17:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 03:17:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 03:17:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 03:17:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 03:17:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 03:17:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 03:41:29 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 03:41:29 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 03:41:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 03:41:29 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 03:41:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 03:41:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 03:52:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 03:52:54 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 15 Jun 2023 03:52:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 03:52:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 03:52:55 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6675870db3e226ae39aec542092b3563b0352c3123a698108eeb8b98d51c47e`  
		Last Modified: Thu, 15 Jun 2023 04:40:00 GMT  
		Size: 1.9 MB (1890568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786e1ff66e74a63d03dac9ca2ad422f0d24773d8a7fbafb18f4a5c5f376516d0`  
		Last Modified: Thu, 15 Jun 2023 04:40:00 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fbb55376f1fbddb9b8d7aff626e903b3d86a702ae59267b0dbc350e6d8f066`  
		Last Modified: Thu, 15 Jun 2023 04:40:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46482da7080de20f8e03f72eae2739d251a8ebca82da30c00753ea334e76ded6`  
		Last Modified: Thu, 15 Jun 2023 04:42:10 GMT  
		Size: 12.0 MB (12037632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30be84ebdbc7d80a7e6359bcd3c6506595133e711ec3f4f06f4a29db0531c953`  
		Last Modified: Thu, 15 Jun 2023 04:42:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a46b0e42c7fd668664ad475b2fcc4411bd39c85aca09d911ade316a8d9e36`  
		Last Modified: Thu, 15 Jun 2023 04:42:46 GMT  
		Size: 12.8 MB (12825302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439031444b468b8006b38226e239121bd707217c4662a5cf93b6e7de1dc1ef7`  
		Last Modified: Thu, 15 Jun 2023 04:42:46 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72f45541e1dcb924030e2e3288aadc136446e1eb357d429d700985030148c7b`  
		Last Modified: Thu, 15 Jun 2023 04:42:46 GMT  
		Size: 18.8 KB (18768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-alpine3.17` - linux; 386

```console
$ docker pull php@sha256:8329a07f3a60f0dcd8440c192f3f580cf9a2210877c9361570d564f8b8e5d6eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33450650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49fde2f7979dc45b730556e1f22d2992c6436bc72fce861a8356b2fc15455e3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:02:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 29 Mar 2023 20:02:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 29 Mar 2023 20:02:38 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 29 Mar 2023 20:02:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 29 Mar 2023 20:02:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 29 Mar 2023 20:02:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 20:02:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 20:02:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 29 Mar 2023 20:02:39 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 09 Jun 2023 02:02:36 GMT
ENV PHP_VERSION=8.2.7
# Fri, 09 Jun 2023 02:02:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Fri, 09 Jun 2023 02:02:37 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Fri, 09 Jun 2023 02:02:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 02:02:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 03:18:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 03:18:20 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 14 Jun 2023 03:18:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 03:18:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 03:18:21 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7929931a828d2015dd9e95a14bd27c73e8ed62100cf82854210175cc954be7`  
		Last Modified: Wed, 29 Mar 2023 21:49:02 GMT  
		Size: 2.0 MB (1992200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026beb5ca186e3c7d06eeb9c4ef9f6f17d8413c0ea078b6b51778c9f64557608`  
		Last Modified: Wed, 29 Mar 2023 21:49:02 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2223ea2b0fd26911a7879b6d53134b714418def170fb74dd549259cdd83ad5f`  
		Last Modified: Wed, 29 Mar 2023 21:49:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcaf7eeac1fa02cd86089707be867a32bdbcd6296640b416e1a4ebfaf55ca6b`  
		Last Modified: Fri, 09 Jun 2023 05:20:09 GMT  
		Size: 12.0 MB (12037616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278368f7b0b9e892564ab7c8007c33cadc2ea44922ebf0509394d8b797d28b48`  
		Last Modified: Fri, 09 Jun 2023 05:20:08 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e42f14757ac89d6a08abe217db55a579ae3a149fb02c780639aed0c36740b1`  
		Last Modified: Wed, 14 Jun 2023 05:13:30 GMT  
		Size: 16.0 MB (15985006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275cc3f4bdb1bc0241606636a5112515a77f7122dc1094de0106c4523e3d0e4b`  
		Last Modified: Wed, 14 Jun 2023 05:13:26 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39a5b2eabf6f6cf93b0532cc429b6b8fee72cfc6416d488c3766ca90bf7a6e4`  
		Last Modified: Wed, 14 Jun 2023 05:13:26 GMT  
		Size: 19.1 KB (19093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-alpine3.17` - linux; ppc64le

```console
$ docker pull php@sha256:5e7f4334429b1d4264664d192ae001b8349868e53465f7c0d9dbcfe04495fb82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30632929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba368b8caea107f3e1632c06215d7e5ac4d311c0eb7c0b0640fdc2460607ecb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:33:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 02:33:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 02:33:05 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 02:33:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 02:33:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 02:33:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 02:33:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 02:33:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 02:58:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 02:58:33 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 02:58:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 02:58:34 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 02:58:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 02:58:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 03:10:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 03:10:51 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 15 Jun 2023 03:10:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 03:10:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 03:10:53 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6bb03e2143381aabfd7cdeef4b333805d412bc6810eb93488896e87e703d7d`  
		Last Modified: Thu, 15 Jun 2023 04:12:29 GMT  
		Size: 2.0 MB (1975934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5726f645ddc4327478b2571ebcc8d1ba8ebe13f0f42be5d680aade1a6c89919`  
		Last Modified: Thu, 15 Jun 2023 04:12:29 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87cc33314d1d7b0c01106a640d857911c907f2cd6a8c45cbcc9a60b3b5d2b53`  
		Last Modified: Thu, 15 Jun 2023 04:12:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512899ebae6c45eaafac3aa91a7c5ab607b721f55439b3b24e8240dcb1c3eb36`  
		Last Modified: Thu, 15 Jun 2023 04:15:03 GMT  
		Size: 12.0 MB (12037623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a87463437e773221285a5ca9fd839daea02d7c9b6a181d759b25757a2e9ac8`  
		Last Modified: Thu, 15 Jun 2023 04:15:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5236e4e51c9d7aba9d80a5d371594b15eaeec878f768f7e0392696fe99bee84`  
		Last Modified: Thu, 15 Jun 2023 04:15:52 GMT  
		Size: 13.2 MB (13206222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3e4ea101b85984881a9a970e8265efc9e960deafd211225ea4c38b29612179`  
		Last Modified: Thu, 15 Jun 2023 04:15:48 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6589f4cfc2fee1fff0877e466218396a7e97a9c7aa170643eeb632e33d00ed`  
		Last Modified: Thu, 15 Jun 2023 04:15:48 GMT  
		Size: 18.8 KB (18773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-zts-alpine3.17` - linux; s390x

```console
$ docker pull php@sha256:63cdac998bcac48cf46ff4f9e50fa889756d83b98af2922b1877fc1f7e4c6da6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31781208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f260efcc62e50f0f3f9b57f88e5368d8de34b57c969d67bc6aba0a72c1be993`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:02:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 29 Mar 2023 19:03:01 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 29 Mar 2023 19:03:01 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 29 Mar 2023 19:03:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 29 Mar 2023 19:03:02 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 09 Jun 2023 00:28:01 GMT
ENV PHP_VERSION=8.2.7
# Fri, 09 Jun 2023 00:28:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Fri, 09 Jun 2023 00:28:01 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Fri, 09 Jun 2023 00:28:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 00:28:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:17:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-embed 				--enable-zts 		--disable-zend-signals 		--enable-zend-max-execution-timers 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 01:17:18 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:17:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 01:17:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 01:17:20 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6521aff379460e3b23538794f9f58987d8c205d856adb8b1906678f475549d`  
		Last Modified: Wed, 29 Mar 2023 19:53:09 GMT  
		Size: 1.9 MB (1926778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ccc0e3e0585970bf7f018f1b481c5bda3c11ade58ae10a67fac7eb146920ec`  
		Last Modified: Wed, 29 Mar 2023 19:53:09 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffa02384e22bdeff50d42395895a9ce2b39494195bc42784c30061aa4ea5384`  
		Last Modified: Wed, 29 Mar 2023 19:53:09 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40560346663fb8e8425211dbd8462e73390248cd550fa60f8cc9796c6853fa4d`  
		Last Modified: Fri, 09 Jun 2023 01:37:46 GMT  
		Size: 12.0 MB (12037619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0d7f9fbe4da5f4f832fd09c5870bb3a8dcea27ad6c8d1aed0d6365482381c`  
		Last Modified: Fri, 09 Jun 2023 01:37:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28619b34aafce53e98b1cbd5e825541bf39117c369c3af2946da1260cc61732c`  
		Last Modified: Thu, 15 Jun 2023 03:56:11 GMT  
		Size: 14.6 MB (14618255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb343be59621fe0cade90c4c709ab54fc91cea2c4b7c8acf5e3ee7d68a5e57c4`  
		Last Modified: Thu, 15 Jun 2023 03:56:08 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9df5607534d42876f0e0f5d34ae242e3ddce28574ef4e38fdba02c2d1cc9dc`  
		Last Modified: Thu, 15 Jun 2023 03:56:09 GMT  
		Size: 18.9 KB (18895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
