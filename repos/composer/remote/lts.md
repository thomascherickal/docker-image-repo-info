## `composer:lts`

```console
$ docker pull composer@sha256:6a9cdecabf541a0f0f14266c08ded27b6a71b6254aa3905f486a2d02e385e399
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

### `composer:lts` - linux; amd64

```console
$ docker pull composer@sha256:5b6d543d24cbd8fae75a9a6d36246dcf0615fa0385ec02cf2b6e957ef4b31a19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69613926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c04092b98ce559af103729fcd207aa1c16653c4b81afd3d494f88b9b12d4f2c8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:53:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 03:53:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 03:53:25 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 03:53:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 03:53:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 03:53:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:53:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:53:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 04:16:21 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 21 Oct 2023 04:38:47 GMT
ENV PHP_VERSION=8.2.11
# Sat, 21 Oct 2023 04:38:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 21 Oct 2023 04:38:47 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 21 Oct 2023 04:38:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 04:38:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:42:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 04:42:19 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:42:20 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 04:42:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 04:42:21 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb5622fa41e7d9451865eeadb9858807e2359c9787e86c9084078c65c7367f`  
		Last Modified: Sat, 21 Oct 2023 06:26:15 GMT  
		Size: 2.7 MB (2679351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587160738cca0d7e2afbad4e319bf69a2e5e51250de0bbb96546aa3a8754f814`  
		Last Modified: Sat, 21 Oct 2023 06:26:15 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802431d360de8be26d17059e07cf6636e5d549b0beeb9db464d3a916bc093afc`  
		Last Modified: Sat, 21 Oct 2023 06:26:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8961096385726bcbba5e9fd658ac4596258683ca052aaacb11d95f24ab58d2ca`  
		Last Modified: Sat, 21 Oct 2023 06:30:02 GMT  
		Size: 12.1 MB (12067120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9f7268d40c7067ea0325482f833b79b80406810e495327dd2e11bf0e5e219a`  
		Last Modified: Sat, 21 Oct 2023 06:30:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15008dbdc65323fcd63a17b89ff3e3dc960cbd51b15f7368616b0d5a55314a25`  
		Last Modified: Sat, 21 Oct 2023 06:30:04 GMT  
		Size: 17.1 MB (17143817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b74dc09bca3e52f58b05d5553aa4bb32b8a8608775ed42ba1a3b69d5f58f51d`  
		Last Modified: Sat, 21 Oct 2023 06:30:01 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b786d1ee988a0c1b7c3b540ba7876a5cdfb5cd81a468791b24249bcc36435be8`  
		Last Modified: Sat, 21 Oct 2023 06:30:01 GMT  
		Size: 19.0 KB (18990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c402779eea844ab94bd520234d501dbd3d70166b1ba416d5363c56ad50f38d`  
		Last Modified: Sat, 21 Oct 2023 07:23:45 GMT  
		Size: 32.5 MB (32534317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a704f43f1ad92da374a777c86f82514085c7f7c9a9449494e8d236de898a1a0b`  
		Last Modified: Sat, 21 Oct 2023 07:23:40 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0db18bd464fd29687db0ed138f5e4c6f1113328bbfa09c377a9a9ab80fd7de`  
		Last Modified: Sat, 21 Oct 2023 07:24:28 GMT  
		Size: 1.8 MB (1763084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d046c46edec94e63d80027a5bc89f953f01c97288ffaee09bd0226f9a8d1ea0`  
		Last Modified: Sat, 21 Oct 2023 07:24:27 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41125c5003f9c9cedf179d855c0c94bedacc596d2d16cc13d6c000490f822119`  
		Last Modified: Sat, 21 Oct 2023 07:24:27 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:lts` - linux; arm variant v6

```console
$ docker pull composer@sha256:872a411d6116a5d933ef5d8946f705471574610c814cfe2b8ca2dbcc7d4c756f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66735572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b72b66938e83dc4ba887483a645ae4c0e5c00ca2ef8fc86765c9faf5dc85fc9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:12:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:12:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:12:16 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:12:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:12:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:12:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:12:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:12:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:33:02 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 21 Oct 2023 01:53:37 GMT
ENV PHP_VERSION=8.2.11
# Sat, 21 Oct 2023 01:53:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 21 Oct 2023 01:53:37 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 21 Oct 2023 01:53:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 01:53:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:56:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 01:56:38 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:56:39 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 01:56:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 01:56:39 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e612e11521ddc11f4fbafd4815fd061e99bf827b9952ec407d3c976ea4237db`  
		Last Modified: Sat, 21 Oct 2023 03:21:10 GMT  
		Size: 2.7 MB (2685635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01946457dc0771f96a346d9812bad780b01a21b5e87a4574d8485c060782c4f1`  
		Last Modified: Sat, 21 Oct 2023 03:21:09 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db630a9f175c24d8d95bee24189d4d7e3c04d766b096001c7b8dd8cadb299ddd`  
		Last Modified: Sat, 21 Oct 2023 03:21:09 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bb17b0fab50a14145c60e214562f358c00e814d689c92a1f93844680235dad`  
		Last Modified: Sat, 21 Oct 2023 03:24:31 GMT  
		Size: 12.1 MB (12067129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d67ed6be53f8e939239765d11a28cf7d89e3c70a4f0701de0c5f1c3371a56e`  
		Last Modified: Sat, 21 Oct 2023 03:24:29 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540be66b203a52bab6cdc1565c3bf291d8ec8e559d9abbc6189060126a026c61`  
		Last Modified: Sat, 21 Oct 2023 03:24:33 GMT  
		Size: 15.7 MB (15732832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32635b86d4eaebcd5ee9da469b33771b01fd349f2c95fa9b7d99728151877f73`  
		Last Modified: Sat, 21 Oct 2023 03:24:29 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08cef1748f49fc956dae2286e59212a9ee899add1e7f4b9512805050197cbdd`  
		Last Modified: Sat, 21 Oct 2023 03:24:29 GMT  
		Size: 18.8 KB (18809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bf3c46655c4a7bc53c6e31ba92331a117792e98474554776b9c20cc9394d5d`  
		Last Modified: Sat, 21 Oct 2023 05:17:23 GMT  
		Size: 31.3 MB (31290650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1d64f0551be53e808509204d154d8c679aef24f792c019afbbbb0463bba98`  
		Last Modified: Sat, 21 Oct 2023 05:17:17 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ccdf3b157e12bfe6db4207410045d103e31f9c3f5d86548a7dda393d59c2f`  
		Last Modified: Sat, 21 Oct 2023 05:18:05 GMT  
		Size: 1.8 MB (1789948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a67e7894fc6264bfaf577e7a3c6c42fecd8373a4af03b540534c7da8c7a579f`  
		Last Modified: Sat, 21 Oct 2023 05:18:04 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f58665114b754bff70c9b844b9ed0f923a47976622dfb124cc190a37bc43c`  
		Last Modified: Sat, 21 Oct 2023 05:18:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:lts` - linux; arm variant v7

```console
$ docker pull composer@sha256:6914cd78d3ce899a13a7d23cd2bb3619da2ae022705eb48c8272f03b081cd96b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64673336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27ac0ea45925172d79a538fcdb8af0deca91f423f3c0b2c5569796a9c5d9cb3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:38:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:38:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:38:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:38:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:38:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:38:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:38:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:38:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:58:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 21 Oct 2023 02:17:31 GMT
ENV PHP_VERSION=8.2.11
# Sat, 21 Oct 2023 02:17:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 21 Oct 2023 02:17:32 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 21 Oct 2023 02:17:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 02:17:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 02:20:35 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:20:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 02:20:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 02:20:36 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b85771de82c52657e20dd48525d4f84f8acc9b0a8e038caa59270b86c697f2`  
		Last Modified: Sat, 21 Oct 2023 03:43:30 GMT  
		Size: 2.5 MB (2524719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9aac39d270b16e3d2ddb731400c6e7d7d75663871e887bcd23f5e8867d4f0b`  
		Last Modified: Sat, 21 Oct 2023 03:43:29 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6906580ddda7fb53704962fe74b174c72d2e1e8f33877ee579c290e1c2bb65a`  
		Last Modified: Sat, 21 Oct 2023 03:43:29 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04ddc113d6961290c875016834d9be402391183088242b6fdfa132a37967d25`  
		Last Modified: Sat, 21 Oct 2023 03:47:02 GMT  
		Size: 12.1 MB (12067125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b38cf41ff7b28b9207e34c43790423cb8e7642b5e600854bc903e155e5a71c`  
		Last Modified: Sat, 21 Oct 2023 03:47:01 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a413c5067a1acf94747d9785a23c8081d807390bc8ef0a72ba4da323c44aef92`  
		Last Modified: Sat, 21 Oct 2023 03:47:04 GMT  
		Size: 14.7 MB (14690749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff6691a9e78d1b0234a20ccc636fb5aafa7c4c2f560f1ecbf84eab01cc24cb9`  
		Last Modified: Sat, 21 Oct 2023 03:47:01 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf6f97c4061c331f01f1120db51652940fe0030a57db419297fdebe195aa2f`  
		Last Modified: Sat, 21 Oct 2023 03:47:01 GMT  
		Size: 18.8 KB (18817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc40bc4b3b84c37a8ff8884206f29afb04b897295c7eb79c6924e423039e612c`  
		Last Modified: Sat, 21 Oct 2023 05:14:10 GMT  
		Size: 30.8 MB (30789403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0f6650679c6c97eb394bfa51dfb45cd951160504e5a5612bc6aed10bce95a4`  
		Last Modified: Sat, 21 Oct 2023 05:14:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6b1e7dc373dd95dde13505dd319eb5ffc006ba47fb3ef3ec1cf6a241333be`  
		Last Modified: Sat, 21 Oct 2023 05:14:50 GMT  
		Size: 1.7 MB (1677335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ca5807d13fe753662e9515e779f71352ed0228cf2234ffe88957bc9d41b7c`  
		Last Modified: Sat, 21 Oct 2023 05:14:50 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaa3384d904d41813977b7d05b7b8a747a9c15cbc6049aa3f47416ea6f96481`  
		Last Modified: Sat, 21 Oct 2023 05:14:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:lts` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:b8e937750a15def6f41610efdfb72acd0875fbbe6446b8951a22c37fd7c2d437
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69944759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23099a5dd15b922ad715dab8ed8995763ccd77c7262ed57128aa20733db82554`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:18:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 03:18:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 03:18:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 03:18:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 03:42:09 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 21 Oct 2023 04:04:14 GMT
ENV PHP_VERSION=8.2.11
# Sat, 21 Oct 2023 04:04:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 21 Oct 2023 04:04:14 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 21 Oct 2023 04:04:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 04:04:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:07:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 04:07:42 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:07:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 04:07:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 04:07:43 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586ad9c0520cf94b10cf643fcc476c76d317d9f7fb19ea6664adc39853495259`  
		Last Modified: Sat, 21 Oct 2023 05:46:23 GMT  
		Size: 2.7 MB (2717014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ca4079608bb17975de556b78088351825e86efc0dd9d7e94be500e7aff4c4e`  
		Last Modified: Sat, 21 Oct 2023 05:46:22 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d96350d9b73c214fd82e72b434fb80879d73a1387ad9f7c654a25c99f169907`  
		Last Modified: Sat, 21 Oct 2023 05:46:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29425996241a636123c283b38486abb392708121a49c84dbec451fa4b5257734`  
		Last Modified: Sat, 21 Oct 2023 05:49:44 GMT  
		Size: 12.1 MB (12067112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4cf5ee33f22bb029e52c660ce33ecb2d69e0d3bf19bbed6d589971834ee01b`  
		Last Modified: Sat, 21 Oct 2023 05:49:43 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0730fcc521050d6451393e0b273fba746f585da0bed79feb2958bd56f2a3dd`  
		Last Modified: Sat, 21 Oct 2023 05:49:45 GMT  
		Size: 17.1 MB (17140256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ab598343bb707400fbb1f0fc2507d781c6b47de7d3a307e962881f62ca6946`  
		Last Modified: Sat, 21 Oct 2023 05:49:43 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a21f7bc3d17c5271ddf3f15fd7dff63889044a958826ec2cefbe9a16eafbd4`  
		Last Modified: Sat, 21 Oct 2023 05:49:43 GMT  
		Size: 18.8 KB (18772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9295b05fd2e2e60ec5fa5534deb6a6c7c42ed46df6bcaf8ab5e8ddeaafb5e7ac`  
		Last Modified: Sat, 21 Oct 2023 07:57:32 GMT  
		Size: 32.9 MB (32888749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435e57bfecc25a912dc20deb39f2c5ff0c37bdf74ec34f3e5a1c6520d15f8cc5`  
		Last Modified: Sat, 21 Oct 2023 07:57:28 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2b21ff636729d947ddffb9852babc2e3971c76352f50acaaf15843cd45d013`  
		Last Modified: Sat, 21 Oct 2023 07:58:14 GMT  
		Size: 1.8 MB (1775744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99125cda8f9e9782e50bede17cd8ba4f17e7e4aecbdf14fd2c4e64b0bcc9621d`  
		Last Modified: Sat, 21 Oct 2023 07:58:13 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415cc6a8e266601f4026e053855574ebfabc6ecb60790b0703be2b180696ff52`  
		Last Modified: Sat, 21 Oct 2023 07:58:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:lts` - linux; 386

```console
$ docker pull composer@sha256:d60d9ec83bab8c52d219e39f6313db93733ea061480ddba9af49b127b7cec4f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46949226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820f9459bc91978e394a42efa46f97c70e3c146ca89107dbff62109211025dd8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:37:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Sep 2023 03:37:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Sep 2023 03:37:48 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Sep 2023 03:37:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Sep 2023 03:37:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 29 Sep 2023 03:37:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 03:37:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 03:37:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Sep 2023 03:57:58 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:50:03 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:50:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:50:03 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:50:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 02:50:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:56:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:56:06 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:56:07 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:56:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:56:07 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a258209926de3d48ed5c8f4ac2b7e261db17a744aae52199857c08261239f51`  
		Last Modified: Fri, 29 Sep 2023 05:20:06 GMT  
		Size: 2.7 MB (2722585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba348a66995f0cef9bcda7f54b35f0d2a39cb8496642c433c687ffc77481bfb2`  
		Last Modified: Fri, 29 Sep 2023 05:20:05 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff34a7b5931f6b1ab2060c56ff97fdc936fadc8099374176a375a16c36555d5`  
		Last Modified: Fri, 29 Sep 2023 05:20:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba3b671b61a1aa55df679863313df77eb7ce03d92637f02c629c44c3c092f1`  
		Last Modified: Sat, 30 Sep 2023 05:25:35 GMT  
		Size: 12.1 MB (12067124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7995e5c4d2bc705da9f966ddaa73a253ed4614670486770d0acd0e77f0668c76`  
		Last Modified: Sat, 30 Sep 2023 05:25:34 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc348c0d9e28dc327cefb1c299ae3764d7c1f660d6ef3511d59bdc8008f2541`  
		Last Modified: Sat, 30 Sep 2023 05:25:39 GMT  
		Size: 17.0 MB (17032488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9efebc29ccdbd291fc62e24e7dfc425df21de3d49c318566c9d4ada4e4b3b`  
		Last Modified: Sat, 30 Sep 2023 05:25:33 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce29cb1cbfa604a0844c8831b5d926e4ab6462b9a7eb209014952b9c38a9cb4`  
		Last Modified: Sat, 30 Sep 2023 05:25:34 GMT  
		Size: 18.9 KB (18928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb9ef068f2e72a341d0d00bca246d0de1848c2924ad1dcd10019872104c9dc2`  
		Last Modified: Sat, 30 Sep 2023 09:16:33 GMT  
		Size: 10.7 MB (10733242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0648a4b886020dcc12863fcb2cb9d29e33f9d6ce187880545170c80516df0d16`  
		Last Modified: Sat, 30 Sep 2023 09:16:31 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b398b9e2a93f896362edd66508f0a29a4d9b22229d88e61ab8b46e6e80607d5d`  
		Last Modified: Sat, 30 Sep 2023 09:17:14 GMT  
		Size: 1.1 MB (1133818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d041bb2079e70d77729a7caacee361535e694f9290c74beb1a8580016adc4b0`  
		Last Modified: Sat, 30 Sep 2023 09:17:14 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3df5b03891c9431b10e759b71e0ba9a2141e9bd93904257b5ec946a13cb4e5`  
		Last Modified: Sat, 30 Sep 2023 09:17:14 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:lts` - linux; ppc64le

```console
$ docker pull composer@sha256:f2b96ac04d860a32802814d89ee8b154c2e6bb7ac932b6f52953a67ee7a9a0bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71520195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939096343f1a487ff7dfd785a80b492a00a0aaa0be8a330855c0a96b6132f09e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:19:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:19:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:19:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:19:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:19:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:19:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:19:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:19:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:36:24 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 21 Oct 2023 01:52:37 GMT
ENV PHP_VERSION=8.2.11
# Sat, 21 Oct 2023 01:52:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 21 Oct 2023 01:52:38 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 21 Oct 2023 01:52:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 01:52:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:55:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 01:55:12 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:55:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 01:55:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 01:55:14 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad27196e84bb3ade565a8dd1e6b1058530043ed6f23f3c2b27e177dd9a872c0f`  
		Last Modified: Sat, 21 Oct 2023 03:15:11 GMT  
		Size: 2.8 MB (2766404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8623e62ddef0a09dade21407c25a1ed872a84bcb0af9cdf932e97f5221e530`  
		Last Modified: Sat, 21 Oct 2023 03:15:10 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763cf47f2cf8995a5d2a492fab64e7743a5d1b7d942d379bdec3a3dc8130ed53`  
		Last Modified: Sat, 21 Oct 2023 03:15:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b1667fcc5126a631720aaa4a7d027b6afd7ca762b301d2f4594934507b8355`  
		Last Modified: Sat, 21 Oct 2023 03:19:02 GMT  
		Size: 12.1 MB (12067110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936405425141c91d0eb418bab07ca6f7d71262c2c46282335c86e6e11379765a`  
		Last Modified: Sat, 21 Oct 2023 03:19:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdad97d83922529edd3b9aa8463bf6d6fc615f98ac8560b39c0148eb204a1f7`  
		Last Modified: Sat, 21 Oct 2023 03:19:04 GMT  
		Size: 17.9 MB (17921292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128291508f12becfaa289c0c95c24a842c4d628befa12220736ea1e44b2f69f`  
		Last Modified: Sat, 21 Oct 2023 03:19:01 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7252b788fa004336deac2bb09c884e08b752f9b8053ac2ecde60a2e18269bde6`  
		Last Modified: Sat, 21 Oct 2023 03:19:01 GMT  
		Size: 18.8 KB (18786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00917ab010412b70bfee71df7d28a02a5edfd707440f92c9d94f7804d6d6ee09`  
		Last Modified: Sat, 21 Oct 2023 04:14:45 GMT  
		Size: 33.5 MB (33538345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1d4c9ad13a538b86d2fe29136df2e68420d8ab4af11fb2832a2b9f94fc5a8f`  
		Last Modified: Sat, 21 Oct 2023 04:14:40 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf63117b19b90bdee1f98ee6490f9e8103fb924d92d991cc7c18ce54dedd0e4`  
		Last Modified: Sat, 21 Oct 2023 04:15:30 GMT  
		Size: 1.9 MB (1856466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ee399923a4908682f49a94fb2c67d2e22367d0cb5edbf7115d69f06801a6de`  
		Last Modified: Sat, 21 Oct 2023 04:15:30 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc5c67b46ee06a61f26e20b25c4138e635e1b2b9f31e39b830c636335b10b2e`  
		Last Modified: Sat, 21 Oct 2023 04:15:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:lts` - linux; s390x

```console
$ docker pull composer@sha256:835071818920035ce6ba1bdcf940671836a7bd47bc15cebf4efcf239ea65b16d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68240246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aac6202e3bdb3fb8174f9da9eedf25efc5c2856cb605744f020e0756b4417c5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:18:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:18:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:18:39 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:18:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:18:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:18:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:18:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:18:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:37:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 21 Oct 2023 01:55:51 GMT
ENV PHP_VERSION=8.2.11
# Sat, 21 Oct 2023 01:55:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 21 Oct 2023 01:55:52 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 21 Oct 2023 01:55:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 01:55:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:58:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 01:58:35 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:58:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 01:58:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 01:58:37 GMT
CMD ["php" "-a"]
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     openssh-client     patch     subversion     tini     unzip     zip     $([ "$(apk --print-arch)" != "x86" ] && echo mercurial)     $([ "$(apk --print-arch)" != "armhf" ] && echo p7zip) # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 29 Sep 2023 13:59:34 GMT
ENV COMPOSER_VERSION=2.2.22
# Fri, 29 Sep 2023 13:59:34 GMT
RUN set -eux ;   curl     --silent     --fail     --location     --retry 3     --output /usr/local/bin/install-php-extensions     --url https://github.com/mlocati/docker-php-extension-installer/releases/download/1.2.58/install-php-extensions   ;   echo 182011b3dca5544a70fdeb587af44ed1760aa9a2ed37d787d0f280a99f92b008e638c37762360cd85583830a097665547849cb2293c4a0ee32c2a36ef7a349e2 /usr/local/bin/install-php-extensions | sha512sum --strict --check ;   chmod +x /usr/local/bin/install-php-extensions ;   install-php-extensions     bz2     zip   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   echo 572b963c4b7512a7de3c71a788772440b1996d918b1d2b5354bf8ba2bb057fadec6f7ac4852f2f8a8c01ab94c18141ce0422aec3619354b057216e0597db5ac2 /tmp/keys.dev.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   echo 47f374b8840dcb0aa7b2327f13d24ab5f6ae9e58aa630af0d62b3d0ea114f4a315c5d97b21dcad3c7ffe2f0a95db2edec267adaba3f4f5a262abebe39aed3a28 /tmp/keys.tags.pub | sha512sum --strict --check ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/f24b8f860b95b52167f91bbd3e3a7bcafe043038/web/installer   ;   echo 3137ad86bd990524ba1dedc2038309dfa6b63790d3ca52c28afea65dcc2eaead16fb33e9a72fd2a7a8240afaf26e065939a2d472f3b0eeaa575d1e8648f9bf19 /tmp/installer.php | sha512sum --strict --check ;   php /tmp/installer.php     --no-ansi     --install-dir=/usr/bin     --filename=composer     --version=${COMPOSER_VERSION}   ;   composer --ansi --version --no-interaction ;   composer diagnose ;   rm -f /tmp/installer.php ;   find /tmp -type d -exec chmod -v 1777 {} + # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
COPY docker-entrypoint.sh /docker-entrypoint.sh # buildkit
# Fri, 29 Sep 2023 13:59:34 GMT
WORKDIR /app
# Fri, 29 Sep 2023 13:59:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 29 Sep 2023 13:59:34 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcde857c8cbd1e2f9e4b3bdb1e05a51819df45223c3af3c89c357d02c0683abd`  
		Last Modified: Sat, 21 Oct 2023 03:23:07 GMT  
		Size: 2.8 MB (2789639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa1b5985d90d234d5b51288c0ce33de4d2a3f6d3634cd2e6818e9e9a36e8f2`  
		Last Modified: Sat, 21 Oct 2023 03:23:06 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a26837a8dae33541022d07fbeb175eb6f280a63fe5c2f5b6fdd82525674502`  
		Last Modified: Sat, 21 Oct 2023 03:23:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a04da66f7d093d661dfbe1313efcb006ee96e841e6a195b2edf223ca08cfc0`  
		Last Modified: Sat, 21 Oct 2023 03:26:08 GMT  
		Size: 12.1 MB (12067116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ebb537b15240ef5af2f91d31e130247e7fe95e07773b3c53c610b1dc171cff`  
		Last Modified: Sat, 21 Oct 2023 03:26:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14ca85185bf8ac6e6bd59f7db6d42d314278b9d63655d14d066bc62f3aca767`  
		Last Modified: Sat, 21 Oct 2023 03:26:09 GMT  
		Size: 16.0 MB (16044081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecace547c5191fd4202a584a8808a0377fabe626438715de7aabbbdb49add926`  
		Last Modified: Sat, 21 Oct 2023 03:26:07 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e31d9dfe21cf9efbf967397903fdd2157e87a511cabf3f21d64fd89f0e680`  
		Last Modified: Sat, 21 Oct 2023 03:26:07 GMT  
		Size: 18.8 KB (18813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a51b5690e3b6817d8107708b37b0e2e38c015673a8d356641401596767e9e`  
		Last Modified: Sat, 21 Oct 2023 04:45:39 GMT  
		Size: 32.3 MB (32334061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b49e40a44a2d5a4a0866d759fca4d44b7161eff08554429aeab1b1e8ffe2080`  
		Last Modified: Sat, 21 Oct 2023 04:45:35 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189cdd1ca430a8ab37e2945fb0585f4a47f75c473ca55e14bfdb39015a04b4f0`  
		Last Modified: Sat, 21 Oct 2023 04:46:08 GMT  
		Size: 1.8 MB (1766143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5389b8dfae60c65cf68df13b6173b03cb062096abde8058837122d0bc8eec567`  
		Last Modified: Sat, 21 Oct 2023 04:46:08 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa98bebe6ec99bd4634404f34356c25416227659539f795f6de922b9f836056`  
		Last Modified: Sat, 21 Oct 2023 04:46:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
