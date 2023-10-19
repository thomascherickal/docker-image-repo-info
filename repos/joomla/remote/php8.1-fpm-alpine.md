## `joomla:php8.1-fpm-alpine`

```console
$ docker pull joomla@sha256:008b8b61820ffddea96a3d39ab4fde04688c6a61dd2b4cccbc97904fcd1193f9
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

### `joomla:php8.1-fpm-alpine` - linux; amd64

```console
$ docker pull joomla@sha256:245922b0012dbb5fc0766a4b36584639d12844bce82bb592fbbb5e36675a6b25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107823467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f3e7c14c7267fa459e8a5f36eff10ffea6232d105e0158c4160cf7729e50e62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:44:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Sep 2023 01:44:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Sep 2023 01:44:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Sep 2023 01:44:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Sep 2023 01:44:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 29 Sep 2023 01:44:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 01:44:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 01:44:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Sep 2023 02:19:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 03:35:52 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 03:35:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 03:35:52 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 03:35:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 03:35:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:43:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 03:43:18 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:43:20 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 03:43:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 03:43:20 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 03:43:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 03:43:20 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 03:43:20 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 03:43:20 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 00:44:46 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 00:44:46 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 01:00:29 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 01:02:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 01:02:24 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 01:02:25 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 01:02:25 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:02:25 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:02:25 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:02:32 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:02:32 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:02:33 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:02:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:02:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b4f1479ad806ba5bd07a2965885c4c0745bc13d6d510139599bfe1bc250114`  
		Last Modified: Fri, 29 Sep 2023 02:46:40 GMT  
		Size: 2.7 MB (2679012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266ff8d3cec50cc8053fc2f8c7323e48be9fc3dcdfcc300841604b4c1f76f3f`  
		Last Modified: Fri, 29 Sep 2023 02:46:40 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6127d1435a8cdc1a5d1f825706c4ad94da38108418d1638aaccfb9149fdb98a6`  
		Last Modified: Fri, 29 Sep 2023 02:46:40 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921d0e01a4d1f2a933749864d2c96c245f6596602a3aad00e4411cc6d89c04bb`  
		Last Modified: Sat, 30 Sep 2023 04:26:19 GMT  
		Size: 11.8 MB (11814632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d569c79bd14bed07d204f9d653a0efdf11c475b695bc84b278100c85df43f01`  
		Last Modified: Sat, 30 Sep 2023 04:26:18 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f840aa56e95076bb21454b9930d0a954aed997f5f8648232c73e16262c37432`  
		Last Modified: Sat, 30 Sep 2023 04:26:46 GMT  
		Size: 12.4 MB (12423796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecc75dab1caae833df9bb57e46453a624593e04feccc8fe609f23a8ef73ea9`  
		Last Modified: Sat, 30 Sep 2023 04:26:43 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49494614ee3f5d5c8cec55c5f780405be95b04ad08b9fec6073a454110611c17`  
		Last Modified: Sat, 30 Sep 2023 04:26:43 GMT  
		Size: 18.9 KB (18936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbca34bfe575553085f0849c61d7bbdb3fdbac37bd87696359087658970e18f`  
		Last Modified: Sat, 30 Sep 2023 04:26:43 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96449961f3c6728ab371be44f40873810e943404776703203057ed8009105c0a`  
		Last Modified: Thu, 19 Oct 2023 01:18:10 GMT  
		Size: 45.2 MB (45184644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64e9dce000a9acf8a125631edb4bb07ee7d6b8091f927e27c61914791261374`  
		Last Modified: Thu, 19 Oct 2023 01:18:05 GMT  
		Size: 6.9 MB (6939389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de9f061f291a0363c9d456a5200ce505370500f1f15d76f8d77ef4d0af3991d`  
		Last Modified: Thu, 19 Oct 2023 01:18:02 GMT  
		Size: 67.9 KB (67881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200cc30e4c5f4c7765e3c28259cb5dcb1a260f9d5f0504c34dc35ec26a58e992`  
		Last Modified: Thu, 19 Oct 2023 01:18:02 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f011689898d19fd09a77c0b53d26be42d51071924827765a484265e850457e`  
		Last Modified: Thu, 19 Oct 2023 01:18:06 GMT  
		Size: 25.3 MB (25275788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2c5a3321490bfc1adca3d7f51a18328298d3f0b8c3ac64fbe45d7b5e87acf7`  
		Last Modified: Thu, 19 Oct 2023 01:18:02 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124dcb66fd90bc73a2e8ae69c9a68a8a975d0c27b51602ec6330d6c27f6673f6`  
		Last Modified: Thu, 19 Oct 2023 01:18:02 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull joomla@sha256:4e9d2d57e4641177196ece29d42b2379ca2c925973ce9bc742a4a152da6f1a48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101970033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f29af33b0b3d32d48f83bcb50e7c1e1ca60d3d45539189bedee1bad05dbdc05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:37:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 28 Sep 2023 23:37:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 28 Sep 2023 23:37:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 28 Sep 2023 23:37:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 28 Sep 2023 23:37:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 28 Sep 2023 23:37:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 28 Sep 2023 23:37:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 28 Sep 2023 23:37:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Sep 2023 00:24:59 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 01:50:36 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 01:50:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 01:50:36 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 01:50:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 01:50:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 01:59:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 01:59:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 01:59:52 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 01:59:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 01:59:53 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 01:59:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 01:59:54 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 01:59:54 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 01:59:54 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 01:19:06 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 01:19:06 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 01:28:05 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 01:30:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 01:30:06 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 01:30:07 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 01:30:07 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:30:07 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:30:07 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:30:15 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:30:16 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:30:16 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:30:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:30:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdb445630a596725c44056b7df28bb58573467c9bd7bb0953fae11402694132`  
		Last Modified: Fri, 29 Sep 2023 00:45:35 GMT  
		Size: 2.7 MB (2685352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d65017109cc5cd94257a019481ecf2c7a4ebed8774de3f27d530aa46ef5dd3`  
		Last Modified: Fri, 29 Sep 2023 00:45:33 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bd556e64b693cc6fa0bb044a3f5a890082838221f316d616228859b739bc02`  
		Last Modified: Fri, 29 Sep 2023 00:45:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5be35e06e016d28b0cccea36009267f4f63de2d11a7b8981329c15637f4f7a`  
		Last Modified: Sat, 30 Sep 2023 02:38:19 GMT  
		Size: 11.8 MB (11814631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c934e16fc78607f03d4c3e1a77bc923a984a9db057ca1d5d396a05d0fb559b38`  
		Last Modified: Sat, 30 Sep 2023 02:38:18 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664bbe29cff084c5c51cad511119fd5ac28468d32c13908fddac68b976c87e0`  
		Last Modified: Sat, 30 Sep 2023 02:38:47 GMT  
		Size: 11.3 MB (11320685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca408cb3592945d1a740f9eeb97dd2a6af0a2f10f68a7f57c9a4c2846b98734b`  
		Last Modified: Sat, 30 Sep 2023 02:38:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593c8daab59c614a628e7c4023a530ba9cf76fd8eec96b80e3a1a3ba7661466c`  
		Last Modified: Sat, 30 Sep 2023 02:38:45 GMT  
		Size: 18.8 KB (18758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142c6c71999cd38edc06ad05b6f59bf5f19682bb7576d521569adfa6dbfa2925`  
		Last Modified: Sat, 30 Sep 2023 02:38:45 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625ffa2e32f70183b2d7fcdf15d020b77e92e2b24672033e2a7e28c431b0f44c`  
		Last Modified: Thu, 19 Oct 2023 01:38:00 GMT  
		Size: 41.0 MB (40993911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcb7e4ebd8ea5593f0e19f063ed84d87df00ac60c2f77f5d6064afd31e533e5`  
		Last Modified: Thu, 19 Oct 2023 01:37:54 GMT  
		Size: 6.6 MB (6630313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9732d64d1aedd4f71c625190185fa5e2c4dd08e650ad4a8f7a2424489eb02c`  
		Last Modified: Thu, 19 Oct 2023 01:37:51 GMT  
		Size: 67.9 KB (67877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d9d9f2952c20f79b1c57fced292971a68581812ea3b8014791ee98996e659a`  
		Last Modified: Thu, 19 Oct 2023 01:37:51 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baa6facb25927319e6a909e00301b19c7406cf082e30eef495c4100705ff149`  
		Last Modified: Thu, 19 Oct 2023 01:37:56 GMT  
		Size: 25.3 MB (25275794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f154c92f18a13cecafea1e51077013fe308739fa6b1d6a57feb7a783378e048`  
		Last Modified: Thu, 19 Oct 2023 01:37:51 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1ef52939601f07b58e8d0fc279d051b78603de23e52b94ca0e2f8ee149256d`  
		Last Modified: Thu, 19 Oct 2023 01:37:51 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull joomla@sha256:1dca52e6069b89c0858c67c6aebec7b2441cd5a66351204de007e0f74628fdf1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.6 MB (98596191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbba60f58ef640d03ee74d1a2b3158c4b7a289c4c5cc4e9ee5e915d2a0664773`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:05:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Sep 2023 01:05:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Sep 2023 01:05:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Sep 2023 01:05:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Sep 2023 01:05:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 29 Sep 2023 01:05:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 01:05:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 01:05:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Sep 2023 01:33:20 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 03:43:03 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 03:43:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 03:43:03 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 03:43:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 03:43:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:48:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 03:48:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:48:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 03:48:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 03:48:54 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 03:48:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 03:48:55 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 03:48:55 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 03:48:55 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 01:42:24 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 01:42:25 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 02:01:17 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 02:03:18 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 02:03:19 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 02:03:20 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 02:03:21 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 02:03:21 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 02:03:21 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 02:03:29 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 02:03:30 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 02:03:30 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 02:03:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 02:03:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec8fbd0dd9c9c11ed8693376186e2b7987ef5f62bd9185f45381065e28df439`  
		Last Modified: Fri, 29 Sep 2023 01:55:49 GMT  
		Size: 2.5 MB (2523034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becee47afe4610a18d76eab064a617346194347ccf56e8fdfdb95d16ed46637e`  
		Last Modified: Fri, 29 Sep 2023 01:55:49 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df313409622ad242bb3fbe3b00fb57355a570dacdd347d6341e75735ea564114`  
		Last Modified: Fri, 29 Sep 2023 01:55:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ba52b29eba5021fd8c8c5ffa98f646cd1d1002023d845f4dc6bc2bae388f8d`  
		Last Modified: Sat, 30 Sep 2023 04:26:12 GMT  
		Size: 11.8 MB (11814635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50690d1c4f0896548eb6b21ccf2f54a72eb76d7523aaf2c4c92f7f6ee23845d`  
		Last Modified: Sat, 30 Sep 2023 04:26:11 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cbaaa00aa558c457fa22c1f9f3a4cfc5090b380f40860d9465e44f06883f2f`  
		Last Modified: Sat, 30 Sep 2023 04:26:39 GMT  
		Size: 10.6 MB (10587313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10514c984f3008d3a7b391d8a3da3d225c4a753ff4cb1eb1965f2301c201b8f5`  
		Last Modified: Sat, 30 Sep 2023 04:26:36 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580f3c47c624b0e913fb87726b70f30c550cc404c62319f02f4b2390ebca6ef`  
		Last Modified: Sat, 30 Sep 2023 04:26:36 GMT  
		Size: 18.8 KB (18761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58517866cb1a94c3309d8b89d38c6837ac1bc5a640883e4b86d28a9b9176da30`  
		Last Modified: Sat, 30 Sep 2023 04:26:36 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e0d4ec253096780aa40c93516569eba88a1a7fbb9a95671e5bdb5849255cc`  
		Last Modified: Thu, 19 Oct 2023 02:15:58 GMT  
		Size: 38.8 MB (38800124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3a423233aa103114acbc7e2c3a4b585494420565d4bec768eb4957396af996`  
		Last Modified: Thu, 19 Oct 2023 02:15:51 GMT  
		Size: 6.6 MB (6591309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cec6345e1993b7e33d7abc8e1300fc9889cf3e6455c24cc9704d1502b7dfb4a`  
		Last Modified: Thu, 19 Oct 2023 02:15:48 GMT  
		Size: 67.9 KB (67894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21e05b5b06421a57e3fa92da672ee7e3bbe47a74c1e575760a361425d06e53c`  
		Last Modified: Thu, 19 Oct 2023 02:15:47 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5c2ab80233670c872bcaea96976f4363f489095b88f135ec860f21da98116f`  
		Last Modified: Thu, 19 Oct 2023 02:15:55 GMT  
		Size: 25.3 MB (25275789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088e1e333fe91732e5f7195eb2e5ea4da360a1b7bb78a1720731633e95352f18`  
		Last Modified: Thu, 19 Oct 2023 02:15:49 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f0c3e6ddd7dc156e45bcce90c00b18b71ba0c4b4283013e863da3ecbca60fa`  
		Last Modified: Thu, 19 Oct 2023 02:15:48 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:081b1da431d99d09a34d33791e4722ec8659ae086fc2812bdae18a6a8cf92029
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107071920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9942a41e0b6af6b2d5b1fcaa68e6871c32c416ad7d28bcf5d0f445c40063a940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:49:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 28 Sep 2023 22:49:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 28 Sep 2023 22:49:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 28 Sep 2023 22:49:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 28 Sep 2023 22:49:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 28 Sep 2023 22:49:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 28 Sep 2023 22:49:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 28 Sep 2023 22:49:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 28 Sep 2023 23:23:58 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 03:00:55 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 03:00:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 03:00:55 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 03:01:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 03:01:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:08:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 03:08:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:08:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 03:08:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 03:08:17 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 03:08:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 03:08:18 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 03:08:18 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 03:08:18 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 01:30:07 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 01:30:07 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 01:43:51 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 01:45:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 01:45:31 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 01:45:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 01:45:31 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:45:31 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:45:31 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:45:36 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:45:37 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:45:37 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:45:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:45:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffca02528f4505c4ba6a7c83f36f65ee3f033abaac3b6fce5fa08004e39559f1`  
		Last Modified: Thu, 28 Sep 2023 23:50:07 GMT  
		Size: 2.7 MB (2715606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6cc431b70282041669618b2c2d5327950e9bc8313767d501caa5f6447a90cf`  
		Last Modified: Thu, 28 Sep 2023 23:50:06 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55997933f10db11319c8c483d3c329f5cab59b36da94068425a5b8cb0691a66d`  
		Last Modified: Thu, 28 Sep 2023 23:50:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226da9d0ba463289656e622ee5d4908c469a3194d1008aa016641c4e37ba4853`  
		Last Modified: Sat, 30 Sep 2023 03:50:25 GMT  
		Size: 11.8 MB (11814625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc34e05ec2cd1c6b7788012433b3a382f7c1181fcfe11b6813cc09e5d2e46d`  
		Last Modified: Sat, 30 Sep 2023 03:50:24 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14555cd11b8250b86e41ddcef200a5c5f8d67adc04e32ffcc2212d9fa753d149`  
		Last Modified: Sat, 30 Sep 2023 03:50:50 GMT  
		Size: 12.5 MB (12489522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88081437975f48dfd34650d992211afd78d1797cf365b4c1952866433e0e6efc`  
		Last Modified: Sat, 30 Sep 2023 03:50:48 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45fe6a35df4c69a459197255b6039e755ff8a6d4fb7514ac82b1727013a586b`  
		Last Modified: Sat, 30 Sep 2023 03:50:48 GMT  
		Size: 18.7 KB (18718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f005d420cbe654700d5f0fbc3073080ad1039b9771b7f2aa024624c8e2fb468d`  
		Last Modified: Sat, 30 Sep 2023 03:50:48 GMT  
		Size: 8.9 KB (8875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7637ac2fe1a8395cf45832d27a34de06fea1874f0e7fe859cc3b4aaeda1c067`  
		Last Modified: Thu, 19 Oct 2023 01:56:39 GMT  
		Size: 44.4 MB (44386472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa715bc907cf3bc08e1cf43fec5174c58511bb6a6d87eb29ef38b1bff7ef50d6`  
		Last Modified: Thu, 19 Oct 2023 01:56:36 GMT  
		Size: 7.0 MB (6954116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40eb9dd96f79370e06438ca669031a8ace28a7d3ea491a812280fcf182c76330`  
		Last Modified: Thu, 19 Oct 2023 01:56:33 GMT  
		Size: 67.8 KB (67824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b919909c2c6e3e09a53ab5c491a2d9a64ba38ce9b48c8fa97fed88b8b98c1`  
		Last Modified: Thu, 19 Oct 2023 01:56:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a9cc505d629087fdfc3b3f9adc1b79c5f19f94694b894dfe8aeb21140cd1e17`  
		Last Modified: Thu, 19 Oct 2023 01:56:36 GMT  
		Size: 25.3 MB (25275789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab08d0a81b51ed9efe6fb60e58cc32df7de9eab53fdd472257de0873c21e116f`  
		Last Modified: Thu, 19 Oct 2023 01:56:32 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59fffb4f5a3b17bbd86ccdf081592a585a5b9604c1dc245d6941aa39c3426ce`  
		Last Modified: Thu, 19 Oct 2023 01:56:33 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.1-fpm-alpine` - linux; 386

```console
$ docker pull joomla@sha256:aab2305b31cbb90f02a22b7ee107b8cbf0f40d2237ccb492f5a49f85f45cf9ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104756307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad341e823495421b9cf7c95d601dc2d26c26a58aa68637434542dd66c753512`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Sep 2023 04:37:08 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 04:13:43 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 04:13:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 04:13:43 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 04:13:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 04:13:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:26:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 04:26:06 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:26:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 04:26:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 04:26:08 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 04:26:08 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 04:26:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 04:26:09 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 04:26:09 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 01:03:56 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 01:03:56 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 01:25:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 01:28:11 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 01:28:12 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 01:28:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 01:28:13 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:28:13 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:28:13 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:28:22 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:28:23 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:28:23 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:28:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:28:24 GMT
CMD ["php-fpm"]
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
	-	`sha256:e89001e2f4e8e22a554e887e01e9b2db0f7b706c171621bd8b695a1ca8371ee5`  
		Last Modified: Sat, 30 Sep 2023 05:30:48 GMT  
		Size: 11.8 MB (11814628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e4cdc97da0eb1aa2c08083619ae2004ace4c3285d0daa113dd15220bb768ae`  
		Last Modified: Sat, 30 Sep 2023 05:30:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22e61343b89d81dfaf337ba7c4d5e9f5ddc0a5110d977fe39df7b75492d073b`  
		Last Modified: Sat, 30 Sep 2023 05:31:17 GMT  
		Size: 12.6 MB (12608107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ff6a52bf4cf8fbc7ee12147387cee5d71c0dbede1472383a0b4e5c66625367`  
		Last Modified: Sat, 30 Sep 2023 05:31:13 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa130458057ce5d1e697ee69c983e3fb25ea581a58b47b883b7915c825a52e97`  
		Last Modified: Sat, 30 Sep 2023 05:31:13 GMT  
		Size: 18.9 KB (18930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ca7557b4c3c30460908f128d365c4efb8f558902ae631e7628f5b432c6ac9f`  
		Last Modified: Sat, 30 Sep 2023 05:31:13 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bddb7817421e067235317f2e237b20a754a6b2915a87eca35364828c953ff9d`  
		Last Modified: Thu, 19 Oct 2023 01:43:16 GMT  
		Size: 42.0 MB (41956986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a33c22b6a34f4f12b67069c2aa0b63346e035b9dca10172e2d37af92831a19`  
		Last Modified: Thu, 19 Oct 2023 01:43:07 GMT  
		Size: 7.0 MB (7038242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7378cb959a9854d6dead899ea2785a915a39643cb50852e0573418d1ab1c0c2`  
		Last Modified: Thu, 19 Oct 2023 01:43:03 GMT  
		Size: 67.9 KB (67861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018f338acccb2285d0c02670f1028ec21ad1f00580df7cc69bd4c734dc279be5`  
		Last Modified: Thu, 19 Oct 2023 01:43:03 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cb6b7032e081197bfbfdfdc6440a0c712e546901115d10ffe5453f54e50b29`  
		Last Modified: Thu, 19 Oct 2023 01:43:11 GMT  
		Size: 25.3 MB (25275784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284c2f497862696d5a89d710075898777cdda1578acd6cd7578365fe52ae5b8d`  
		Last Modified: Thu, 19 Oct 2023 01:43:03 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd70c096190b6bfb4cd8365dc81739419a71aadd0f169ac60f8918d03c7f61ce`  
		Last Modified: Thu, 19 Oct 2023 01:43:03 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.1-fpm-alpine` - linux; ppc64le

```console
$ docker pull joomla@sha256:6b160298c4349b70536659a8d65d679e798c7fe44863b224c7ac812674183c60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113413913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08cd5acfa872a58328abf9b1f8897168eb044f176d2ed3c3bfcdf4b2cd3819b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:39:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 28 Sep 2023 23:39:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 28 Sep 2023 23:39:10 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 28 Sep 2023 23:39:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 28 Sep 2023 23:39:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 28 Sep 2023 23:39:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 28 Sep 2023 23:39:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 28 Sep 2023 23:39:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Sep 2023 00:20:21 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 04:32:37 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 04:32:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 04:32:37 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 04:32:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 04:32:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:40:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 04:40:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:40:58 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 04:40:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 04:40:59 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 04:41:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 04:41:02 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 04:41:03 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 04:41:04 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 00:26:02 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 00:26:03 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 00:54:04 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 00:56:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 00:56:29 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 00:56:30 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 00:56:31 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 00:56:31 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 00:56:31 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 00:56:41 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 00:56:44 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 00:56:44 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 00:56:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 00:56:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390a6ee1300672d460b9ec34945f5977cdeb7a2cf7ee7ce77778e311555e5a2`  
		Last Modified: Fri, 29 Sep 2023 00:51:15 GMT  
		Size: 2.8 MB (2765636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980d9e41040298f9395efc037451bda63dab242099de0e34ceb51502aa198496`  
		Last Modified: Fri, 29 Sep 2023 00:51:14 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc29f4c1f00919f2726ab8335d8c4b1584cc2c9e37b0d1c61f18a0a48c23a02`  
		Last Modified: Fri, 29 Sep 2023 00:51:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbba7626daa2eacc7b190e78ff6551931433eeb06f7b498793891fc25523ab03`  
		Last Modified: Sat, 30 Sep 2023 05:32:05 GMT  
		Size: 11.8 MB (11814618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925b9e08f8b5f0e6f0457f5bd083d84648b0590b97f60205f1e36a2ba9350082`  
		Last Modified: Sat, 30 Sep 2023 05:32:04 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1adc625e13534628dd278b8d15748087124a543dc1373a29d6347e0a49e1925`  
		Last Modified: Sat, 30 Sep 2023 05:32:37 GMT  
		Size: 12.8 MB (12788768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acae52a7e7c93cea24813ae345e95f4472db5722f6563e02ea78c33e893b0534`  
		Last Modified: Sat, 30 Sep 2023 05:32:34 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b86847e48fa260a8945f7b7bbbdd588768eccf3f3971e20d79ccd95a2fc185`  
		Last Modified: Sat, 30 Sep 2023 05:32:34 GMT  
		Size: 18.7 KB (18720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e56324d32fd2865cc1bcc4f4cd434e545ca1762adacb419c0a4391a03b0f44`  
		Last Modified: Sat, 30 Sep 2023 05:32:34 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a49ff68b816fdd2ffaec2815179cf94fd1dbe08d5656669c3d213332e18f73b`  
		Last Modified: Thu, 19 Oct 2023 01:13:17 GMT  
		Size: 50.1 MB (50098089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8638194c3215202ad832b9b5ecfab721c1c37e5b4654f2211ad5b67e6ee25bed`  
		Last Modified: Thu, 19 Oct 2023 01:13:12 GMT  
		Size: 7.2 MB (7220500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1707a615cd89e161799e9bb4de3bb90eeb3e10c2518056ce93843a4177039ab9`  
		Last Modified: Thu, 19 Oct 2023 01:13:08 GMT  
		Size: 67.9 KB (67853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6600a611d81c1f1ac0a16fb2c882be1ad79562729321a91ccfc739dede408`  
		Last Modified: Thu, 19 Oct 2023 01:13:07 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfc05a83d398734ea1d828b416d5fdcc79cc203ec94efe9659333ac8ebe8823`  
		Last Modified: Thu, 19 Oct 2023 01:13:12 GMT  
		Size: 25.3 MB (25275797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1383629cf04cdf499f2aefea52ae924284a21409ba0c85e658da33d0d8a02ba6`  
		Last Modified: Thu, 19 Oct 2023 01:13:07 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d218cebd1735736939678637c75ece6ebd7db8bb76e054ad8119f97be22731`  
		Last Modified: Thu, 19 Oct 2023 01:13:07 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.1-fpm-alpine` - linux; s390x

```console
$ docker pull joomla@sha256:35db85bead8e2ca312a624b23bd49de84601624b855ed1f2c31d04d8c812ba0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106736048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca7198fe238e8ecef02a03a54e1fd9f7ae1fc704734581c7d727bef03777fcc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:18:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Sep 2023 00:18:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Sep 2023 00:18:39 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Sep 2023 00:18:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Sep 2023 00:18:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 29 Sep 2023 00:18:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 00:18:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Sep 2023 00:18:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Sep 2023 00:47:54 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 05:35:48 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 05:35:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 05:35:48 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 05:35:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 30 Sep 2023 05:35:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 05:52:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 05:52:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 05:52:11 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 05:52:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 05:52:12 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 05:52:12 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 05:52:12 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 05:52:12 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 05:52:12 GMT
CMD ["php-fpm"]
# Thu, 19 Oct 2023 01:07:04 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 19 Oct 2023 01:07:04 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 19 Oct 2023 01:21:52 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 19 Oct 2023 01:23:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 19 Oct 2023 01:23:22 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Oct 2023 01:23:23 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 19 Oct 2023 01:23:23 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:23:23 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:23:23 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:23:30 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:23:33 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:23:33 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:23:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b5c1e9a2d2847c9799278b6c94003b35994b8a984f9e50737c1572941e2828`  
		Last Modified: Fri, 29 Sep 2023 01:43:27 GMT  
		Size: 2.8 MB (2788383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0230f9f42e261270cd48c4bb7c26a92ac9e597e042a09d0a000fab2f6a3aed3`  
		Last Modified: Fri, 29 Sep 2023 01:43:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12cc85392696abbafd6c89e07013a6f0e4a2ece8438520c685c92438a21e062`  
		Last Modified: Fri, 29 Sep 2023 01:43:25 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053e5745df3fbcc48ea3e1c84eac3d9c24d6554612acc2f8fad09bd982ddd79f`  
		Last Modified: Sat, 30 Sep 2023 06:55:26 GMT  
		Size: 11.8 MB (11814623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e53954f9a2dee84bdf8595dc75696271bb4bdda27fac5e7fbe035143c32816`  
		Last Modified: Sat, 30 Sep 2023 06:55:25 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4153b8d2e47708885acb8edbc293f213ef64f68cddc200967f21db0f491940d`  
		Last Modified: Sat, 30 Sep 2023 06:56:36 GMT  
		Size: 11.6 MB (11588993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7fbda8d6096b3db8c9bbc49e1b1f239d8206f2c04b5c9bd6d26cf7b5c4221c`  
		Last Modified: Sat, 30 Sep 2023 06:56:34 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b82630bdd7025330bce1a2049915d4559f7eb1b19cb53abba4ab9356332fbc`  
		Last Modified: Sat, 30 Sep 2023 06:56:34 GMT  
		Size: 18.8 KB (18751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bea226d436de20a34fc1465fd126aa9cf69e9855e18f3f79942fd46fbb0fc3`  
		Last Modified: Sat, 30 Sep 2023 06:56:34 GMT  
		Size: 8.9 KB (8882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977f8c66ac1bc2629b51bdd35adc6338360e4a03a2dd56a4eee51424da409480`  
		Last Modified: Thu, 19 Oct 2023 01:35:22 GMT  
		Size: 44.9 MB (44929548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8ee479f18b35a2b1beb2fde78c817e3bcf5d94c55cfbf8a6ee1256f8cd637c`  
		Last Modified: Thu, 19 Oct 2023 01:35:17 GMT  
		Size: 7.0 MB (7020087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee31d96b02934acc628650a149cbfe1fad872e3b968c9a5e6f95f479afc9ee25`  
		Last Modified: Thu, 19 Oct 2023 01:35:15 GMT  
		Size: 67.3 KB (67335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdf9ab69fb0819054fdec1e7937874d30adc47c5e1e288bed56a3130a110b0`  
		Last Modified: Thu, 19 Oct 2023 01:35:14 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07df9392c63674b5a036265e48734ee0eb181a74f92001d92ec65fb32cc1ce36`  
		Last Modified: Thu, 19 Oct 2023 01:35:18 GMT  
		Size: 25.3 MB (25275796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0032f801251bbfddcd0ad121a542e370381436224a14e1dc44e46fdad248636`  
		Last Modified: Thu, 19 Oct 2023 01:35:14 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c43981fd5ea73e236bb20891c6984fd41a394feeb7384f2a4ea81325feb3e23`  
		Last Modified: Thu, 19 Oct 2023 01:35:15 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
