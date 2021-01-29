## `composer:latest`

```console
$ docker pull composer@sha256:2d2e012198a35b7312007adac8048bf30b6f32841eddb48c8c2910b0ef856baf
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

### `composer:latest` - linux; amd64

```console
$ docker pull composer@sha256:005d4a50002fcf58eb93b749345b73441cb615644f0790844538d0990cc3ce20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62417362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21e0bd4ead1c9c98e491c19a4b10307760a1a5060996f40e5f5229bd6882b578`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 15 Jan 2021 02:23:51 GMT
ADD file:edbe213ae0c825a5bfbe569928cf20f683f334f93a093ccd0a3a014b7428e760 in / 
# Fri, 15 Jan 2021 02:23:51 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:43:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:43:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:43:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:43:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:43:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:43:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:43:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:43:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:43:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 23:43:30 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 23:43:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 23:43:31 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 23:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:43:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:51:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 20:17:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:17:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 20:17:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 20:17:51 GMT
CMD ["php" "-a"]
# Thu, 28 Jan 2021 22:32:03 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 28 Jan 2021 22:32:24 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 28 Jan 2021 22:32:24 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 28 Jan 2021 22:32:25 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 28 Jan 2021 22:32:25 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 28 Jan 2021 22:32:25 GMT
ENV COMPOSER_VERSION=2.0.9
# Thu, 28 Jan 2021 22:32:27 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 28 Jan 2021 22:32:27 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 28 Jan 2021 22:32:28 GMT
WORKDIR /app
# Thu, 28 Jan 2021 22:32:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 28 Jan 2021 22:32:28 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:596ba82af5aaa3e2fd9d6f955b8b94f0744a2b60710e3c243ba3e4a467f051d1`  
		Last Modified: Fri, 15 Jan 2021 02:08:10 GMT  
		Size: 2.8 MB (2810825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74f285bb27c6623f2b5c8c3a2e487603c7dd5c51859fd6e13859542f4310c3`  
		Last Modified: Sat, 16 Jan 2021 01:00:24 GMT  
		Size: 1.7 MB (1694838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab8440e5667ccb2ffd4e62ed905a106742dfdd7dd3167d9d64b4bdeed8a4945`  
		Last Modified: Sat, 16 Jan 2021 01:00:20 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64889fa545ec919e6fe392c368b8cb41a10e7834c1ba4d4d96fd9ee2e3405cc1`  
		Last Modified: Sat, 16 Jan 2021 01:00:20 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94168e6487351b04d28db6aabb22e0c68ad3582533cf8d7e00322078720f8081`  
		Last Modified: Sat, 16 Jan 2021 01:00:19 GMT  
		Size: 10.7 MB (10661716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3898f14298ef25ab2005e9025a88f553003a83a1b6a61765e93d78879441aa36`  
		Last Modified: Sat, 16 Jan 2021 01:00:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3747e5f21671eba796a4b76a6abc180c60b0ef9414e9a80b325b31aeaa1f6ca`  
		Last Modified: Sat, 16 Jan 2021 01:00:21 GMT  
		Size: 15.3 MB (15318011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3df0f8088890764041d8dbfe574cd5bdf020400801b0b108cd6b7f965aab3a`  
		Last Modified: Thu, 21 Jan 2021 20:28:34 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6ddeaf0bdcf495df2e7c8d72852796c1bae3d9f8ef8260058fdb43b995163`  
		Last Modified: Thu, 21 Jan 2021 20:28:34 GMT  
		Size: 17.5 KB (17539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29338fcaf9eb090ba02397a08616210ac758731039ac2d2a5db97288090a1845`  
		Last Modified: Thu, 28 Jan 2021 22:32:55 GMT  
		Size: 31.2 MB (31158400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a0bf379d52ae6a08ffd2313828e5738aa1cfd2a934c2403e6065ae7f94ba05`  
		Last Modified: Thu, 28 Jan 2021 22:32:49 GMT  
		Size: 198.3 KB (198274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a346beb5e7dfc07424d1d661858912a89fab48a63bd89492e0c97c3cf1a6c75`  
		Last Modified: Thu, 28 Jan 2021 22:32:49 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e86daf479799f96a49bc265571da38b2be4344f28a6b8ed4a0a18cb1dafae08`  
		Last Modified: Thu, 28 Jan 2021 22:32:49 GMT  
		Size: 552.8 KB (552794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048afd2f48877072346dfbc095e6883b2ccc828164f17723d6e95d230c798b83`  
		Last Modified: Thu, 28 Jan 2021 22:32:49 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad27987395f1263b907d761fc5f4b5a356869262f62cd2b055f7c8bb050317ac`  
		Last Modified: Thu, 28 Jan 2021 22:32:49 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v6

```console
$ docker pull composer@sha256:8555fcdcc559af5253afc8400e8f2f92937211b20947c2b1d231b3ab2a703663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58265639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d766a7469442cfbfeb325a177218e32152d532c8efaec2dd15a2fd56020467`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

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
# Fri, 29 Jan 2021 00:34:11 GMT
ENV PHP_VERSION=8.0.1
# Fri, 29 Jan 2021 00:34:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 29 Jan 2021 00:34:13 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 29 Jan 2021 00:34:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 00:34:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:37:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 00:37:35 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:37:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 00:37:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 00:37:40 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 02:11:29 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 29 Jan 2021 02:11:49 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 29 Jan 2021 02:11:51 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 29 Jan 2021 02:11:51 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Jan 2021 02:11:52 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Jan 2021 02:11:52 GMT
ENV COMPOSER_VERSION=2.0.9
# Fri, 29 Jan 2021 02:11:55 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 29 Jan 2021 02:11:56 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 29 Jan 2021 02:11:57 GMT
WORKDIR /app
# Fri, 29 Jan 2021 02:11:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Jan 2021 02:11:58 GMT
CMD ["composer"]
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
	-	`sha256:fdd2125b643842a0b1fb7799c57d504cb3ea72f1cdaac6d48b6d3ee2fa033d39`  
		Last Modified: Fri, 29 Jan 2021 01:05:50 GMT  
		Size: 10.7 MB (10661723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370c8d7d436fffa9dd306db82b4a90f7b25ae1d68c658dac4c195ec6a921976e`  
		Last Modified: Fri, 29 Jan 2021 01:05:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c1bd9522799773adb723d78cef494168d851dd759ef42bdf230e3518c9888d`  
		Last Modified: Fri, 29 Jan 2021 01:05:54 GMT  
		Size: 13.6 MB (13571709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b70fa5215a21be024094dd917f70d206590186d21137fcb75d1fb68a887a2`  
		Last Modified: Fri, 29 Jan 2021 01:05:49 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b25bcaba65cbff9b151c9ab65d005350d890d7728bfe14024f5f4bd9ca890`  
		Last Modified: Fri, 29 Jan 2021 01:05:49 GMT  
		Size: 17.5 KB (17531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dda7886eea28b54dfe2eea50537d02027bbbcda31bb0d081dff700b99290584`  
		Last Modified: Fri, 29 Jan 2021 02:12:41 GMT  
		Size: 29.0 MB (28956651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90907b51293338df699b9f07cbb70441610fa8f2924e32d21967026449fe4064`  
		Last Modified: Fri, 29 Jan 2021 02:12:28 GMT  
		Size: 193.5 KB (193490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85552216f6bbc21bc776e9622f10a51b96b9a92310894072d91339b4fe625b1e`  
		Last Modified: Fri, 29 Jan 2021 02:12:28 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277406688472a6794691f5e4a67b9a1fff148488bd3592f46c1ff32c50b9e712`  
		Last Modified: Fri, 29 Jan 2021 02:12:28 GMT  
		Size: 552.8 KB (552840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adf754bdf3aa207b3395bac818c602ae3326449c8eef1d435c2deefb3a2dd0`  
		Last Modified: Fri, 29 Jan 2021 02:12:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d326c954a1dde2641329fe23cd34f82ea22e784961b8e5e3098ea38e58e06bf`  
		Last Modified: Fri, 29 Jan 2021 02:12:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v7

```console
$ docker pull composer@sha256:f13a72b2af8baea99b06a09475bb86fcfdafabdb9e735b095b2b4f84986b1d0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55741665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d653ad4903851b7e67f0a926e4f330bfeacbbc40530ee049bd86ed9e3ef726d5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

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
# Fri, 29 Jan 2021 01:06:52 GMT
ENV PHP_VERSION=8.0.1
# Fri, 29 Jan 2021 01:06:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 29 Jan 2021 01:06:53 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 29 Jan 2021 01:06:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:06:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:09:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:09:58 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:10:01 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:10:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:10:03 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 04:02:40 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 29 Jan 2021 04:03:01 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 29 Jan 2021 04:03:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 29 Jan 2021 04:03:09 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Jan 2021 04:03:10 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Jan 2021 04:03:11 GMT
ENV COMPOSER_VERSION=2.0.9
# Fri, 29 Jan 2021 04:03:14 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 29 Jan 2021 04:03:15 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 29 Jan 2021 04:03:15 GMT
WORKDIR /app
# Fri, 29 Jan 2021 04:03:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Jan 2021 04:03:19 GMT
CMD ["composer"]
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
	-	`sha256:267c5de2407f9c610f687cd02181b85cfbc80aa78b00dc8df1f74f722d813aa7`  
		Last Modified: Fri, 29 Jan 2021 01:42:33 GMT  
		Size: 10.7 MB (10661715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7ac54305cb9b12a36a08c89f48a36ec691370f32e4bf2ae6ed884f7bd98353`  
		Last Modified: Fri, 29 Jan 2021 01:42:32 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438ddb97ac647203517fba653508c2cdbaf8f1e2412f9bfc158a18fd3022ad1a`  
		Last Modified: Fri, 29 Jan 2021 01:42:36 GMT  
		Size: 12.7 MB (12704007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415ddff3c5d1ba737a3a3fc9acebb4321479f1a0c53e621949cef4b1f29ae10b`  
		Last Modified: Fri, 29 Jan 2021 01:42:31 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a9ea8e3758cb1f01a7b4dd8d3a1acced921aeb0db3b8ead1fc26986dbca6ef`  
		Last Modified: Fri, 29 Jan 2021 01:42:31 GMT  
		Size: 17.5 KB (17523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014fb7bd207b9cd14b7353c8abc6783f978b77df1ce874dba055c6021527b5c6`  
		Last Modified: Fri, 29 Jan 2021 04:04:02 GMT  
		Size: 27.6 MB (27635536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59ab60603bcb1e812ec9318bf38d77a7915d63de74abb059b249c71d72d2582`  
		Last Modified: Fri, 29 Jan 2021 04:03:51 GMT  
		Size: 186.3 KB (186285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6137a7287b362bf569d56b73bb8b167b0849a7a922c05046ef2c75cc329a5`  
		Last Modified: Fri, 29 Jan 2021 04:03:51 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2cc8f5628aaf6ba9cd552fbbe3a41cb7ee433fbe7ed281ad4a11b1303d3a93`  
		Last Modified: Fri, 29 Jan 2021 04:03:51 GMT  
		Size: 552.8 KB (552834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876cbd991c8b9dfa9b42d16a8f0e69adafac9f5db7023c8684f355450bee59d`  
		Last Modified: Fri, 29 Jan 2021 04:03:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45523f6d4d8a0503920bee311715cf93652bc3e91281c048f00ccf8b0dce78e4`  
		Last Modified: Fri, 29 Jan 2021 04:03:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:decabcc6e2913a9333c502413f27dc66339ac9fa66656bc4b0dd7bf604824709
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61578075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae9090aeafa1c7f956ee135261de2cdf81ebc0e73fa021d494d1ad2f8090d10`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

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
# Fri, 29 Jan 2021 01:27:53 GMT
ENV PHP_VERSION=8.0.1
# Fri, 29 Jan 2021 01:27:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 29 Jan 2021 01:27:55 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 29 Jan 2021 01:28:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:28:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:32:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:32:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:32:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:32:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:32:49 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 02:58:50 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 29 Jan 2021 02:59:11 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 29 Jan 2021 02:59:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 29 Jan 2021 02:59:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Jan 2021 02:59:16 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Jan 2021 02:59:17 GMT
ENV COMPOSER_VERSION=2.0.9
# Fri, 29 Jan 2021 02:59:20 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 29 Jan 2021 02:59:21 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 29 Jan 2021 02:59:22 GMT
WORKDIR /app
# Fri, 29 Jan 2021 02:59:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Jan 2021 02:59:24 GMT
CMD ["composer"]
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
	-	`sha256:0693db536d04b5948e2cc9286e5efec81b943bb03e41543552032ef9864ad2ca`  
		Last Modified: Fri, 29 Jan 2021 02:09:29 GMT  
		Size: 10.7 MB (10661736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a0d26b0a525c699f348c37abb9b859a7f5845a7115d799cc402e182cf7a516`  
		Last Modified: Fri, 29 Jan 2021 02:09:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432fd9b62b67077d59247b991e2bd57ada06a70fa0a2e2d43dce5af8de61cd33`  
		Last Modified: Fri, 29 Jan 2021 02:09:32 GMT  
		Size: 14.4 MB (14362682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8713b4138b76135d4111770c881c6c4ae39a6fd4d5b6ecdf1ef5105c2bb83`  
		Last Modified: Fri, 29 Jan 2021 02:09:28 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160cf685a5abfdc85c57bfcdf259ac1dc1d4cbcf3e634de979148e7eb990759e`  
		Last Modified: Fri, 29 Jan 2021 02:09:28 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9671a0d249ed6986e7aece723b73539b453be87dc58333cd5c457eec9a66903`  
		Last Modified: Fri, 29 Jan 2021 03:00:04 GMT  
		Size: 31.4 MB (31376350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231b0bc739b252a825b19e287233b5c41966952bca1eea0eb9d70b57d9c6454d`  
		Last Modified: Fri, 29 Jan 2021 02:59:52 GMT  
		Size: 196.0 KB (196021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93324ea0b6082334f6f1484e16f4a9868c47fac2ce6505bf87438c0050f9f636`  
		Last Modified: Fri, 29 Jan 2021 02:59:52 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556bb7b740c52f406796d128ae51c03ed53c55f49861b8f61cbe8ff3aa41232f`  
		Last Modified: Fri, 29 Jan 2021 02:59:53 GMT  
		Size: 552.8 KB (552843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbe33a940d7c394a338002f55c371881a5c6b460bd2eb2995c37584bd5b4ec5`  
		Last Modified: Fri, 29 Jan 2021 02:59:52 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2db434fa921fc9359703740c614987dee112bbc76edb14c13b09e098baea12`  
		Last Modified: Fri, 29 Jan 2021 02:59:52 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; 386

```console
$ docker pull composer@sha256:d1366c8963cfab30a01f8eaf0c86def4785d85fcd67616b0325ad4e4e4633832
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63702654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af66081ead599dedc0d793ecd53ecd5631d90a00ce2dfb71be5d837044975ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 15 Jan 2021 01:38:28 GMT
ADD file:d8723c02f1eb0efa4dadc6480a753d18d7e28d9815bff96a92ff09ff55a92b11 in / 
# Fri, 15 Jan 2021 01:38:29 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:42:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:42:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:42:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:42:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:42:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:42:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:42:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:42:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 22:42:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 22:42:25 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 22:42:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 22:42:25 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 22:42:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 22:42:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 22:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:44:48 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:44:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:44:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:44:51 GMT
CMD ["php" "-a"]
# Thu, 28 Jan 2021 22:38:41 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 28 Jan 2021 22:38:56 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 28 Jan 2021 22:38:57 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 28 Jan 2021 22:38:57 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 28 Jan 2021 22:38:57 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 28 Jan 2021 22:38:57 GMT
ENV COMPOSER_VERSION=2.0.9
# Thu, 28 Jan 2021 22:38:59 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 28 Jan 2021 22:39:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 28 Jan 2021 22:39:00 GMT
WORKDIR /app
# Thu, 28 Jan 2021 22:39:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 28 Jan 2021 22:39:00 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:9e6a151110e36daa7a487250f98425289313f856e3a586d89d82bafc1bf322c3`  
		Last Modified: Fri, 15 Jan 2021 01:39:01 GMT  
		Size: 2.8 MB (2817152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b194694eae0c8525a66d3c56796eb37a9e263d63f03eaecf6bc83d2ab3f7c9`  
		Last Modified: Fri, 15 Jan 2021 23:50:55 GMT  
		Size: 1.8 MB (1793505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a9a95dec7f2cd3bcf6903d006a870fa7113f6a974d30ec6634ab82b0a0a792`  
		Last Modified: Fri, 15 Jan 2021 23:50:52 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ad687f5cfc54121cc70af5ff69cb844177c4325a2c14efcd144cb096ecfba2`  
		Last Modified: Fri, 15 Jan 2021 23:50:54 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ae4debbbbc31db383a639e6a7df85ebf9c2f15905a9ec2df4fb8a3998dec90`  
		Last Modified: Fri, 15 Jan 2021 23:50:56 GMT  
		Size: 10.7 MB (10661677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900efcbd73b95b91ec42e946efd16fa2e312e57beba40e9aac2b0699baa90d1d`  
		Last Modified: Fri, 15 Jan 2021 23:50:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c042850cc5dcebe86c931da9e6014fe607a6c507fe5a61059ba47003a80cac2`  
		Last Modified: Fri, 15 Jan 2021 23:51:00 GMT  
		Size: 15.3 MB (15348857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a592432a0a1e356653687e23dd3c8f953d0fc904db0377fa898de0c851be229d`  
		Last Modified: Thu, 21 Jan 2021 19:55:39 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3b6898b8d491988e64358ef661f654c98cbec8cc3e36edeedea25334aae60e`  
		Last Modified: Thu, 21 Jan 2021 19:55:40 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fcd335e71480482247bfd7863baa60db887184f8227377b99d22f61dc2a4d6`  
		Last Modified: Thu, 28 Jan 2021 22:39:38 GMT  
		Size: 32.3 MB (32292342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f574926dca5384453b345a61350707cbf2753926b84e8c685a1899bbe6ff5b`  
		Last Modified: Thu, 28 Jan 2021 22:39:28 GMT  
		Size: 213.8 KB (213825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25022b6f8e9b3bd588f8db12caab7e929709dcb604f7f84786e3a7d54f6bd2f4`  
		Last Modified: Thu, 28 Jan 2021 22:39:28 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383490e188660eeea8b6c894366164f4300f53b351efbc251fa34ccd12a24504`  
		Last Modified: Thu, 28 Jan 2021 22:39:28 GMT  
		Size: 552.8 KB (552799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7647a67da25834616edba6106817cca07fa93408500bf11d4aaa476837b4bcb1`  
		Last Modified: Thu, 28 Jan 2021 22:39:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eedfded7d6e258e16f2eec203d90eaa4b9de30b187ba609ee65940bf265403`  
		Last Modified: Thu, 28 Jan 2021 22:39:28 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; ppc64le

```console
$ docker pull composer@sha256:516f1b8e91b56e6135fe3434d5cd789140e2c5c750bd57b2671dd5981e70225c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63652505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:978e628973fc7b3354ff2c6d8f8ac19e7b69d32fb8476b72b3c75885239de68c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

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
# Fri, 29 Jan 2021 03:56:41 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 29 Jan 2021 03:57:24 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 29 Jan 2021 03:57:50 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 29 Jan 2021 03:57:57 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Jan 2021 03:58:05 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Jan 2021 03:58:15 GMT
ENV COMPOSER_VERSION=2.0.9
# Fri, 29 Jan 2021 03:58:46 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 29 Jan 2021 03:58:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 29 Jan 2021 03:59:17 GMT
WORKDIR /app
# Fri, 29 Jan 2021 03:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:59:46 GMT
CMD ["composer"]
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
	-	`sha256:57b72e6b43921e2a3bd09e9d5046210632cb21f1d952c87952b6c20f88dd0e5c`  
		Last Modified: Fri, 29 Jan 2021 04:01:45 GMT  
		Size: 32.0 MB (31993572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264d7ad348e64953565f77489818b0cbb34e574fd5e003495ab1017715d9dfc4`  
		Last Modified: Fri, 29 Jan 2021 04:01:32 GMT  
		Size: 204.0 KB (204021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08a800584251e4a3c4eb7d0a4ca3986bf5ffbff8226baa149913a30922873ac`  
		Last Modified: Fri, 29 Jan 2021 04:01:32 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1607a1ee4c6778dffd77dde901e6889fdf55266a3bb27ae407f8422ad3e27`  
		Last Modified: Fri, 29 Jan 2021 04:01:32 GMT  
		Size: 552.9 KB (552851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb0271a34e3a4a1764016ca9fbb214b60552eaafdc4f735ae7a1b8e69911111`  
		Last Modified: Fri, 29 Jan 2021 04:01:32 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbd616341e72152b1947babd4e214262957187deea299ee4ed66cdafb614cb5`  
		Last Modified: Fri, 29 Jan 2021 04:01:31 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; s390x

```console
$ docker pull composer@sha256:d59342ab4044b5c7e97887b6e5c4d763703cd40a655d4071bccc778bf5d111f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61144564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff52061ce6a9f8ed8952cee6687cc68a4186c834d5308904f29e1abf0dc232d7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

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
# Fri, 29 Jan 2021 00:38:43 GMT
ENV PHP_VERSION=8.0.1
# Fri, 29 Jan 2021 00:38:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 29 Jan 2021 00:38:44 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 29 Jan 2021 00:38:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 00:38:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 00:43:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:43:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 00:43:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 00:43:19 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 02:33:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 29 Jan 2021 02:33:30 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 29 Jan 2021 02:33:32 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 29 Jan 2021 02:33:33 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Jan 2021 02:33:33 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Jan 2021 02:33:34 GMT
ENV COMPOSER_VERSION=2.0.9
# Fri, 29 Jan 2021 02:33:36 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/keys.dev.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub;   curl --silent --fail --location --retry 3 --output /tmp/keys.tags.pub --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 29 Jan 2021 02:33:36 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 29 Jan 2021 02:33:37 GMT
WORKDIR /app
# Fri, 29 Jan 2021 02:33:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Jan 2021 02:33:38 GMT
CMD ["composer"]
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
	-	`sha256:3e1ae2f3457c79f0a0e5e2322c5d1c25c476a5ba0f9b75fe829d561b26e58877`  
		Last Modified: Fri, 29 Jan 2021 01:20:32 GMT  
		Size: 10.7 MB (10661727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d5a7bcb5c0dc18c34af028d62dc4abee99dda7059eed197f1253cbbc51fc5b`  
		Last Modified: Fri, 29 Jan 2021 01:20:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c14d7f9eeef4534d8b3befcbdc431a27f490061473693547ec6d43d4bf7603`  
		Last Modified: Fri, 29 Jan 2021 01:20:33 GMT  
		Size: 14.0 MB (13962274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cfee97bd289ec1d9d3997c87c9931a1005a765699ee08ba011ea71e8bdfe2`  
		Last Modified: Fri, 29 Jan 2021 01:20:31 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c352e304bbb172dc76649f03b99a41f4669dde43b82681152946134729c3`  
		Last Modified: Fri, 29 Jan 2021 01:20:31 GMT  
		Size: 17.5 KB (17519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c76fac5cb408f52536c401cd77d43535820166daf2a70680088d60bbc3c18a`  
		Last Modified: Fri, 29 Jan 2021 02:34:22 GMT  
		Size: 31.4 MB (31388945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8b94ee1d77b230dca3c81ae2100b6d395d85599f8a41f65c7c254c8a1dc25`  
		Last Modified: Fri, 29 Jan 2021 02:34:05 GMT  
		Size: 197.8 KB (197791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4006375c93489a865cdfc25c9e1e75ed965bfc170871e8d5a2a3f9cf0d8c7b`  
		Last Modified: Fri, 29 Jan 2021 02:34:05 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821f040d814bc1c1f2d6a5ec7c3612f16e1f59fbc45d96656eb07ae69916b90`  
		Last Modified: Fri, 29 Jan 2021 02:34:05 GMT  
		Size: 552.8 KB (552829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43869c366a4ebcde3a9b6d1e9ab88b0b479cc0185483c4efe5b94247dcc87fa`  
		Last Modified: Fri, 29 Jan 2021 02:34:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5f76e0a63305a007c47d4226119e70e3d52c9a3c714c7e42af9ed719b3c557`  
		Last Modified: Fri, 29 Jan 2021 02:34:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
