## `joomla:3-php7.3-fpm-alpine`

```console
$ docker pull joomla@sha256:d3d9450b63634cff8b802fb15ca1a6cecb4338b92f5321ebf039df9cb318c550
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

### `joomla:3-php7.3-fpm-alpine` - linux; amd64

```console
$ docker pull joomla@sha256:9dff1701e323f18838ba0cc3142ad3fa9d1ba7d7eeb4b6611c7867c39a59e4ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47698064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb180ba9e8d7ce121694c2986f4b709364f7cfa386facadcba6ca327f82aa57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 07:48:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 07:48:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 07:48:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 07:48:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 09:59:00 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 09:59:01 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 09:59:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 09:59:01 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 09:59:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 09:59:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 10:11:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 10:11:28 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 10:11:30 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 10:11:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 10:11:30 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 10:11:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 10:11:32 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 10:11:32 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 10:11:32 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 15:04:02 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 13 Nov 2021 15:04:03 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 13 Nov 2021 15:04:04 GMT
RUN apk add --no-cache 	bash
# Sat, 13 Nov 2021 15:05:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 13 Nov 2021 15:05:42 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 15:05:42 GMT
ENV JOOMLA_VERSION=3.10.3
# Sat, 13 Nov 2021 15:05:42 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Sat, 13 Nov 2021 15:05:47 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 13 Nov 2021 15:05:48 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 13 Nov 2021 15:05:48 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 13 Nov 2021 15:05:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 15:05:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f99012ff9aa7245baebc28963e44f53cc1832fcfaec246f78b5e7e861fbe6`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.7 MB (1712224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db81da314e0b3e7be6d4c80bd6a2cdc1d7f66d6fffc8334a527f6b6e20fca340`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5646ac679ebe77089fb6446f9911a66ae64db7d5b774d356b04c1c911ca0a081`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9292b685181028ca2ed46331518b9878398e1b35ace836313be23c7bd914f78`  
		Last Modified: Sat, 13 Nov 2021 10:50:15 GMT  
		Size: 12.2 MB (12162705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54af0e5545a2c78d6770af2c39e379e850030885a6e94d0cb31056c23dfa24ff`  
		Last Modified: Sat, 13 Nov 2021 10:50:14 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6657c1cc47b6260742af8639cbc208519e43750e6bc7c67807a3a4bf5b2dc45`  
		Last Modified: Sat, 13 Nov 2021 10:50:51 GMT  
		Size: 14.6 MB (14562873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a275c1e454da1f124f036141bc6d55d35a21b68f0293fce80e0671c58b008a67`  
		Last Modified: Sat, 13 Nov 2021 10:50:48 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da6b5ec09c69472619376836b7914861a9d1bbff059f9c67b26cb1af62fa9ff`  
		Last Modified: Sat, 13 Nov 2021 10:50:48 GMT  
		Size: 18.0 KB (18015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce88f96b4df788ce42df92e73f25e3e79a98d7fa1e821433a8af2d484e770b9e`  
		Last Modified: Sat, 13 Nov 2021 10:50:48 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6a91dcb347ddc852060dc8a7b41444bd5d5210b45d3fe0f556b416bbc05b76`  
		Last Modified: Sat, 13 Nov 2021 15:09:43 GMT  
		Size: 465.8 KB (465781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64963f935db0d517f48f716c815c68c269cb8d200ad4050e7e214cef08c45caf`  
		Last Modified: Sat, 13 Nov 2021 15:09:44 GMT  
		Size: 6.3 MB (6258111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb76e25bffadecf6dd81e253f7386d2fcf13722b26b5f5c4b96cedd0eccde5a6`  
		Last Modified: Sat, 13 Nov 2021 15:09:45 GMT  
		Size: 9.7 MB (9680820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f551130641456b3f609414f049b52c693ee174586800fc13d4424d2157bcf775`  
		Last Modified: Sat, 13 Nov 2021 15:09:43 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7514457619dc9c16a9481c543271eeca6898f98076ba3d77edfb8f34fb13bf92`  
		Last Modified: Sat, 13 Nov 2021 15:09:43 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull joomla@sha256:8422ae874da6826b894d9fe223062dc438a410ab6f201693b2f610e4660ff627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45840349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b88a85ac117dd1398a51476252d8ece5e3c82451d88ad0b311d25b3363cabf7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:00:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:00:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:00:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:00:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:11:29 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 18 Nov 2021 16:24:39 GMT
ENV PHP_VERSION=7.3.33
# Thu, 18 Nov 2021 16:24:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Thu, 18 Nov 2021 16:24:40 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Thu, 18 Nov 2021 16:24:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:24:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:34:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:34:28 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:34:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:34:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:34:32 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:34:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:34:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:34:35 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:34:35 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 19:03:05 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 18 Nov 2021 19:03:05 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 18 Nov 2021 19:03:08 GMT
RUN apk add --no-cache 	bash
# Thu, 18 Nov 2021 19:07:31 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 18 Nov 2021 19:07:32 GMT
VOLUME [/var/www/html]
# Thu, 18 Nov 2021 19:07:32 GMT
ENV JOOMLA_VERSION=3.10.3
# Thu, 18 Nov 2021 19:07:33 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Thu, 18 Nov 2021 19:07:45 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 18 Nov 2021 19:07:46 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 18 Nov 2021 19:07:47 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 18 Nov 2021 19:07:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 19:07:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fb65eff99d3570be8bbee58e3796b49e0e6fbc64d6c2b55e01eaf1b07709af`  
		Last Modified: Sat, 13 Nov 2021 02:49:22 GMT  
		Size: 1.7 MB (1702248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe18ffa25cea29b8a20ba6c41b7485fd89e792d6d333919ea738dcff33555f`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c6f1ae3409a42a8b2531ec3f19b4dddc77724624fdc7fe72175b53fa03ad0`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc877c3a6bcc4e3b78a8d85f86662e5a59e26c58b32f6d49c89f124e248da2dc`  
		Last Modified: Thu, 18 Nov 2021 17:08:30 GMT  
		Size: 12.2 MB (12164221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b92c5aceeaae3ced5ccc2b0a8243669ed1ee2aaa7f3d5b5c02ef01b540200d`  
		Last Modified: Thu, 18 Nov 2021 17:08:28 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd38758b5d1bcda6a8609a1dda3ac00cdc8044aff4f52040a572c9954b5a1d`  
		Last Modified: Thu, 18 Nov 2021 17:09:22 GMT  
		Size: 13.5 MB (13493423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88042017e6e9b1555b8f4413f6261a19825790b4c7bc2ffb1c48b65820fd09d1`  
		Last Modified: Thu, 18 Nov 2021 17:09:13 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2c7760488aadafe832546c593ba0f3e5d10f3a1a34199588dda71a05c7b6b`  
		Last Modified: Thu, 18 Nov 2021 17:09:13 GMT  
		Size: 18.0 KB (18034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a5914d2208b4ea665ac131d36859ae0b7a2503c229b72c8292c2d5dc99cd7a`  
		Last Modified: Thu, 18 Nov 2021 17:09:13 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ac793a3b8bb3506d7d5cea582b429d34e13c59eacdf60b5aa3c3c2504dabe4`  
		Last Modified: Thu, 18 Nov 2021 19:14:50 GMT  
		Size: 454.6 KB (454575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fe6116d249eeecac44059eb31d03a3640da62e4ba2cba562435a487d6852b`  
		Last Modified: Thu, 18 Nov 2021 19:14:52 GMT  
		Size: 5.7 MB (5677085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0884dab55bab49e1a94b7031bab78c68b3b481faff89c01ea2841c9625408e52`  
		Last Modified: Thu, 18 Nov 2021 19:15:01 GMT  
		Size: 9.7 MB (9680819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae88a07548b70243d987b38ba2e14fc528ece15eea422e6d0a7c97fb14e31c`  
		Last Modified: Thu, 18 Nov 2021 19:14:49 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181a5d3c9c8045ebca5a1d8ec9756a9ea7cd9fdae69eaaa6669230ac4f2c46a2`  
		Last Modified: Thu, 18 Nov 2021 19:14:49 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull joomla@sha256:fd9e59f6ef9a2717e729fd44ac08a1ef410c502f6613b25272bb183d3ee4c867
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44629539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bac548eeac731187788e8ccb520570dcf3df4dd748a39627328f9c95ffa2895`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:20:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 02:20:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 02:20:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 02:20:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 02:20:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 02:20:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 03:32:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 03:32:54 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 03:32:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 03:32:55 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 03:33:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 03:33:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:42:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 03:42:18 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:42:21 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 03:42:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 03:42:21 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 03:42:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 03:42:24 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 03:42:24 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 03:42:24 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 17:46:31 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 13 Nov 2021 17:46:32 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 13 Nov 2021 17:46:34 GMT
RUN apk add --no-cache 	bash
# Sat, 13 Nov 2021 17:50:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 13 Nov 2021 17:50:46 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 17:50:47 GMT
ENV JOOMLA_VERSION=3.10.3
# Sat, 13 Nov 2021 17:50:47 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Sat, 13 Nov 2021 17:50:59 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 13 Nov 2021 17:51:00 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 13 Nov 2021 17:51:01 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 13 Nov 2021 17:51:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 17:51:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d591a38553bed13e4644c2ee36cc92a36f4f866265bcec258baef16176c11b`  
		Last Modified: Sat, 13 Nov 2021 04:21:17 GMT  
		Size: 1.6 MB (1571523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a132a38f5266edd87272c20d2129b4448b3dfb530a70424219ddd45fd1d2eb73`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99b8f25382a7fadffc08ae9ebf09b2a2be48a858daf03148035e46335c089a`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fce6240701bfe6d0a640c4e0d575fe2efc6fac89e9098e8bdb9fc46c79e5c3`  
		Last Modified: Sat, 13 Nov 2021 04:33:45 GMT  
		Size: 12.2 MB (12162709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558a2c12a8f92ed07555cb7d43d6373c91171a25e85d049a8b003ab046de3946`  
		Last Modified: Sat, 13 Nov 2021 04:33:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf171de4efaea696344ee5eb132f4fbf0a478f3727aab36a22c41ba196ac76e9`  
		Last Modified: Sat, 13 Nov 2021 04:34:37 GMT  
		Size: 12.6 MB (12627381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47609911a512f251796537bcddac6186b2354c94383dd38ccd05b581bc32c57d`  
		Last Modified: Sat, 13 Nov 2021 04:34:28 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85b7ce8944731a9b04823bcfc7d6419cb5a9a7688478ef4a0747fe5d3118940`  
		Last Modified: Sat, 13 Nov 2021 04:34:28 GMT  
		Size: 18.0 KB (18021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4619bccd3dc9eb0a7d65afb440bda459cdf571b5a96ed1f864e981da70637`  
		Last Modified: Sat, 13 Nov 2021 04:34:28 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38fce4d882c38877d323b0062a119f7aba140e4f2db019fea2ce545d8cb33d7`  
		Last Modified: Sat, 13 Nov 2021 18:03:07 GMT  
		Size: 415.1 KB (415080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9718d4ada0e2860e4f29659772515447a0c97e460264b53f992cb84a0c84a53c`  
		Last Modified: Sat, 13 Nov 2021 18:03:10 GMT  
		Size: 5.7 MB (5700838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc1b9df811070bf4589f137884d2d93517e57b709bc5f52952f24593649d877`  
		Last Modified: Sat, 13 Nov 2021 18:03:19 GMT  
		Size: 9.7 MB (9680811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a6dfabdfbdb2af9570775cc760cbf0b81c331c987b9c3d568ee8f91a12aa9a`  
		Last Modified: Sat, 13 Nov 2021 18:03:07 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e12e6e8230b1be9cc423cf967e3526415ef9264b153aa1c7a40ad22bf4ac6c`  
		Last Modified: Sat, 13 Nov 2021 18:03:07 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:385777f0bbfabd02a2e06e6bc594e16c27e36712bd6e34577bad03e6fd776bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47222640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644791c47ff8da63149aa92b70a976b97d5f91459ee3c3a00ffba494ef928ffe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:30:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:30:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:30:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:30:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:30:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:30:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:52:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 12 Nov 2021 20:52:04 GMT
ENV PHP_VERSION=7.3.32
# Fri, 12 Nov 2021 20:52:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Fri, 12 Nov 2021 20:52:06 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Fri, 12 Nov 2021 20:52:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 12 Nov 2021 20:52:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Nov 2021 21:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Nov 2021 21:00:37 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 12 Nov 2021 21:00:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Nov 2021 21:00:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Nov 2021 21:00:40 GMT
WORKDIR /var/www/html
# Fri, 12 Nov 2021 21:00:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 12 Nov 2021 21:00:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 12 Nov 2021 21:00:43 GMT
EXPOSE 9000
# Fri, 12 Nov 2021 21:00:44 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 14:29:50 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 13 Nov 2021 14:29:50 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 13 Nov 2021 14:29:52 GMT
RUN apk add --no-cache 	bash
# Sat, 13 Nov 2021 14:31:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 13 Nov 2021 14:31:54 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 14:31:55 GMT
ENV JOOMLA_VERSION=3.10.3
# Sat, 13 Nov 2021 14:31:56 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Sat, 13 Nov 2021 14:32:02 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 13 Nov 2021 14:32:03 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 13 Nov 2021 14:32:04 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 13 Nov 2021 14:32:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 14:32:05 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716534ffbe55fb7b1cdc9c51401565113fe78d473379c595bf42e6d05fd5e6e`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 1.7 MB (1711801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d47cbc9449ef4aab290c562e2d538c1152c89268a02bb026807264d1c3d6da`  
		Last Modified: Fri, 12 Nov 2021 21:25:49 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a654447725655854a94c8af1e17c61ba95c1eb179a627aa323bfd70bfbae408`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37ea41d54140ffa8bd23aed643abb1c33674378a426fcc23eaaf16206abb895`  
		Last Modified: Fri, 12 Nov 2021 21:33:45 GMT  
		Size: 12.2 MB (12162485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0211332e3aa29375fc8973eceaa4bdab1ec4141057d9e2f2f628008d98b9dc43`  
		Last Modified: Fri, 12 Nov 2021 21:33:43 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d08a2ac48b1586435ee12f795239ab77a3b4486d29a202f4da5948018368619`  
		Last Modified: Fri, 12 Nov 2021 21:34:19 GMT  
		Size: 14.3 MB (14251407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9993affd8ea3c8059555c53e282b4d832b6ac6e879eff9e828afa1fe92ddb7dc`  
		Last Modified: Fri, 12 Nov 2021 21:34:16 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608a16d64b1461c542629b26d003f115cfa42a0df07228b13fdf789e630c594`  
		Last Modified: Fri, 12 Nov 2021 21:34:16 GMT  
		Size: 17.9 KB (17936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3ab5eeb7b309233d434543281deeb15d64bced125c9ae834ef8dca432c924`  
		Last Modified: Fri, 12 Nov 2021 21:34:16 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495a9f184c6c52059b7b1533a603b8a94ea36719901d9a24deaf61347783e3ff`  
		Last Modified: Sat, 13 Nov 2021 14:37:56 GMT  
		Size: 474.0 KB (473966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fa4c54e99ecf4c67a563ac659782cb4aebe66a5a674bfa97700cea31bc5f88`  
		Last Modified: Sat, 13 Nov 2021 14:37:57 GMT  
		Size: 6.2 MB (6191464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17abf349f976aa322c1e5c9c6f79710643c33dd167ec8307c044c35c6a646ad4`  
		Last Modified: Sat, 13 Nov 2021 14:37:58 GMT  
		Size: 9.7 MB (9681402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d777e764e553ebad650e187b05c4ba94f27e9e434d69bc5620ef9928dc18097`  
		Last Modified: Sat, 13 Nov 2021 14:37:55 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23331667e3edcdf05a97d7e65114ee9f50441cf7f007e98e687e0676a59928ec`  
		Last Modified: Sat, 13 Nov 2021 14:37:55 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.3-fpm-alpine` - linux; 386

```console
$ docker pull joomla@sha256:43d3be7b30a5acc714a3c82d71fa7c1f3eadc310f277d91f98affce059cfdf91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48216814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ac977a58a6d83c319a71b48a07840e2a7ef6e1a90cdfa698379e1dc38086d79`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:47:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 00:47:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 00:47:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 00:47:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 00:47:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 00:47:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:53:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 02:53:40 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 02:53:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 02:53:40 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 02:54:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 02:54:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:11:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 03:11:08 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:11:09 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 03:11:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 03:11:10 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 03:11:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 03:11:11 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 03:11:11 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 03:11:12 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 11:01:22 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 13 Nov 2021 11:01:22 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 13 Nov 2021 11:01:24 GMT
RUN apk add --no-cache 	bash
# Sat, 13 Nov 2021 11:03:26 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 13 Nov 2021 11:03:26 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 11:03:26 GMT
ENV JOOMLA_VERSION=3.10.3
# Sat, 13 Nov 2021 11:03:27 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Sat, 13 Nov 2021 11:03:34 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 13 Nov 2021 11:03:34 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 13 Nov 2021 11:03:35 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 13 Nov 2021 11:03:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 11:03:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05111b719bf0e9c81182879ace55b68244fff3ccaacc6813f9ce740b1adf4d`  
		Last Modified: Sat, 13 Nov 2021 04:00:31 GMT  
		Size: 1.8 MB (1812696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f12e62d2679739a2acadab070b1c7d0f433a8a46d449147d00fa5c4aa0a8753`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3e1535943b040497915113f37b46a4ba0dc10f27aabcdb6dbf9d0b594ca8be`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab8474ee661848bf8f531b7bbcfab486faf0509cd9244e321cf0e38f54dde50`  
		Last Modified: Sat, 13 Nov 2021 04:11:01 GMT  
		Size: 12.2 MB (12162696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dec147342e7674851fb64552ceeafcf7f8f1922cef56550c3f5ce21bc77a240`  
		Last Modified: Sat, 13 Nov 2021 04:11:00 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa0647a109448d6cd3b151a2778f08cfe8b2edf28b0a395ba977faae63746df`  
		Last Modified: Sat, 13 Nov 2021 04:11:39 GMT  
		Size: 14.9 MB (14883860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a8e389d1e091cb01d4845b93af56962eca9ebd1ad66b50dc8a24caa7c1807c`  
		Last Modified: Sat, 13 Nov 2021 04:11:36 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18b0021f8ebd7561a4d8c96a54517c60bb53bf61b1b020ac2fa84f24c9b348f`  
		Last Modified: Sat, 13 Nov 2021 04:11:36 GMT  
		Size: 18.0 KB (18013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c45b722466bd7a45328f20f90e88a547bffb6d0dc07f3a6630fcdc5dad453`  
		Last Modified: Sat, 13 Nov 2021 04:11:36 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a17101920b09e440e8563f2c1a97d501d3a4e8b722efd6523c5cbc53f0aeee7`  
		Last Modified: Sat, 13 Nov 2021 11:10:56 GMT  
		Size: 502.0 KB (501992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2524915b82d11f1b2e353111c9ae9c43bfe85b04a88f59fc56dfcf44f9aa8a`  
		Last Modified: Sat, 13 Nov 2021 11:10:57 GMT  
		Size: 6.3 MB (6311233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975228d6e95965f8d6b4c1fe035ea8f5096388a41430e7061a31002560230734`  
		Last Modified: Sat, 13 Nov 2021 11:11:00 GMT  
		Size: 9.7 MB (9680821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7462f1db279abf31f0463cab5cbd7f0d968ef39f6ea8518ddf4424bd15994b9`  
		Last Modified: Sat, 13 Nov 2021 11:10:56 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bb4acd01be5ad90e52fd2e4fe1b9c794773dc996cba1e991eee7696b933ba4`  
		Last Modified: Sat, 13 Nov 2021 11:10:56 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.3-fpm-alpine` - linux; ppc64le

```console
$ docker pull joomla@sha256:036d44b19d1890a2a1f62770fdf6fa0b6e2f8a3826d44f6e44ef26aa725b269b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49000254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3986a5769d0777a5b6562b7b74e7206d157f2f0f2534f0b3dc027e750e7ffa7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:56:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 11:56:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 11:56:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 11:56:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 11:56:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 11:56:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 13:26:13 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 13:26:15 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 13:26:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 13:26:18 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 13:26:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 13:26:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 13:36:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 13:36:15 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 13:36:26 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 13:36:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 13:36:31 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 13:36:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 13:36:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 13:36:46 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 13:36:48 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 20:54:46 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 13 Nov 2021 20:54:48 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 13 Nov 2021 20:54:53 GMT
RUN apk add --no-cache 	bash
# Sat, 13 Nov 2021 20:57:26 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 13 Nov 2021 20:57:28 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 20:57:30 GMT
ENV JOOMLA_VERSION=3.10.3
# Sat, 13 Nov 2021 20:57:32 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Sat, 13 Nov 2021 20:57:43 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 13 Nov 2021 20:57:47 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 13 Nov 2021 20:57:47 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 13 Nov 2021 20:57:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 20:57:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf526002982778a0157923a6219fbadd645d22999e9251af0db89be07d002272`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.8 MB (1759206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b47bb623f5bce1748b7a2c4e16b2726478248c03150000de676a1020aaeada`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035bbd1b7db7792a68686cccf93b48bd273f6f89375962d7fae46bab690f7ac`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb7bf13616eac548bc57504d80d61badd8e660e33ac387d2bf645439c251c10`  
		Last Modified: Sat, 13 Nov 2021 14:16:44 GMT  
		Size: 12.2 MB (12162707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c695864b11e20cd00baa535a219ac1144da20c4b0e627d2fd3b024597da273c2`  
		Last Modified: Sat, 13 Nov 2021 14:16:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4249da2901452eba6d7afae20b44402247095824e415dc06a5cded9b313e2e`  
		Last Modified: Sat, 13 Nov 2021 14:17:20 GMT  
		Size: 15.6 MB (15632091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1403896f2de2978a501451650047ac3f1117a700915e72f5ff4af38ad72e8650`  
		Last Modified: Sat, 13 Nov 2021 14:17:17 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4539e880e72603b72052e5072357de966697dce3258d81db9ed1ce274baee5`  
		Last Modified: Sat, 13 Nov 2021 14:17:17 GMT  
		Size: 18.0 KB (18030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf3bdcea270e6d1bc856d3e21e43b9020bf5d3a333f77c09acb267df2f72be4`  
		Last Modified: Sat, 13 Nov 2021 14:17:17 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8709a64d4d4db27cbbade897564676dbe89dc0391aa7bf04b460aa9f7c0dc21c`  
		Last Modified: Sat, 13 Nov 2021 21:04:24 GMT  
		Size: 529.9 KB (529946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f496d26a15f679c151cb924582cbe8059cf14798fead9648490e172e65ee27ad`  
		Last Modified: Sat, 13 Nov 2021 21:04:25 GMT  
		Size: 6.4 MB (6385411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d864f4aaf76589138c246a780bfdefe46a4d04c7f00453e1985ced6d8bb8d`  
		Last Modified: Sat, 13 Nov 2021 21:04:26 GMT  
		Size: 9.7 MB (9680835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8eb458d1e1dba10b68d18558b6c9e433be6f3238feb476237503f98fe7b55`  
		Last Modified: Sat, 13 Nov 2021 21:04:24 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ab7aacff308ce47eeb0af71062f49ae8cc995abe6bb4b332d94839be839b13`  
		Last Modified: Sat, 13 Nov 2021 21:04:24 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:3-php7.3-fpm-alpine` - linux; s390x

```console
$ docker pull joomla@sha256:47930852b4624ba12317a2937a6bde80a3d98c0482a614a99a9618c70313e568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46577336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bedded1316f2419988db39353983101047b4814e188315522a880a2b782a859`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:58:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:58:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:58:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:58:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:58:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:44:14 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 18 Nov 2021 16:42:57 GMT
ENV PHP_VERSION=7.3.33
# Thu, 18 Nov 2021 16:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Thu, 18 Nov 2021 16:42:57 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Thu, 18 Nov 2021 16:43:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:43:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:48:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:48:30 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:48:31 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:48:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:48:31 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:48:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:48:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:48:31 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:48:32 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 18:29:41 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 18 Nov 2021 18:29:41 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 18 Nov 2021 18:29:42 GMT
RUN apk add --no-cache 	bash
# Thu, 18 Nov 2021 18:30:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		libjpeg-turbo-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install mcrypt-1.0.4; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		mcrypt 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 18 Nov 2021 18:30:51 GMT
VOLUME [/var/www/html]
# Thu, 18 Nov 2021 18:30:51 GMT
ENV JOOMLA_VERSION=3.10.3
# Thu, 18 Nov 2021 18:30:51 GMT
ENV JOOMLA_SHA512=1843595b67ee594038418efb570d2bac2e92b0f1907ead6c6d8c4cf1a547d93181358be458ce6d0a7879b9bb9d6d0f683b0f5507e345be5ee24c993bed614fe5
# Thu, 18 Nov 2021 18:30:55 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 18 Nov 2021 18:30:56 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 18 Nov 2021 18:30:57 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 18 Nov 2021 18:30:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 18:30:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6db577f243875f52f246d8a7fdab675a850569d52d6bba314f58258225c1f`  
		Last Modified: Fri, 12 Nov 2021 21:10:48 GMT  
		Size: 1.8 MB (1774038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472bfa2a1552842a7406f914151af808b4f2a9e245ddbfe7cbc332697f96b12`  
		Last Modified: Fri, 12 Nov 2021 21:10:47 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3cea1835285017465c0df7a510c36971229f7066ec32d2ac436c4f9ac6ebd3`  
		Last Modified: Fri, 12 Nov 2021 21:10:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a8b23accf2e713f723d25ee53c852a7ce60f61c347f04199e45cb7af5d2777`  
		Last Modified: Thu, 18 Nov 2021 17:17:33 GMT  
		Size: 12.2 MB (12164214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d775cdd6ca223afb41b6c314f69687244d511176e9243c76d67e582c3f564f0`  
		Last Modified: Thu, 18 Nov 2021 17:17:32 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06cf9eeb9fa7814535e3bd75884682a6741b25efe7ce756ca15ad9f88637495`  
		Last Modified: Thu, 18 Nov 2021 17:17:55 GMT  
		Size: 13.9 MB (13937848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fc53ac641fae493e75f82713e1414496fe6c88ff4db98b3528cfd35c274358`  
		Last Modified: Thu, 18 Nov 2021 17:17:53 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42657c24235cb1ecf217395255b610f86b5492a436065d6c9475309f1a40e36`  
		Last Modified: Thu, 18 Nov 2021 17:17:53 GMT  
		Size: 18.0 KB (18037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d7025d91ca16580175d6aa336d586ab004c64876b2f053c7026c8899ca873`  
		Last Modified: Thu, 18 Nov 2021 17:17:53 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8abc15217e7f19ed8f852c8b28802eb4772123f2fc89f9c2803244d66c624a`  
		Last Modified: Thu, 18 Nov 2021 18:39:17 GMT  
		Size: 483.1 KB (483058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80fa8c65eb1ae7208a1ba0eb7c7170c846f1fc15b2935acf896f7b4ca995e0a`  
		Last Modified: Thu, 18 Nov 2021 18:39:18 GMT  
		Size: 5.9 MB (5895494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d025f72de5099676c04d6f6c762269b9b7cd3651fd79f7583e4f516de75bdf`  
		Last Modified: Thu, 18 Nov 2021 18:39:19 GMT  
		Size: 9.7 MB (9680819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5efd4e38e77d894183a49e7e3afff08f944d08f639eafb72be5cff05af7dbd`  
		Last Modified: Thu, 18 Nov 2021 18:39:17 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1549aa0151eace20930856e8449efedf4c44f724faa595b8eb2764f6bab07ebb`  
		Last Modified: Thu, 18 Nov 2021 18:39:17 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
