## `joomla:4-php8.1-fpm-alpine`

```console
$ docker pull joomla@sha256:9304c3e346edef6c956a7686b12e5f81df1798a24a0a7bef50251be97d571318
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

### `joomla:4-php8.1-fpm-alpine` - linux; amd64

```console
$ docker pull joomla@sha256:34da2f0c06b11227a7889224ff0702195d5fe234d7d1e479be9606b79663424f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108730380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7d6475339f8300232019816b3830c8fbf288a691132eb009348c6a4ec6f10f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:17:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 10:17:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 10:17:24 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 10:17:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:59:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 23:47:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Mon, 27 Mar 2023 23:47:50 GMT
ENV PHP_VERSION=8.1.17
# Mon, 27 Mar 2023 23:47:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Mon, 27 Mar 2023 23:47:50 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Mon, 27 Mar 2023 23:47:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 27 Mar 2023 23:47:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:55:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 23:55:11 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:55:12 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 23:55:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 23:55:12 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 23:55:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 23:55:13 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 23:55:13 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 23:55:13 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 03:15:59 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Mar 2023 03:15:59 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Mar 2023 03:16:03 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 28 Mar 2023 03:18:01 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Mar 2023 03:18:02 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 03:18:03 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Mar 2023 03:18:03 GMT
VOLUME [/var/www/html]
# Tue, 28 Mar 2023 03:18:03 GMT
ENV JOOMLA_VERSION=4.2.9
# Tue, 28 Mar 2023 03:18:03 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Tue, 28 Mar 2023 03:18:10 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Mar 2023 03:18:10 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 28 Mar 2023 03:18:10 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Tue, 28 Mar 2023 03:18:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Mar 2023 03:18:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80fdb865a69a85ee910e603ec69d253469dd9367105df81057c89ef565ab971`  
		Last Modified: Sat, 11 Feb 2023 11:20:06 GMT  
		Size: 1.9 MB (1869555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4dbeadc75c19cda75784e259745d42dd938cf860218f8fec2103bf0852be3c7`  
		Last Modified: Sat, 11 Feb 2023 11:20:06 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264f1d8a0fe21992c1965fb26383acb821f955df95372187fff111c1b19a7401`  
		Last Modified: Tue, 28 Mar 2023 00:54:25 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8288c6d158e7299d24f4956ec85b8cf6149821373723c816a3c70278a0b229`  
		Last Modified: Tue, 28 Mar 2023 00:58:46 GMT  
		Size: 11.8 MB (11839150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9faafbebf9eb82d71d481f80ff8d91dca083e35378ac0b3b31d9d6fa1cdc44`  
		Last Modified: Tue, 28 Mar 2023 00:58:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f69ad1699faa9af3adaf58e6d002c5b4ec8f7fddd0f367369afd1c12c777aa9`  
		Last Modified: Tue, 28 Mar 2023 00:59:10 GMT  
		Size: 14.9 MB (14918623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6269f21a4ce38c6f96b106e3a7b5a23512543d8707c4a4551fc1a82e366e79b`  
		Last Modified: Tue, 28 Mar 2023 00:59:07 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905eba940746f9df6fdce8a08b27c6aed6bfc6b904942dfddcca40a05fa254`  
		Last Modified: Tue, 28 Mar 2023 00:59:07 GMT  
		Size: 19.0 KB (19046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005dbb2a7262c0e0a555c77aafc9c55a02ce0e5f63582278ff5049441b38102a`  
		Last Modified: Tue, 28 Mar 2023 00:59:07 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3b3e7e1291f28d5e2741c51dde068c3e255947256c4dc88f6a7aeacf7af23c`  
		Last Modified: Tue, 28 Mar 2023 03:29:46 GMT  
		Size: 45.7 MB (45697956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86020bf3daa0752f7eff8006f0d45daae292124ea9a0ec67e116ec77899c9ddd`  
		Last Modified: Tue, 28 Mar 2023 03:29:40 GMT  
		Size: 6.6 MB (6628106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642d6bbde8de3a686fa2db7d07acfc51d6a3cdd35efbb3199245f2ebbcdf1e52`  
		Last Modified: Tue, 28 Mar 2023 03:29:37 GMT  
		Size: 68.3 KB (68344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e064e8f0edee61952fd238408a6e424bd976059b030e15297ef7c89285a593e`  
		Last Modified: Tue, 28 Mar 2023 03:29:37 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7209c45e7db9358db7ac710e3c9033efe8885b48bff79332818fc458388abba7`  
		Last Modified: Tue, 28 Mar 2023 03:29:41 GMT  
		Size: 24.3 MB (24298857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0a354338199c6c9e9d73ccfbdb7af90474872da20c08ecc7c8be24e60af299`  
		Last Modified: Tue, 28 Mar 2023 03:29:37 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5a0895a2ff40ac447117d2e49702fe41fe8217ce34bf8ad91932711f27c40c`  
		Last Modified: Tue, 28 Mar 2023 03:29:37 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull joomla@sha256:d5629010fe9950baaf84275060d7664439b6966391d9525ced3657a2c076f61a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102094492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38ec95459ca51a70893b927bd76fc5997f6de9e060ebb5e8e1a73a49ce19296`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 21:07:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 13 Mar 2023 21:07:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 13 Mar 2023 21:07:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 13 Mar 2023 21:07:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:55:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:55:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:55:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:55:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 23:12:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Mon, 27 Mar 2023 23:12:26 GMT
ENV PHP_VERSION=8.1.17
# Mon, 27 Mar 2023 23:12:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Mon, 27 Mar 2023 23:12:26 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Mon, 27 Mar 2023 23:12:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 27 Mar 2023 23:12:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:44:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Mar 2023 00:44:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:44:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Mar 2023 00:44:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Mar 2023 00:44:46 GMT
WORKDIR /var/www/html
# Tue, 28 Mar 2023 00:44:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 28 Mar 2023 00:44:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 28 Mar 2023 00:44:47 GMT
EXPOSE 9000
# Tue, 28 Mar 2023 00:44:47 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 02:56:53 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Mar 2023 02:56:54 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Mar 2023 02:56:59 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 28 Mar 2023 02:58:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Mar 2023 02:58:58 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 02:58:58 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Mar 2023 02:58:59 GMT
VOLUME [/var/www/html]
# Tue, 28 Mar 2023 02:58:59 GMT
ENV JOOMLA_VERSION=4.2.9
# Tue, 28 Mar 2023 02:58:59 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Tue, 28 Mar 2023 02:59:06 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Mar 2023 02:59:06 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 28 Mar 2023 02:59:06 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Tue, 28 Mar 2023 02:59:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Mar 2023 02:59:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b525ba211658332771b8d1e1e6274a63819ca62cce4ae60af48bd6ea6de2e81e`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 1.9 MB (1865508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8f3139761283dde8c51dccb6f9887eedcebb955cb74f916390ef170c7f432c`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b2294d8939831fff5fb231ea290fbc0ada6718821184cbd9378d4e5f23ed7e`  
		Last Modified: Tue, 28 Mar 2023 01:56:54 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9569d7742d2a6a6026c84e1f9b552d34c69be554ab3921302d3be66dd186278a`  
		Last Modified: Tue, 28 Mar 2023 01:59:08 GMT  
		Size: 11.8 MB (11839132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db9d52d47fcb0ab684967c520f837a50acd0d371b1cdd31c7d92e1f6466e68c`  
		Last Modified: Tue, 28 Mar 2023 01:59:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb90e4034d95f22575a8c917c2f1b04c9cd6443de16834b6a2be7a1d627317a`  
		Last Modified: Tue, 28 Mar 2023 01:59:34 GMT  
		Size: 13.4 MB (13390688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a521d18334f5cba4c8b794180c33b9c74098eec97d43d1f64770abbd41a1f7`  
		Last Modified: Tue, 28 Mar 2023 01:59:30 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368e6192ea873c0d3e1d9ce9c127464205c810f179cab33dbc7f7ae3ef99bc13`  
		Last Modified: Tue, 28 Mar 2023 01:59:30 GMT  
		Size: 18.8 KB (18821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282993d064c5d8ca7ed1003822e53eb252e8927264f56db167b0ca79fb50d69f`  
		Last Modified: Tue, 28 Mar 2023 01:59:30 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39e580bfe3e28194a942bf90462ff66b2b246b719db043f7bd9b60207a5df`  
		Last Modified: Tue, 28 Mar 2023 03:05:54 GMT  
		Size: 41.2 MB (41219993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b618cd3f72003d982bc25735c8108142f1caff3399708e59b8da7181578ac`  
		Last Modified: Tue, 28 Mar 2023 03:05:48 GMT  
		Size: 6.3 MB (6266078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fb0767a41f2489952239b88a7f030a5c3cc7693de967accabcee70003bead`  
		Last Modified: Tue, 28 Mar 2023 03:05:46 GMT  
		Size: 68.2 KB (68249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b54b381109925bb276603a22a976ea4c69117f6ae4620ef76471f725a37d7`  
		Last Modified: Tue, 28 Mar 2023 03:05:45 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951e4fd637c77a37bd7cc027afa5864942f5a27d66b19349a1fa400326484737`  
		Last Modified: Tue, 28 Mar 2023 03:05:50 GMT  
		Size: 24.3 MB (24298842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eac995065dde0a1ffaac15d9677eba94db9f7ab4e489e11dd4638555f2c0da3`  
		Last Modified: Tue, 28 Mar 2023 03:05:45 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a15219e5f74de73115969b21d747555a3b8fa4f4ba43588b557d759033d2a70`  
		Last Modified: Tue, 28 Mar 2023 03:05:45 GMT  
		Size: 725.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull joomla@sha256:35a5e9f2f9949490ec1d99b98e120a1c121fde78a96c192a660b9d57fd292420
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96984603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a62f1ee0344e9e14df7bdef33e8f38e99708fe91bd72c28ca4cb150ca43db8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 21:36:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 21:36:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 21:36:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 21:36:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 21:36:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 21:36:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:36:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:36:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 22:12:31 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 16 Mar 2023 23:44:36 GMT
ENV PHP_VERSION=8.1.17
# Thu, 16 Mar 2023 23:44:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Thu, 16 Mar 2023 23:44:36 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Thu, 16 Mar 2023 23:44:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 23:44:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 23:49:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:49:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 23:49:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 23:49:35 GMT
WORKDIR /var/www/html
# Thu, 16 Mar 2023 23:49:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Mar 2023 23:49:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 23:49:36 GMT
EXPOSE 9000
# Thu, 16 Mar 2023 23:49:36 GMT
CMD ["php-fpm"]
# Fri, 17 Mar 2023 03:24:31 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 17 Mar 2023 03:24:31 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 17 Mar 2023 03:24:36 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 17 Mar 2023 03:26:32 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 17 Mar 2023 03:26:33 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Mar 2023 03:26:33 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 17 Mar 2023 03:26:33 GMT
VOLUME [/var/www/html]
# Fri, 17 Mar 2023 03:26:33 GMT
ENV JOOMLA_VERSION=4.2.9
# Fri, 17 Mar 2023 03:26:34 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Fri, 17 Mar 2023 03:26:41 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 17 Mar 2023 03:26:41 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 17 Mar 2023 03:26:41 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Fri, 17 Mar 2023 03:26:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Mar 2023 03:26:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9169ee53f4934f506408e6416f765930339b501b32c7cc932909cc1f0c22190`  
		Last Modified: Wed, 01 Mar 2023 23:08:09 GMT  
		Size: 1.7 MB (1715927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c652394f365d675be459982d3ff25a0cd449736b35738b11ada9fbcd26323603`  
		Last Modified: Wed, 01 Mar 2023 23:08:08 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8004a620a679d75c3c87ee59d53822c6d18bd9cb75d9bb8e515e1aa829e823e`  
		Last Modified: Wed, 01 Mar 2023 23:08:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157a07c73f8625f566569e94f2fd18261d9439ca36dd9752d81f894ee3bd87b0`  
		Last Modified: Fri, 17 Mar 2023 00:19:37 GMT  
		Size: 11.8 MB (11839130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eaa75cee390f6fdc40016edf0c726b2b7f673eaf10223891ac998e91dfba01`  
		Last Modified: Fri, 17 Mar 2023 00:19:35 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53f15daec813dd7bc2c01ab312df0ed00400b5306debb8267308c640ddaa65d`  
		Last Modified: Fri, 17 Mar 2023 00:20:13 GMT  
		Size: 10.6 MB (10601667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7566066654600ccf1435bf7a86ee90dd80a135a7404c09eb61708da76889e40`  
		Last Modified: Fri, 17 Mar 2023 00:20:11 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4312d2a2018e18f58f5cdad78f10dd8ab951c251f209dcd12de90bf54951e5`  
		Last Modified: Fri, 17 Mar 2023 00:20:11 GMT  
		Size: 18.7 KB (18747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92af324f0150d18d7c1d36c606192bbbe9aaa58d86875468e1c8748a2ba86680`  
		Last Modified: Fri, 17 Mar 2023 00:20:11 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9531e20e99716753854e314be951ac9c8ddfdb859858bfd5577019018488399`  
		Last Modified: Fri, 17 Mar 2023 03:32:15 GMT  
		Size: 39.3 MB (39322286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83493ecffca7cd2973e490ba02177538358f4f0a440185e8b588c8ec3f9eb5f3`  
		Last Modified: Fri, 17 Mar 2023 03:32:10 GMT  
		Size: 6.2 MB (6235045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6909761125dca95cb4f315d8922e3211d52eec88108f8192e570e6806079cb0f`  
		Last Modified: Fri, 17 Mar 2023 03:32:06 GMT  
		Size: 68.2 KB (68167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253551b8e7166ddd249ac09587de4d00c9a6ef25ca37a2da7f66956761c08eac`  
		Last Modified: Fri, 17 Mar 2023 03:32:06 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b756454d884e5409385f702f334608656a4ca49ac3cf848efa08fd44ed98271`  
		Last Modified: Fri, 17 Mar 2023 03:32:11 GMT  
		Size: 24.3 MB (24298843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63b7bc4c72b861acba2bda2455077c2ede0e80cc05425e304d14d6b1bcfa6b2`  
		Last Modified: Fri, 17 Mar 2023 03:32:06 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c0711505a3506ce62acd09005625d9a6c9fb12c5d8da7226e754313dad3046`  
		Last Modified: Fri, 17 Mar 2023 03:32:06 GMT  
		Size: 727.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:622fa400e39dce36d39fee1a29ca72140c15c84813e4a2535d2f3838cb534e06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107074074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c510a5212cf5e1b7472c9d480e87f1cbaf4e8d0dcb1775a47425fa02c92cf3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:02:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 02:02:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 02:02:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 02:02:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 23:26:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 23:26:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 23:26:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 23:26:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Mar 2023 00:16:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 28 Mar 2023 00:16:26 GMT
ENV PHP_VERSION=8.1.17
# Tue, 28 Mar 2023 00:16:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Tue, 28 Mar 2023 00:16:26 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Tue, 28 Mar 2023 00:16:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 28 Mar 2023 00:16:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:24:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Mar 2023 00:24:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:24:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Mar 2023 00:24:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Mar 2023 00:24:13 GMT
WORKDIR /var/www/html
# Tue, 28 Mar 2023 00:24:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 28 Mar 2023 00:24:14 GMT
STOPSIGNAL SIGQUIT
# Tue, 28 Mar 2023 00:24:14 GMT
EXPOSE 9000
# Tue, 28 Mar 2023 00:24:14 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 02:32:05 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Mar 2023 02:32:06 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Mar 2023 02:32:09 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 28 Mar 2023 02:33:52 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Mar 2023 02:33:53 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 02:33:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Mar 2023 02:33:54 GMT
VOLUME [/var/www/html]
# Tue, 28 Mar 2023 02:33:54 GMT
ENV JOOMLA_VERSION=4.2.9
# Tue, 28 Mar 2023 02:33:54 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Tue, 28 Mar 2023 02:33:59 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Mar 2023 02:33:59 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 28 Mar 2023 02:33:59 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Tue, 28 Mar 2023 02:33:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Mar 2023 02:34:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65da1d1bbae15a06f79c4d79d885439cb51d02c27c69741770a1ace04a962454`  
		Last Modified: Sat, 11 Feb 2023 03:02:23 GMT  
		Size: 1.9 MB (1862646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53689469854ea07050d653c2567c0a362a36bf42c1db6ad7ca78f0ce04d4a862`  
		Last Modified: Sat, 11 Feb 2023 03:02:22 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6dc56a855ceb86b0a12444e3f18b9c0fe2a825021cc250002e2932fdc3b1ec`  
		Last Modified: Tue, 28 Mar 2023 01:11:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a3fdfe6e6b0056a1f4bb863bcdb9a7202e04e1638834319cd66cad34064d2`  
		Last Modified: Tue, 28 Mar 2023 01:15:58 GMT  
		Size: 11.8 MB (11839137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51adb5c4c45261be061dae663a6b4b34110200c141a6079787b9b650b07a8410`  
		Last Modified: Tue, 28 Mar 2023 01:15:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4afc50538760d0003a355a03fc6ca077c258fe8c952f6bbc3e101eee7e83fa8`  
		Last Modified: Tue, 28 Mar 2023 01:16:26 GMT  
		Size: 14.8 MB (14765870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c4c1420848303840c5f69b63c7b6f377725c87335d96df9093a3678a6e4733`  
		Last Modified: Tue, 28 Mar 2023 01:16:24 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb6fc8d9d7d92eeeed2ec5c1940b9bb023aafd9de3b4205eacaa1d6b1ac2ddc`  
		Last Modified: Tue, 28 Mar 2023 01:16:24 GMT  
		Size: 18.8 KB (18826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472b0625e91c56397e0904abbd4de1d220afb4aafb126728885d40eecf4bf38`  
		Last Modified: Tue, 28 Mar 2023 01:16:24 GMT  
		Size: 8.9 KB (8874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb7cfc249cf2a264fac88d08db7f59e26876089f298989499950553dabedc9f`  
		Last Modified: Tue, 28 Mar 2023 02:44:13 GMT  
		Size: 44.4 MB (44374029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab76e3d907adb6b68c780d94f03b0e4e0793fdac826293a31d4d9bb58a02d31`  
		Last Modified: Tue, 28 Mar 2023 02:44:08 GMT  
		Size: 6.6 MB (6568195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8543104589e5d64a41e2966742ccca69ae94ae3b97e07a6cc62e4f7a83b507`  
		Last Modified: Tue, 28 Mar 2023 02:44:05 GMT  
		Size: 68.3 KB (68253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08efabda573296044ecff82241bb84bbf19a874421f59f110fd0177412a917a`  
		Last Modified: Tue, 28 Mar 2023 02:44:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00300ef0945f1d8ce0c242899eb85a34359e25a40456ec3e8cf8a8e0eb2060d5`  
		Last Modified: Tue, 28 Mar 2023 02:44:08 GMT  
		Size: 24.3 MB (24298863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fa453b53c25a0620f7d50deb14880ca1fbf1946152efe7e0909739c98ef478`  
		Last Modified: Tue, 28 Mar 2023 02:44:05 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18417b3adbca451b0487c5ef1c591bca330c300547f54fff5294e32a4820927f`  
		Last Modified: Tue, 28 Mar 2023 02:44:05 GMT  
		Size: 725.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm-alpine` - linux; 386

```console
$ docker pull joomla@sha256:d5de98ed64689cca97fc52af3430ee34ef6cdd8530632c114bb2954a5b0dedfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105510033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ae8d1acebd0eef99eca17b33403b8830302768360a2c26836af78f67fd33433`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 15:08:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 15:08:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 15:08:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 15:08:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 15:08:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 15:08:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:08:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:08:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 16:30:36 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 16 Mar 2023 23:47:44 GMT
ENV PHP_VERSION=8.1.17
# Thu, 16 Mar 2023 23:47:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Thu, 16 Mar 2023 23:47:44 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Thu, 16 Mar 2023 23:47:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 23:47:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Mar 2023 00:00:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 17 Mar 2023 00:00:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 17 Mar 2023 00:00:10 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Mar 2023 00:00:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Mar 2023 00:00:11 GMT
WORKDIR /var/www/html
# Fri, 17 Mar 2023 00:00:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 17 Mar 2023 00:00:11 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Mar 2023 00:00:11 GMT
EXPOSE 9000
# Fri, 17 Mar 2023 00:00:12 GMT
CMD ["php-fpm"]
# Fri, 17 Mar 2023 02:06:15 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 17 Mar 2023 02:06:15 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 17 Mar 2023 02:06:25 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 17 Mar 2023 02:08:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 17 Mar 2023 02:08:49 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Mar 2023 02:08:50 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 17 Mar 2023 02:08:50 GMT
VOLUME [/var/www/html]
# Fri, 17 Mar 2023 02:08:50 GMT
ENV JOOMLA_VERSION=4.2.9
# Fri, 17 Mar 2023 02:08:50 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Fri, 17 Mar 2023 02:08:58 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 17 Mar 2023 02:08:58 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 17 Mar 2023 02:08:59 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Fri, 17 Mar 2023 02:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Mar 2023 02:08:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5394292b2b83b2b876e0f3301349b0299305f8034ed3fa062d20c20268efbd52`  
		Last Modified: Wed, 01 Mar 2023 18:23:52 GMT  
		Size: 2.0 MB (1991827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e923c580cf6f27c534dc0869dfae4f7e9e424c149940e20be2ffef7aa344c424`  
		Last Modified: Wed, 01 Mar 2023 18:23:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c6096004f76a359d1c0d104682a61452036bae13908723157c118939b617b6`  
		Last Modified: Wed, 01 Mar 2023 18:23:51 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17887aee92afb496aeb706457ca6b3ccd074623dffe57f0db871cade7db98c93`  
		Last Modified: Fri, 17 Mar 2023 00:48:03 GMT  
		Size: 11.8 MB (11839140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8a347e5ede6b6a293db90857150d0b1c54d103320f635aae4707bc1f2abb1d`  
		Last Modified: Fri, 17 Mar 2023 00:48:02 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb965fe7ceecb1b66a038056839758d61af7d1f12cef4a3787dc5b64542a1eb7`  
		Last Modified: Fri, 17 Mar 2023 00:48:42 GMT  
		Size: 12.8 MB (12757642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb174f08eb3db5d2a48ca89a86f3f155d3ca3a823f9a0bf155fcca9c4df068bd`  
		Last Modified: Fri, 17 Mar 2023 00:48:39 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f33586c206cfa67c589010184505a4a4af4cf85162e118d8b0498989ec7463`  
		Last Modified: Fri, 17 Mar 2023 00:48:39 GMT  
		Size: 18.9 KB (18931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d2a8b3b6454ec7d2aa1579b05c17f8c4c3765ea65e2b47cf1e45d0e71a41fd`  
		Last Modified: Fri, 17 Mar 2023 00:48:39 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42e6a82f45e7b18883671111bb12001c3d07832c80b86e0fe0bad4967f56424`  
		Last Modified: Fri, 17 Mar 2023 02:14:56 GMT  
		Size: 44.3 MB (44281251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c3c523d09e3a67a823e7568ae08964bb4555768a750073b5ae87146391d80a`  
		Last Modified: Fri, 17 Mar 2023 02:14:48 GMT  
		Size: 6.8 MB (6825488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2924c0b2d63dc10979e26e81bc308d5f845f7948f28b1827f94b0d854df5505f`  
		Last Modified: Fri, 17 Mar 2023 02:14:43 GMT  
		Size: 68.3 KB (68263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6848561e1420b00c46bbf65a5aeca7a28a4306b08b1a3f24b2a97a76b4adb`  
		Last Modified: Fri, 17 Mar 2023 02:14:43 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecdd4e19ace247bf45f853c6c32954e22a7a1386442d578b9b5ec0a81c1f68e`  
		Last Modified: Fri, 17 Mar 2023 02:14:50 GMT  
		Size: 24.3 MB (24298844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030f8f0d66ec19faa8fa60f1794f4b48245be2f3666fb147164f90754c0efc6`  
		Last Modified: Fri, 17 Mar 2023 02:14:43 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c554daae7bfd8a97a006d18760d1492047c5d1de6dadd489e422f76a9ea695`  
		Last Modified: Fri, 17 Mar 2023 02:14:43 GMT  
		Size: 725.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm-alpine` - linux; ppc64le

```console
$ docker pull joomla@sha256:7012d231d44c21c59bd4cfbf3c9fa58f0672d3ca0da701c74a9073eafdddc95b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111487688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90535e15a9606dc9eaec4fb5b751ed0ef272088ea4754544cacc2c5eba4875d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:08:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 10 Feb 2023 23:08:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 10 Feb 2023 23:08:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 23:08:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 10 Feb 2023 23:08:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 10 Feb 2023 23:38:04 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 16 Mar 2023 22:12:00 GMT
ENV PHP_VERSION=8.1.17
# Thu, 16 Mar 2023 22:12:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Thu, 16 Mar 2023 22:12:01 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Thu, 16 Mar 2023 22:12:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 22:12:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:20:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 22:20:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:20:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 22:20:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 22:20:31 GMT
WORKDIR /var/www/html
# Thu, 16 Mar 2023 22:20:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Mar 2023 22:20:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 22:20:33 GMT
EXPOSE 9000
# Thu, 16 Mar 2023 22:20:33 GMT
CMD ["php-fpm"]
# Fri, 17 Mar 2023 00:04:17 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 17 Mar 2023 00:04:17 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 17 Mar 2023 00:04:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 17 Mar 2023 00:08:08 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 17 Mar 2023 00:08:10 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Mar 2023 00:08:11 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 17 Mar 2023 00:08:12 GMT
VOLUME [/var/www/html]
# Fri, 17 Mar 2023 00:08:12 GMT
ENV JOOMLA_VERSION=4.2.9
# Fri, 17 Mar 2023 00:08:12 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Fri, 17 Mar 2023 00:08:24 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 17 Mar 2023 00:08:26 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 17 Mar 2023 00:08:26 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Fri, 17 Mar 2023 00:08:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Mar 2023 00:08:27 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfa1898e4103c3c306fd301195ab70581ac39be1be2ad84260c45520aaa5d05`  
		Last Modified: Sat, 11 Feb 2023 00:28:07 GMT  
		Size: 1.9 MB (1946683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fded8faaf0ac23f23c9b92d38d3e833d89b91908a65685dd807fc5ed5718e57`  
		Last Modified: Sat, 11 Feb 2023 00:28:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8afe3cb27338f4dc17809e93d8c3ba65ea9bbe27288f937f4e25fb03bc6010`  
		Last Modified: Sat, 11 Feb 2023 00:28:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577b02bdf7580d38f56b8715192424b61c62a28faf8cf68d16aad34c7ba9887f`  
		Last Modified: Thu, 16 Mar 2023 22:55:53 GMT  
		Size: 11.8 MB (11839145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f852cc776caceae0b8ad38c89d6de16514ec0ce3d814a840da29f27891def53b`  
		Last Modified: Thu, 16 Mar 2023 22:55:52 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5adb971245beaf55713acd729271be607a384c7e5eada672c928cfde40c61c9`  
		Last Modified: Thu, 16 Mar 2023 22:56:31 GMT  
		Size: 13.1 MB (13128992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c59a071d7732a91241bf45c697de5cb2b40d0d1bb4ad24d799fc83b2c76b7`  
		Last Modified: Thu, 16 Mar 2023 22:56:28 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fccec620fe560c5346a52e81a09c3fab973dfb1cd8c54ecf32d6e2d00dca02b`  
		Last Modified: Thu, 16 Mar 2023 22:56:28 GMT  
		Size: 18.8 KB (18785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2316be1f05681d23d64f1ad6c18df45dda381dc3e6357caba49393e360519174`  
		Last Modified: Thu, 16 Mar 2023 22:56:28 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed52839e3ab37e038f4aa1e02ae1badc80fa3a9bed10a35585f9728bcd73dd68`  
		Last Modified: Fri, 17 Mar 2023 00:16:35 GMT  
		Size: 49.8 MB (49843407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a4af0183d03265a541f6ce0548c5f8d2a1db15da53463be09a4739a7c3116`  
		Last Modified: Fri, 17 Mar 2023 00:16:26 GMT  
		Size: 6.9 MB (6936605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4de3c7e569289b8aa3c6e8434a8cfd8c0afb05cf695526967ce4b2f755cc74`  
		Last Modified: Fri, 17 Mar 2023 00:16:21 GMT  
		Size: 68.2 KB (68197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebcf6ffbe68fe8e338f0572e8ef051c9d5dbdf1dddc68f601520a9fb8e814d9`  
		Last Modified: Fri, 17 Mar 2023 00:16:21 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d02734d779625f1acc01362caeee1cc26598eb208cb5fec8e89d9f00b9b7c98`  
		Last Modified: Fri, 17 Mar 2023 00:16:28 GMT  
		Size: 24.3 MB (24298835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440e332def8484ac103c05930c5f1b89a4afa0647522451dce67ee0c5b277596`  
		Last Modified: Fri, 17 Mar 2023 00:16:21 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70c6ac34087373255eeccc5e757a56a09c9931a4f664e333142b8c6f5aff2c7`  
		Last Modified: Fri, 17 Mar 2023 00:16:21 GMT  
		Size: 723.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm-alpine` - linux; s390x

```console
$ docker pull joomla@sha256:aa21bb675113674466f1b395052a9a00b72914a65ea86051b3f7493661c070a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107999602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b3e8314afa85ccfb7e11d45d1b7a7a70176a36ecb2b71594f36e4b66e75d7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:40:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 03:40:21 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 03:40:22 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 03:40:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:56:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:56:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:56:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:56:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 23:24:20 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Mon, 27 Mar 2023 23:24:20 GMT
ENV PHP_VERSION=8.1.17
# Mon, 27 Mar 2023 23:24:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Mon, 27 Mar 2023 23:24:20 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Mon, 27 Mar 2023 23:24:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 27 Mar 2023 23:24:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:30:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 23:30:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:30:04 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 23:30:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 23:30:04 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 23:30:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 23:30:05 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 23:30:05 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 23:30:05 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 01:15:26 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Mar 2023 01:15:26 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Mar 2023 01:15:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 28 Mar 2023 01:18:56 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .joomla-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Mar 2023 01:18:57 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 01:18:57 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Mar 2023 01:18:57 GMT
VOLUME [/var/www/html]
# Tue, 28 Mar 2023 01:18:57 GMT
ENV JOOMLA_VERSION=4.2.9
# Tue, 28 Mar 2023 01:18:58 GMT
ENV JOOMLA_SHA512=25805241234753c05f562cf3be599c63cfcfb2e7dcf6b5b76b1cb4b6a4d305497c720eaccdc0939e4fceffa83099db9b3c44963fce86bafc3efc2fc34fecaa20
# Tue, 28 Mar 2023 01:19:04 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.9/Joomla_4.2.9-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Mar 2023 01:19:06 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 28 Mar 2023 01:19:07 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Tue, 28 Mar 2023 01:19:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Mar 2023 01:19:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e08f96f9a305daacf9ee42f9847666c785231f5db9684aae1648426463f923`  
		Last Modified: Sat, 11 Feb 2023 04:35:13 GMT  
		Size: 1.9 MB (1917113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b2b7eda29298bc923307ecd06eca2607d89341d31329cad08c2ddd6d3dda03`  
		Last Modified: Sat, 11 Feb 2023 04:35:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed3e28bc20861203adff74b75366ba94168ab87750cb62dc24cda8b23c04be`  
		Last Modified: Tue, 28 Mar 2023 00:03:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392fae61250f516e16dee618c7bf8e01048a569bbbf043e8c247a135c45e44dc`  
		Last Modified: Tue, 28 Mar 2023 00:05:30 GMT  
		Size: 11.8 MB (11839153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749c73386e62a34a0857f81c782c6662a2675bae2a216f9c4d3c513c160f1c40`  
		Last Modified: Tue, 28 Mar 2023 00:05:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93241f2516ac9f18d2e763477521403973f893a5eef26e29dcffb4cb979eef9`  
		Last Modified: Tue, 28 Mar 2023 00:05:47 GMT  
		Size: 13.8 MB (13811547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adc5afb0eb529adfb7af226042c2a9bb88956cd5197131d32e282f28736b6ca`  
		Last Modified: Tue, 28 Mar 2023 00:05:45 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e60e85fff5c69f6dd62788f6f4026d31ad59ce34151393d5c0dcf30e8250f5b`  
		Last Modified: Tue, 28 Mar 2023 00:05:45 GMT  
		Size: 18.8 KB (18845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea1ea562defce691c9ccbda27a09fdc1f73c8d6a64dcde6cbfae50bcbae498`  
		Last Modified: Tue, 28 Mar 2023 00:05:45 GMT  
		Size: 8.9 KB (8875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea336b3a5be14e103522871beb8c2c0a6d8ce49ca459d034cf270e728f3976b2`  
		Last Modified: Tue, 28 Mar 2023 01:27:54 GMT  
		Size: 46.2 MB (46211643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24725f7a74115c704b82e29471be7ed9eac95748baf2ef23cfada27134206b1c`  
		Last Modified: Tue, 28 Mar 2023 01:27:48 GMT  
		Size: 6.6 MB (6642701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af34bd8847f8d9ecac2fc92d03011213844c2d95716f84e2dd647ac781afe14`  
		Last Modified: Tue, 28 Mar 2023 01:27:46 GMT  
		Size: 68.3 KB (68347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7ef8d778163945212dc70d5c7ede410a791ba41f41717d4e240fe3bdd6aa56`  
		Last Modified: Tue, 28 Mar 2023 01:27:46 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54f57c567325f3073595acb94d3221c015bcac42f6d576c6f58589515db319c`  
		Last Modified: Tue, 28 Mar 2023 01:27:50 GMT  
		Size: 24.3 MB (24298842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e4b20ad4b9844ae24502b300a6ec8b105a96f89cf6697b02efaa54d48e276`  
		Last Modified: Tue, 28 Mar 2023 01:27:46 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6736bd472208c783b466f8f0127a6b0736f06314bfe2458e66d60520d97470b7`  
		Last Modified: Tue, 28 Mar 2023 01:27:46 GMT  
		Size: 725.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
