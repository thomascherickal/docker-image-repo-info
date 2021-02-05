## `php:cli-alpine3.13`

```console
$ docker pull php@sha256:36d654399ecefc4f9b9935b61eecfd77b43c9a0ad91756828c8dabdd0dee00b9
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

### `php:cli-alpine3.13` - linux; amd64

```console
$ docker pull php@sha256:bd82036c78a96d27fe31a4489645d9b321e182bfa429a708952b64704a697ebf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30144246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9484fd084dd9214be29452b1a6c60adc7e55b347b3d734946d75bccae12eb881`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:09:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:09:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:09:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:09:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:09:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:09:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:09:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:09:36 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 04:22:44 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 04:22:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 04:22:44 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 04:22:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 04:22:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 04:34:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 04:34:02 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 05 Feb 2021 04:34:04 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 04:34:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 04:34:05 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed03eff2d6362e11708d8c6c19ad4c39f85830d917a40c5254ff7f589caa9982`  
		Last Modified: Fri, 29 Jan 2021 02:50:08 GMT  
		Size: 1.7 MB (1694844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67667da1de1f032c9daa354a18c7525286103540b8f4a884606ccdef49006f`  
		Last Modified: Fri, 29 Jan 2021 02:50:07 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6961b2fabe936ad3c26fc41f241379caba86b0d660acaf263f971d8d33e4219b`  
		Last Modified: Fri, 29 Jan 2021 02:50:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0ff0908eb3be4251b34a25d351665d82968a1c98b7ba83475e23af3222d267`  
		Last Modified: Fri, 05 Feb 2021 05:05:21 GMT  
		Size: 10.7 MB (10669904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3194413ee7dec46105ab569c2873edb1523e2121f683b3eae92489c272628f`  
		Last Modified: Fri, 05 Feb 2021 05:05:20 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3f9163b801e059a4236391e25f963c3f539461cfece99c0016168ca1cd472e`  
		Last Modified: Fri, 05 Feb 2021 05:05:24 GMT  
		Size: 14.9 MB (14946438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68aac131d818516ba0378057d5d3e3fbef370b2c7332d5d13f6175c9114b8004`  
		Last Modified: Fri, 05 Feb 2021 05:05:21 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4e7f70d907634f5d04c3b2100e94f90177d4c4caedafb3520a1e49e9a440cc`  
		Last Modified: Fri, 05 Feb 2021 05:05:30 GMT  
		Size: 17.5 KB (17527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.13` - linux; arm variant v6

```console
$ docker pull php@sha256:c5babff3e9e76682eea35fa16fb37390c81b94a92083911aa428ae288b91704b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28580406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddfad2f61a2ba46fab482aa75806483d974bb1b1a6bd441491c312490a18af34`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:33:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 00:33:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 00:33:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 00:34:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 00:34:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 00:34:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:34:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:34:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:34:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 02:28:27 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 02:28:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 02:28:29 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 02:28:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 02:28:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 02:31:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 02:31:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 05 Feb 2021 02:31:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 02:31:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 02:31:57 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa34846effbef1e901021c65a67535efc29a1aa39b259a4c29559d1439f4131`  
		Last Modified: Fri, 29 Jan 2021 01:05:52 GMT  
		Size: 1.7 MB (1684855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba088c5e0e1fb4c64a8b59354bedcae82636c10a93fe3790125bec5c1e841299`  
		Last Modified: Fri, 29 Jan 2021 01:05:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b10584422ada7d37ac091eae04bcee5df4cee5b93cd86068ce55c7ab085ae62`  
		Last Modified: Fri, 29 Jan 2021 01:05:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63629fd33790bdb39f8c140251809bd392c3f6f92d331090b2c6e9ca4a8eaad3`  
		Last Modified: Fri, 05 Feb 2021 02:47:49 GMT  
		Size: 10.7 MB (10669921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc693263993b2cd90d46c7c10fa9f4c31d698948f6537d1a4c26984715a172a0`  
		Last Modified: Fri, 05 Feb 2021 02:47:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b4fe73a2196e7a190b5456dc967a1a3d882810ff5cc0aa5a8f74d933999fe2`  
		Last Modified: Fri, 05 Feb 2021 02:47:54 GMT  
		Size: 13.6 MB (13582054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae87ff7ee620e8dfa072549a643076caa6b2d58700a00425ea93974eab3ec7a`  
		Last Modified: Fri, 05 Feb 2021 02:47:47 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e144fadde578c3382d77440cd608a4af5d01a4a994876dfa4f2c16f421811f`  
		Last Modified: Fri, 05 Feb 2021 02:47:47 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.13` - linux; arm variant v7

```console
$ docker pull php@sha256:da0ff08ed4181a220f8769f4bfc2139c9829c3eb08f35144f85238ad16b48a36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27397390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d95f8dca84d5d93dc7f7a7b5764d938ce8dc4ff86ffbbc59580800139798bf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:06:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:06:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:06:46 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:06:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:06:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:06:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:06:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:06:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:06:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 03:13:47 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 03:13:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 03:13:49 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 03:13:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 03:13:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:16:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 03:16:59 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:17:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 03:17:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 03:17:03 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85929efbae7230a09dc3cfdea4cf9d3cb6406e6d08ea1f1f27c0f2cbeac922b8`  
		Last Modified: Fri, 29 Jan 2021 01:42:34 GMT  
		Size: 1.6 MB (1555132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5e29134f861e9b4885f23eae2f99d8886b0dcd558b80afc619e2044102346`  
		Last Modified: Fri, 29 Jan 2021 01:42:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7241eb5d2691c2e356b0deeeceebaa6eec6e60e5db535473c1c5940502649f00`  
		Last Modified: Fri, 29 Jan 2021 01:42:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2857f4bc54a57843a8c91dfa1b6034e164c18e7cc6509806dc0ec697296af93c`  
		Last Modified: Fri, 05 Feb 2021 03:32:59 GMT  
		Size: 10.7 MB (10669916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62a4e3659d86ecfac6190ff41c234703dc86b612c303c841d6264a02fad12a5`  
		Last Modified: Fri, 05 Feb 2021 03:32:58 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b457e4490f5f772aa86cfa4ada0c58830ad2777efd7c7c4671d8a4d0c5682dd7`  
		Last Modified: Fri, 05 Feb 2021 03:33:02 GMT  
		Size: 12.7 MB (12726964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7573dd5523f72f590fdf2773417de93bac4ac0514d53839c68a476b77a3e8fe3`  
		Last Modified: Fri, 05 Feb 2021 03:32:58 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76986fb7f21509746233e01cf5851eb5d5b3f9b6dc8efecf4b79feb7423d23a9`  
		Last Modified: Fri, 05 Feb 2021 03:32:58 GMT  
		Size: 17.5 KB (17530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull php@sha256:981e26674ea8b51854a798b99dfa5774eedea5c6de94cc78e782569f8ee6586a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29472606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc246e125ec68bdb08099c4b8def7631c69be8fd646497696eb64fc1a0c5fad8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:27:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:27:39 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:27:43 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:27:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:27:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:27:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:27:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:27:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:27:52 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 02:59:25 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 02:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 02:59:26 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 02:59:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 02:59:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:03:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 03:03:46 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:03:49 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 03:03:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 03:03:52 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878faaa0cbd74b5e94aae0682e345b19f40d9f47ce41b90494c9ab94e12a1606`  
		Last Modified: Fri, 29 Jan 2021 02:09:31 GMT  
		Size: 1.7 MB (1694574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12efacc7494753eaf44ab2bfe05cc02be70cae3241be0b5fe2378c9f8c7b36c9`  
		Last Modified: Fri, 29 Jan 2021 02:09:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1212c0105c6a0060dfb2a16f744f1e40aa7ce3e9957450ee00a8f86934141a10`  
		Last Modified: Fri, 29 Jan 2021 02:09:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56550b3454fe8b1491000595ec00044e7fe62e0aa019e56b4dda3604c7f1aad`  
		Last Modified: Fri, 05 Feb 2021 03:23:05 GMT  
		Size: 10.7 MB (10669944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486a09530da8f25442968050b5494c0403bd1f527b96f02c0f4eff4aa065e5df`  
		Last Modified: Fri, 05 Feb 2021 03:23:00 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439a71d1567635efe464149f15871ede5859b7103d0e3356ccd6a606dd052d2`  
		Last Modified: Fri, 05 Feb 2021 03:23:05 GMT  
		Size: 14.4 MB (14375005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54c6040a9afe7b72dba3f46befe15ddd287261d483540588357f3cde16261b7`  
		Last Modified: Fri, 05 Feb 2021 03:23:00 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4671b4ac11f21d979f21b08b3b32c77bcd53c98b89d53833953664721f42ee`  
		Last Modified: Fri, 05 Feb 2021 03:23:00 GMT  
		Size: 17.5 KB (17536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.13` - linux; 386

```console
$ docker pull php@sha256:bdc9e7c986872d7ad2a987cc813562c4732605a870f8246fe29eb0b34768bab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30274339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4c08d3fac3fbc31e730fc914e819c3ef15a58813b791720b000214ad32e3ec`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:16:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:16:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:16:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:16:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:16:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:16:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:16:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:16:36 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 02:55:12 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 02:55:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 02:55:13 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 02:55:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 02:55:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:06:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 03:06:45 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:06:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 03:06:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 03:06:47 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7693c189358487be8693c8f24f54e75dc5e54a6d33edc79a7ddf6851c9f2e670`  
		Last Modified: Fri, 29 Jan 2021 03:00:10 GMT  
		Size: 1.8 MB (1793522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2956bde582e6c6782cd1f42ba90c812f6449eec18badce15706f72fb5fed3db4`  
		Last Modified: Fri, 29 Jan 2021 03:00:07 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eb950875108b8e92353d43040a08536210b13d2ea2a265b8a93f88149d556f`  
		Last Modified: Fri, 29 Jan 2021 03:00:08 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca903ef08ae3bbcf42454b82fc0d17632a9f27d41d88b54af3489a15361d017`  
		Last Modified: Fri, 05 Feb 2021 03:43:27 GMT  
		Size: 10.7 MB (10669888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21a3626d25fc511a2f2706c0191f3cb548cba2b240697873b6a0532a90842b4`  
		Last Modified: Fri, 05 Feb 2021 03:43:24 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0163f74f2fae72844c560e12c351e39f5c2c92c6c4c1d54eb4cec1d6c1bb16f`  
		Last Modified: Fri, 05 Feb 2021 03:43:34 GMT  
		Size: 15.0 MB (14971581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ed3d94022de518cfa6d73eebfa2266be18eb1c4eb9c29fd3e23d1918836cc5`  
		Last Modified: Fri, 05 Feb 2021 03:43:24 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec5f2ab4b0a4e8fb0617473ee71770e74107d2c2f319cc8483dce07e585f446`  
		Last Modified: Fri, 05 Feb 2021 03:43:24 GMT  
		Size: 17.5 KB (17509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.13` - linux; ppc64le

```console
$ docker pull php@sha256:76b2b2ee1fbad0aff0bce6b3f739c2eba949be6f9baa5185a05c6675cb71f65e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30901272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774fa1564f2cca500f0ec8c29270c82e893ba79f73abb0ed9ec00d0649815e0f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:47:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 00:47:11 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 00:47:28 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 00:47:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 00:47:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 00:47:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:47:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:47:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:47:57 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 29 Jan 2021 00:48:02 GMT
ENV PHP_VERSION=8.0.1
# Fri, 29 Jan 2021 00:48:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 29 Jan 2021 00:48:08 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 29 Jan 2021 00:48:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 00:48:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:53:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 00:53:24 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:53:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 00:53:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 00:53:43 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9051dfce6625cce4ab1471f70365886b7c23ec19442e08bf3bc297f0a38d57f6`  
		Last Modified: Fri, 29 Jan 2021 01:43:50 GMT  
		Size: 1.7 MB (1741752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82481345688ea8ca47c72ddbbae52d55e215ba3458011ffc13503f16e7caba02`  
		Last Modified: Fri, 29 Jan 2021 01:43:48 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06851413a731c975b7b2d96c8a3ebb2848c57555cf34ab98ca93d7873280b947`  
		Last Modified: Fri, 29 Jan 2021 01:43:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f94bb7dfd6d7c3433e155d8826545ab119407094d3ec2902f38a72b2330fc7f`  
		Last Modified: Fri, 29 Jan 2021 01:43:45 GMT  
		Size: 10.7 MB (10661702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652889176bda203930001efad52057fe986cbc2aa486d7f5282bbea7a316351b`  
		Last Modified: Fri, 29 Jan 2021 01:43:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121059a52f3fb2dec15d1b413eec967a4bddfc9824aaac7813ee59efc53485c7`  
		Last Modified: Fri, 29 Jan 2021 01:43:47 GMT  
		Size: 15.7 MB (15663484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6b7e901eb8104c83ec2a931b1ec85cb33367b423a8521953450855b91b097d`  
		Last Modified: Fri, 29 Jan 2021 01:43:43 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a57d63f94080c81df8c8f4455d48d31bd45ceb921457434bfc1ed42b29b0e8`  
		Last Modified: Fri, 29 Jan 2021 01:43:43 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.13` - linux; s390x

```console
$ docker pull php@sha256:615b7b34c2fdff5c072cb260b47bdc791fc560ce88af8c29d581fe16d20260ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29018699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17964c01de47cf7d0600f8ddee9fba08ebd8222bbc82758f2b32309c755aace4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:38:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 00:38:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 00:38:40 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 00:38:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 00:38:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 00:38:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:38:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:38:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:38:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 09:21:20 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 09:21:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 09:21:22 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 09:21:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 09:21:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 09:29:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 09:29:51 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 05 Feb 2021 09:29:58 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 09:29:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 09:29:59 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ca6a535daf2f11149d562663f17aa1c644768776000a66fbf3c3a408575b41`  
		Last Modified: Fri, 29 Jan 2021 01:20:34 GMT  
		Size: 1.8 MB (1756344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49dba0dd587ac68bb7a364dfb548d9e4c5725a4e26f9c844457805036cfa6cb`  
		Last Modified: Fri, 29 Jan 2021 01:20:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10d9258fa200837167aa8dd3a89838c0c749ff3167f7eaea8db0ef3b421a99`  
		Last Modified: Fri, 29 Jan 2021 01:20:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc155458e7a909b1f3a77c38e065f2691294846cf17a3f31f3c2bbaa2707dd2`  
		Last Modified: Fri, 05 Feb 2021 10:19:20 GMT  
		Size: 10.7 MB (10669926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08033927b4bb2cbf57d75653bb092a00032dccee7c0c8c56f27d89044bbe1d5d`  
		Last Modified: Fri, 05 Feb 2021 10:19:19 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd41f354dcdb5eba20dd8db89eb3942011948b8927bce9d9e28cd43fd8c6a08`  
		Last Modified: Fri, 05 Feb 2021 10:19:19 GMT  
		Size: 14.0 MB (13968551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a6b57c575ada8e08775ea78caafbf0f959b621805c448628d884092cf00cbb`  
		Last Modified: Fri, 05 Feb 2021 10:19:19 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b82eec856c9841bea7a9ce24e51fa197820a82f59fa92d38363ce73849c19b`  
		Last Modified: Fri, 05 Feb 2021 10:19:19 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
