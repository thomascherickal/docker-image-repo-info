## `php:7-zts-alpine`

```console
$ docker pull php@sha256:41fad42488f3f37f56368828170896c94f50a24c9edbd6ce32226fb544a2cf14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `php:7-zts-alpine` - linux; amd64

```console
$ docker pull php@sha256:444c3ddbeb302b89dfc6542cd80442fb118cc5bbbc08e0f537f8c12ce3b4d661
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25695284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e426dc3c6df43ff6a9e844541cf7998b3275440bf877dd22a4f3a451edbbb52`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:32:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 23:32:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 23:32:48 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 23:32:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 23:32:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 23:43:26 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 16 Jun 2021 23:43:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 23:43:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 23:43:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 23:43:27 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 16 Jun 2021 23:43:28 GMT
ENV PHP_VERSION=7.4.20
# Wed, 16 Jun 2021 23:43:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 16 Jun 2021 23:43:28 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Wed, 16 Jun 2021 23:43:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 23:43:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 25 Jun 2021 21:03:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 25 Jun 2021 21:03:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 25 Jun 2021 21:03:28 GMT
RUN docker-php-ext-enable sodium
# Fri, 25 Jun 2021 21:03:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 25 Jun 2021 21:03:29 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcf566573f3f708d78b43786614663e55d9a9d02621f3dab2127292efbbacab`  
		Last Modified: Fri, 25 Jun 2021 21:36:24 GMT  
		Size: 1.7 MB (1707289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ff9828d9544109bb07a2fa8308b1ed77b75738fa50300d61284755c126426a`  
		Last Modified: Fri, 25 Jun 2021 21:36:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165b10189b0ff16bb4ac114562bc55a25c753c9fc11999774fc42e9979feef99`  
		Last Modified: Fri, 25 Jun 2021 21:36:23 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0439375a735f62e2a1c10ab162f69538be648d976bdc214fdac2940aba2abebf`  
		Last Modified: Fri, 25 Jun 2021 21:40:26 GMT  
		Size: 10.4 MB (10365310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c07ff1a6efc4b401de9f668255fe4957b6b8a9b9cc5976a56a5af7235b42b4`  
		Last Modified: Fri, 25 Jun 2021 21:40:25 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2841f57cd8063e0d174fc27e5e630fc875842a845a9919fe0a315c22d7f95ea4`  
		Last Modified: Fri, 25 Jun 2021 21:40:27 GMT  
		Size: 10.8 MB (10789140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ac04b45bd891e49e29900f3d462aca94c6b443e8c9ac4659eadaa6884e234`  
		Last Modified: Fri, 25 Jun 2021 21:40:25 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf6b672f6a50578899a03d32028580a99d25776f1b2bbb26f95832f8dda77cf`  
		Last Modified: Fri, 25 Jun 2021 21:40:25 GMT  
		Size: 17.8 KB (17779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-alpine` - linux; arm variant v6

```console
$ docker pull php@sha256:7bd789f3c2237df6d577facebf14424b674c2b3b5587b73928e7699c66bb463b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25253341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9441daba37da92148eee49213dbc5e478aa0a58ac20184f11f8916e88056cf96`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:46:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 11:46:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 11:46:28 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 11:46:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 11:46:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 12:59:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 16 Jun 2021 12:59:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 12:59:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 12:59:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 12:59:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 16 Jun 2021 12:59:55 GMT
ENV PHP_VERSION=7.4.20
# Wed, 16 Jun 2021 12:59:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 16 Jun 2021 12:59:56 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Wed, 16 Jun 2021 13:00:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 13:00:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:07:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Jun 2021 13:07:35 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:07:36 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Jun 2021 13:07:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Jun 2021 13:07:36 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e113482d370ef8d7b85d30f26b1f72d1cd6e8c7ef16619d81f1364d7f5f97ec`  
		Last Modified: Wed, 16 Jun 2021 14:11:08 GMT  
		Size: 1.7 MB (1696009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5d12efcb9deb440e177cd74008605e0885ee38e5a282e913d4fb01610f91b8`  
		Last Modified: Wed, 16 Jun 2021 14:11:06 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde1e767b72e3d24122483f9530db0acdec168e2f3e9fc54bf590de1b887c13c`  
		Last Modified: Wed, 16 Jun 2021 14:11:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee65db8a09f20a5572b6e38e089edc7e15197ba545899cc3892e35104733266`  
		Last Modified: Wed, 16 Jun 2021 14:18:04 GMT  
		Size: 10.4 MB (10365077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8c73fa39b141287cb7861d049caf0ca775e069c509201c9938e7d8f4bf4d90`  
		Last Modified: Wed, 16 Jun 2021 14:18:02 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56c0bca250bf497acacf0245c2d655943834d371a1d1415df51b3f37c54acdb`  
		Last Modified: Wed, 16 Jun 2021 14:18:06 GMT  
		Size: 10.5 MB (10548248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915a202b77e73696f5606327934aee4daf1be796cf6a7cf998f96a553161e57a`  
		Last Modified: Wed, 16 Jun 2021 14:18:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76e36ef24724575966c4ddcf1207166ba40b35b8dcb8fbf2ee47e6965d4ee71`  
		Last Modified: Wed, 16 Jun 2021 14:18:02 GMT  
		Size: 17.6 KB (17583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-alpine` - linux; arm variant v7

```console
$ docker pull php@sha256:12f19aa30b1ef8b184ca7b38681e08dafa042adb7f330e70c1dcf7ef70721990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23889523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4ddc909d5e59546615c142e362005555d24346061037e3786fa2538b0ef6ec`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Wed, 23 Jun 2021 08:42:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Jun 2021 08:42:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Jun 2021 08:42:55 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Jun 2021 08:42:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:42:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 10:08:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 23 Jun 2021 10:08:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 10:08:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 10:08:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 10:08:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 10:08:31 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 10:08:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 10:08:32 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Wed, 23 Jun 2021 10:08:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 23 Jun 2021 10:08:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:51:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 25 Jun 2021 20:51:43 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:51:45 GMT
RUN docker-php-ext-enable sodium
# Fri, 25 Jun 2021 20:51:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 25 Jun 2021 20:51:46 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1185f00838acc4bd6c4bfdbfdd1b3b8b68fc8500c1d8393fdcc5bd8846c452da`  
		Last Modified: Fri, 25 Jun 2021 21:25:06 GMT  
		Size: 1.6 MB (1564529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5362957231a188851bc9f0b7a86718fd0561376062ac2198e3d325660d73168`  
		Last Modified: Fri, 25 Jun 2021 21:25:05 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b284c21ad15282e61562b8098064c462bfe0395c2e3de85a1b7f5fa6394e9474`  
		Last Modified: Fri, 25 Jun 2021 21:25:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9790f1e9bdb96533b614fee3462a3421be154caf9d274861353569b90800d34f`  
		Last Modified: Fri, 25 Jun 2021 21:32:10 GMT  
		Size: 10.4 MB (10365321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f6c5dd228b19b80e98a2138d138945c6962940c0eb3f095d97e89ceb6fce6f`  
		Last Modified: Fri, 25 Jun 2021 21:32:08 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec952c0945979bf7d764d4e8a998c1b577b6f57a06a11ca1fd2c0070622c1c0f`  
		Last Modified: Fri, 25 Jun 2021 21:32:15 GMT  
		Size: 9.5 MB (9509676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a1f31e126ede8a9876e71a0ee4a6031c5ef28e9be36e08fc098dab06ec3ad3`  
		Last Modified: Fri, 25 Jun 2021 21:32:08 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ef82a8c27b342223bc92c3e209d6b0d0a86ac7a2b8e6a7a04fdc46b3966bdd`  
		Last Modified: Fri, 25 Jun 2021 21:32:08 GMT  
		Size: 17.8 KB (17790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-alpine` - linux; arm64 variant v8

```console
$ docker pull php@sha256:9939e950ed56d154ca0283aab74811e247917a3a01471e17aadea4ef77d4aa5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25494322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c155586fa8a24e6e1a6277e5e4e815da5394047f4e04f5a2df28d4c5f068b42a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 22:42:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 22:42:41 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 22:42:42 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 22:42:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 22:42:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 22:53:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 16 Jun 2021 22:53:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 22:53:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 22:53:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 22:53:51 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 16 Jun 2021 22:53:51 GMT
ENV PHP_VERSION=7.4.20
# Wed, 16 Jun 2021 22:53:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 16 Jun 2021 22:53:51 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Wed, 16 Jun 2021 22:53:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 22:53:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:24:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 25 Jun 2021 20:24:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:24:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 25 Jun 2021 20:24:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 25 Jun 2021 20:24:41 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dbb31d082d4e4f90933b28b4719802e03a2261dafc489b60e4c94dd8f4e56a`  
		Last Modified: Fri, 25 Jun 2021 20:47:47 GMT  
		Size: 1.7 MB (1709425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681ea156e05a3343d484d4b75ca6196085b59763b04185e7a76b8c4a5b355568`  
		Last Modified: Fri, 25 Jun 2021 20:47:47 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e1c9b66e33460d7ebc60517e350c7107ee8977e3f6b05d2be0a44b4758d1c6`  
		Last Modified: Fri, 25 Jun 2021 20:47:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcf4f2b20675587b254cbd9bef4b4ffbce4fbb53b595a9dc6b233c6fb9c2e70`  
		Last Modified: Fri, 25 Jun 2021 20:52:54 GMT  
		Size: 10.4 MB (10365311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8f7cd52255dca1e02be0ffe369d6b71d07028aacf570c91d52ef1e78f8e2d`  
		Last Modified: Fri, 25 Jun 2021 20:52:53 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc916800fb090fdb080bcc96b5c08c6cd171e3d2b2c12cd7d46dde9cc5fb6dab`  
		Last Modified: Fri, 25 Jun 2021 20:52:55 GMT  
		Size: 10.7 MB (10687892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fe30f3ee3a4be5824b7807e2d0784fd3ad13d5e9459fb66b2a257356feeb20`  
		Last Modified: Fri, 25 Jun 2021 20:52:53 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea765b9aa072fee8ce022963a7639aa57809a146e6d12c0fb2a247962a954ba9`  
		Last Modified: Fri, 25 Jun 2021 20:52:53 GMT  
		Size: 17.8 KB (17782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-alpine` - linux; 386

```console
$ docker pull php@sha256:8705b842ffb8e1cf97b98ebd628a596ce11908e27dc90d0e815e12777bc8a2c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26079591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927ece7242fd0e3ae750a2f7f28d6e40dd4ebdaeceff867af7443db75d53c100`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 22:42:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 22:42:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 22:42:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 22:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 22:42:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 22:54:05 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 16 Jun 2021 22:54:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 22:54:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 22:54:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 22:54:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 16 Jun 2021 22:54:06 GMT
ENV PHP_VERSION=7.4.20
# Wed, 16 Jun 2021 22:54:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 16 Jun 2021 22:54:06 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Wed, 16 Jun 2021 22:54:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 22:54:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 25 Jun 2021 21:02:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 25 Jun 2021 21:02:57 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 25 Jun 2021 21:02:58 GMT
RUN docker-php-ext-enable sodium
# Fri, 25 Jun 2021 21:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 25 Jun 2021 21:02:59 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93eab99e0ef5f9d723ae4897063553cae85d76d084993a6ef1f4753c87cc5be`  
		Last Modified: Fri, 25 Jun 2021 21:42:26 GMT  
		Size: 1.8 MB (1804771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed49b65d5b9099a8d60337fc7a53d1ab0b053dc9d9ed95f1d212417c2f502f9`  
		Last Modified: Fri, 25 Jun 2021 21:42:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf026c104ba1de5b61fbc98582049fd882405b54f7b58a5db53aa5b999ff14c`  
		Last Modified: Fri, 25 Jun 2021 21:42:26 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46794a8ea871b2ab9dcb682abf487b16090c9a7acbea5a3113c2d4dd7e0acd6`  
		Last Modified: Fri, 25 Jun 2021 21:47:44 GMT  
		Size: 10.4 MB (10365311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d44fd7f90bafdfd0a04dc524d7215a7d03865d27e54891336b322ae17059dd`  
		Last Modified: Fri, 25 Jun 2021 21:47:43 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c361776350ac09e67542da361d53477245b656770d61afff7c20d8f821b97df`  
		Last Modified: Fri, 25 Jun 2021 21:47:46 GMT  
		Size: 11.1 MB (11066725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba9b6b7c03a144398cb10f7fc2f2a9c4745a5665d2e4f302fbe68ae44853921`  
		Last Modified: Fri, 25 Jun 2021 21:47:43 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077a6efa6b28398f2da50f3899c176e1f86af4139a812952a2e87a58ff0c673f`  
		Last Modified: Fri, 25 Jun 2021 21:47:43 GMT  
		Size: 17.8 KB (17782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-alpine` - linux; ppc64le

```console
$ docker pull php@sha256:065fc4ac40fb31b144d410b177f6a6a16777f69bd3ab13477becc2e64822e48b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26709761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699ceab3399dd6cb821f8799ee00d3c87dcaab40b630b1ab63a5b9118eef6fdf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:59:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 14 Apr 2021 20:59:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 21:00:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 21:00:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 21:00:12 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 04 Jun 2021 00:51:43 GMT
ENV PHP_VERSION=7.4.20
# Fri, 04 Jun 2021 00:51:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Fri, 04 Jun 2021 00:51:55 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Fri, 04 Jun 2021 00:52:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Jun 2021 00:52:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:57:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 00:57:25 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:57:37 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 00:57:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 00:57:46 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3580978f8a10d38890610248b0fcebc078a8b69524c7e5534ab57704ac495c9d`  
		Last Modified: Fri, 04 Jun 2021 01:19:56 GMT  
		Size: 10.4 MB (10365089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831619a33c68a77ba19582f943620a878a53afc3961c62e1a3be3ca90b3dd7cf`  
		Last Modified: Fri, 04 Jun 2021 01:19:54 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0a9d431ff8ec49a95e85f39cac05adddd2f5038c7162a194d37bde8ee35053`  
		Last Modified: Fri, 04 Jun 2021 01:19:57 GMT  
		Size: 11.8 MB (11761005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eda0ca75e6ad44c96336e43ac9f0691bfc96b2cd1bb4afe933aee6a2a0542a3`  
		Last Modified: Fri, 04 Jun 2021 01:19:54 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70096ec32eb07c5b49d43bc81aed8c201f701c24c2260728c694917d8ed3be4c`  
		Last Modified: Fri, 04 Jun 2021 01:19:54 GMT  
		Size: 17.6 KB (17596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-zts-alpine` - linux; s390x

```console
$ docker pull php@sha256:e5a92bbb5b67716be632ec35c4de2f5a46af2b33ec75aa34867ba4628ff6dd46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25476298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9878b8adcf6c498d60abcb2059ce03d4e819722a8e4079a4d83164997e0ed4ca`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:26:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Wed, 14 Apr 2021 19:26:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:26:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:26:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:26:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 04 Jun 2021 00:21:28 GMT
ENV PHP_VERSION=7.4.20
# Fri, 04 Jun 2021 00:21:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Fri, 04 Jun 2021 00:21:28 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Fri, 04 Jun 2021 00:21:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Jun 2021 00:21:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:25:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 00:26:00 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:26:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 00:26:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 00:26:03 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717f67eab3922199f01c1792b5df566a36ab321b4d1820ddf056774f27da444e`  
		Last Modified: Fri, 04 Jun 2021 00:44:46 GMT  
		Size: 10.4 MB (10365094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c90c93cc970cacc8af269f1db7e8e9440877c773e90dfb97455d07b6ec79ae`  
		Last Modified: Fri, 04 Jun 2021 00:44:45 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a1f26276c0717ed5c971cbc51003cca2df25a4dfcb84a829b81bc23ad972ae`  
		Last Modified: Fri, 04 Jun 2021 00:44:46 GMT  
		Size: 10.7 MB (10725969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166b0607e56344bdad262971db4fa7f3fd0a2548ea6dcf932d4367e0752e1602`  
		Last Modified: Fri, 04 Jun 2021 00:44:45 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2741eca32907aa1d5414cf53848cf808c26f00320b6ff6a7cd094ee45c946f14`  
		Last Modified: Fri, 04 Jun 2021 00:44:45 GMT  
		Size: 17.6 KB (17596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
