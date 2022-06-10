## `joomla:4-php7.4-fpm-alpine`

```console
$ docker pull joomla@sha256:f2e6e69bc2d1c6ab19aa5190583b4ee992bdca4fa89c99094379acda06ddb1e0
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

### `joomla:4-php7.4-fpm-alpine` - linux; amd64

```console
$ docker pull joomla@sha256:7cbfd7f46b5e1bf9805953aac1bed1a6b0dbe78aaf30b74d21ca32857ff8559b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58585677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b34f06c3d7c69a61b010ac79c812d5bf0aee0dc8af68b4306a5434023d58c6e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:48:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:48:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:48:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:48:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:48:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:13:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 25 May 2022 20:13:28 GMT
ENV PHP_VERSION=7.4.29
# Wed, 25 May 2022 20:13:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 25 May 2022 20:13:28 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 25 May 2022 20:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 20:13:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:20:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:20:36 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:20:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:20:36 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:20:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:20:37 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:20:37 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:20:37 GMT
CMD ["php-fpm"]
# Wed, 25 May 2022 23:58:41 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 25 May 2022 23:58:41 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 25 May 2022 23:58:42 GMT
RUN apk add --no-cache 	bash
# Thu, 26 May 2022 00:00:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 26 May 2022 00:00:23 GMT
VOLUME [/var/www/html]
# Fri, 27 May 2022 21:20:22 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 27 May 2022 21:20:22 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 27 May 2022 21:20:28 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 27 May 2022 21:20:29 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 27 May 2022 21:20:29 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 27 May 2022 21:20:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 May 2022 21:20:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5ea1cb188409ac6276c7e55f3a6f6b0dfe9e3bd72711881e32183f03e8d99`  
		Last Modified: Wed, 25 May 2022 20:28:12 GMT  
		Size: 1.7 MB (1704858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3935ba60366aecf1bc3d1f0c663cb07711d490232ffa0ddde876eb4ebc40e469`  
		Last Modified: Wed, 25 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4712e34f1d293d5afd1871939afc2d84d672bf03d6c4ef9c9558c720f40e5195`  
		Last Modified: Wed, 25 May 2022 20:28:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38485f657c58ee91f6c189b3bdea5474a8b422a345a873d02f1396365d89661e`  
		Last Modified: Wed, 25 May 2022 20:31:43 GMT  
		Size: 10.4 MB (10438817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a057edf730b8f519da35397ff5ac709dcf1510cb864654b4b01027aa7a800`  
		Last Modified: Wed, 25 May 2022 20:31:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a807c9e52ca2fa74c8e47488491871e72349e2d9eede098686df8a3c1d3436`  
		Last Modified: Wed, 25 May 2022 20:32:24 GMT  
		Size: 11.5 MB (11456109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739d534fe3d2562599fd67e81bd7a08fb68730961265104663ff3e4282813204`  
		Last Modified: Wed, 25 May 2022 20:32:22 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbf04586c85ad49f30a1723bfed8282119a852d09ec742810d62527f2574c6`  
		Last Modified: Wed, 25 May 2022 20:32:22 GMT  
		Size: 18.4 KB (18361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a5c3c60b568f02c603d4af0daea625842e819f74cab44015714f61a2387a28`  
		Last Modified: Wed, 25 May 2022 20:32:22 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f4e1d338e7529727ed539497161cdf85747ee31c18f866405940a7d8b43c7`  
		Last Modified: Thu, 26 May 2022 00:08:13 GMT  
		Size: 466.9 KB (466899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7c1addba0aa1d7cb4b8b9517bf2bbe4c3afbcffb67fb25fe947d72a75853cd`  
		Last Modified: Thu, 26 May 2022 00:08:14 GMT  
		Size: 9.6 MB (9611994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d44dd10c45013a8abd9522e7265ba44658ee5786c958e97aa9e0a9643205735`  
		Last Modified: Fri, 27 May 2022 21:23:06 GMT  
		Size: 22.1 MB (22074398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10140feeb37855c71768db3a07b107fc4c19862e2c4607eb26f3e051dee86d1d`  
		Last Modified: Fri, 27 May 2022 21:23:02 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971596700a9484e69b3684b9265ed085213f6643972167154146c3b1998ba056`  
		Last Modified: Fri, 27 May 2022 21:23:02 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull joomla@sha256:aeff690e6ef377ecd18356b5457b912cc9f4c3930d00ea92119f1436766c43a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.9 MB (56856164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f3f0c79e436bd62d946da0f40cb95514160e8df13f74379f62dd0e7b04d407`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 21:50:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 21:50:07 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 21:50:08 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 21:50:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 21:50:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 22:22:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 22:58:01 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 22:58:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 22:58:02 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 22:58:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 09 Jun 2022 22:58:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:08:50 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:08:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:08:54 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:08:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 09 Jun 2022 23:08:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 09 Jun 2022 23:08:56 GMT
EXPOSE 9000
# Thu, 09 Jun 2022 23:08:57 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 00:50:22 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 10 Jun 2022 00:50:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 10 Jun 2022 00:50:25 GMT
RUN apk add --no-cache 	bash
# Fri, 10 Jun 2022 00:55:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 10 Jun 2022 00:55:10 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 00:55:11 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 10 Jun 2022 00:55:11 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 10 Jun 2022 00:55:31 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 10 Jun 2022 00:55:33 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 10 Jun 2022 00:55:33 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 10 Jun 2022 00:55:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 00:55:34 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e7eae6d0293087d982d321125f6f132894675f6acb732427528058758d6ae3`  
		Last Modified: Wed, 25 May 2022 22:46:23 GMT  
		Size: 1.7 MB (1693282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad96c7e3fdd13c53c906a10fab89b0dc599bf1746acd163f9648f8f9ec949de`  
		Last Modified: Wed, 25 May 2022 22:46:21 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1acccbd45290b92307c479937198ace1c187e0fd49d5e1ea72c1f5d7d5e1705`  
		Last Modified: Wed, 25 May 2022 22:46:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018c479e11e460f769a664e3d035a1f58d48a6be9217bc267fee2a7cef56050`  
		Last Modified: Thu, 09 Jun 2022 23:48:06 GMT  
		Size: 10.4 MB (10439063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aeb9e0c79391e9b7c9159709b06e5dd6a0f62ec37e73b8d3fbc62cd4a2a48f`  
		Last Modified: Thu, 09 Jun 2022 23:48:03 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e3e1b803bf466b610fbb5b5921e6570698030260083ab1844adcf5532a736f`  
		Last Modified: Thu, 09 Jun 2022 23:49:12 GMT  
		Size: 10.7 MB (10723649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fcd8d9973bbd18794af50980e0da190e9c43931665f6af20336dac238148d2`  
		Last Modified: Thu, 09 Jun 2022 23:49:04 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd669e83bb0d365f9d91d6e0f37d6669f957ce989ae48671a92356df7d23d83`  
		Last Modified: Thu, 09 Jun 2022 23:49:05 GMT  
		Size: 18.4 KB (18367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78e3e097ca61f322cc47921b13a7fa52203d6b6b314b41abc98de138b234c7`  
		Last Modified: Thu, 09 Jun 2022 23:49:04 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef95a7833655d02823e64be70f89c573c9276960407aa582b7bfecde7abc43e`  
		Last Modified: Fri, 10 Jun 2022 01:13:03 GMT  
		Size: 454.3 KB (454293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49687f44812a818f749871c84e44e41eafff322ebf1214b7d4cf9912ae460fd2`  
		Last Modified: Fri, 10 Jun 2022 01:13:06 GMT  
		Size: 8.8 MB (8831597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42356306c47c1de659f94a4848c08301e141cd1fdf5497aa801e168a56be278a`  
		Last Modified: Fri, 10 Jun 2022 01:13:14 GMT  
		Size: 22.1 MB (22074414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554e5d7494e4d087ded5602c55f0eb008fd65a2b0ee388844f827213ef22a1bb`  
		Last Modified: Fri, 10 Jun 2022 01:13:03 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d8bbf408d41e53d4164703aff8189e18cfbfda7d7d83287b3ebbf5a4664437`  
		Last Modified: Fri, 10 Jun 2022 01:13:03 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull joomla@sha256:9f45ad0c8a049e71eec84c06cb3a9cbba087de6942f02acc3ef3d3c15fde1505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55734384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e9b6b52ed85e87984f3276fa16e85aa1e7df56d173bc217b969185dad8c0f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:01:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:01:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:01:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:01:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:01:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:36:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 25 May 2022 19:36:20 GMT
ENV PHP_VERSION=7.4.29
# Wed, 25 May 2022 19:36:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 25 May 2022 19:36:21 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 25 May 2022 19:36:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 19:36:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 19:46:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 19:46:05 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 19:46:07 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 19:46:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 19:46:08 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 19:46:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 19:46:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 19:46:11 GMT
EXPOSE 9000
# Wed, 25 May 2022 19:46:11 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 03:30:40 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 26 May 2022 03:30:41 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 26 May 2022 03:30:43 GMT
RUN apk add --no-cache 	bash
# Thu, 26 May 2022 03:35:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 26 May 2022 03:35:13 GMT
VOLUME [/var/www/html]
# Fri, 27 May 2022 20:58:49 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 27 May 2022 20:58:49 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 27 May 2022 20:59:08 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 27 May 2022 20:59:10 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 27 May 2022 20:59:10 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 27 May 2022 20:59:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 May 2022 20:59:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68c4c667bd6865eca9aa9f496ecc527223b3162b260cad2e40c45ad49edc479`  
		Last Modified: Wed, 25 May 2022 20:09:19 GMT  
		Size: 1.6 MB (1560829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6bb9188dd796f59353a38be6412d00920f7c1da1effa359dc5c9a5724c0fb0`  
		Last Modified: Wed, 25 May 2022 20:09:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbde557014a2ec2c7a2e22a836cdf6978cf4aaea9b738859980a1d98c9b1282`  
		Last Modified: Wed, 25 May 2022 20:09:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02954cc670b8f5240fd2c85d77660674e7b2b47ed0fd55e4b5f967b7020fa768`  
		Last Modified: Wed, 25 May 2022 20:15:58 GMT  
		Size: 10.4 MB (10438808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61272aa02c2af4b15db30085c8e6ca18d250a7d5f61a21118e6e12413420d940`  
		Last Modified: Wed, 25 May 2022 20:15:56 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5bc9cdf26b7873e8dcae3795c8b5c051569822a35c3065c7359843c0197e36`  
		Last Modified: Wed, 25 May 2022 20:17:03 GMT  
		Size: 10.1 MB (10089758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64db602bc2640a74d8e1d596834e697242912a29f8b2d4045522961c6fbea1`  
		Last Modified: Wed, 25 May 2022 20:16:56 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922690085ee34bb8ef6468d2232dec76fe98c0c9000e25f8468aa3259e9102f2`  
		Last Modified: Wed, 25 May 2022 20:16:56 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca53ed35885b2d353e752bfc5f0cb6cbe18e6133cd599dbb4e8a48e055283427`  
		Last Modified: Wed, 25 May 2022 20:16:56 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77651c1bb5bffaeac4af989d77524c65013c2dacb5885478289bdc1f894c991`  
		Last Modified: Thu, 26 May 2022 03:57:32 GMT  
		Size: 414.8 KB (414821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0516469824e265e809c8d163f9b54b65429a5bf7695111da1473df697c771e`  
		Last Modified: Thu, 26 May 2022 03:57:36 GMT  
		Size: 8.7 MB (8710426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43eec1280721fb393a97fd17cd828524007bb90b0b81b62b68d86aebdfefc8f9`  
		Last Modified: Fri, 27 May 2022 21:10:15 GMT  
		Size: 22.1 MB (22074395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cea3ae8f1e5847f81039f6c1f64b68c2485c9076d2aa8ec1c8b66ed800f5d5`  
		Last Modified: Fri, 27 May 2022 21:09:55 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474ac46bded0e2ed85a8e5d7db08da0f88194361a9a4d931b68f9b674619e5ac`  
		Last Modified: Fri, 27 May 2022 21:09:56 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:ef99edefa2a40a958009e5137840c15872e58320753fa8d55fd82498478206f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58243209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec9bbf2db1c9b7ac188797d599360f300d7de6ef526c99094e27295e63df8144`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:06:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 20:06:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 20:06:20 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 20:06:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 20:06:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 20:06:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 21:02:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 25 May 2022 21:02:56 GMT
ENV PHP_VERSION=7.4.29
# Wed, 25 May 2022 21:02:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 25 May 2022 21:02:58 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 25 May 2022 21:03:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 21:03:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 21:15:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 21:15:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 21:15:15 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 21:15:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 21:15:17 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 21:15:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 21:15:19 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 21:15:20 GMT
EXPOSE 9000
# Wed, 25 May 2022 21:15:21 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 00:53:07 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 26 May 2022 00:53:08 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 26 May 2022 00:53:10 GMT
RUN apk add --no-cache 	bash
# Thu, 26 May 2022 00:55:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 26 May 2022 00:55:08 GMT
VOLUME [/var/www/html]
# Fri, 27 May 2022 21:40:26 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 27 May 2022 21:40:27 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 27 May 2022 21:40:34 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 27 May 2022 21:40:36 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 27 May 2022 21:40:37 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 27 May 2022 21:40:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 May 2022 21:40:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a240d0a51bf6100803c8ce9f1ce769377fd09a2824a580ad991fb1a8a64610`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 1.7 MB (1703255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d989eb157716fb2e84408b95764324504b7dd9aac628dd9a66a7f15eeb43a66`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940028d0e55a77f4d9df2de18c1a76fa1058bdb66dee66fa6309f9337e500d6e`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79204fbd3f89c75048ba1f710c653426630d4f42fe5c43440ade502f24df49a`  
		Last Modified: Wed, 25 May 2022 21:31:03 GMT  
		Size: 10.4 MB (10438582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ef3bf440ec26105084aed8908902a0536f16fd590a7db56fc1cc32802b4007`  
		Last Modified: Wed, 25 May 2022 21:31:02 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c428a2c9f0656f509527ad7cda74d6da82f5beb7a26b676223dabd239105e8`  
		Last Modified: Wed, 25 May 2022 21:31:48 GMT  
		Size: 11.3 MB (11284103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb69e98fda850c8e4ff1c67afdc455eea522d087fae14f3930ef222089f62c6`  
		Last Modified: Wed, 25 May 2022 21:31:46 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039937e24cc43eb48fb4bf0901d45bd7a89e534f43cf567158b8ffd308f7992a`  
		Last Modified: Wed, 25 May 2022 21:31:46 GMT  
		Size: 18.3 KB (18253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c5fa133d62d63605d9307c3159f95e4b407536d6fdf65b89a286ea4ff4c2f`  
		Last Modified: Wed, 25 May 2022 21:31:47 GMT  
		Size: 8.4 KB (8440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f818a15af5b0aad203fc754fb487564d7629d21d6fec0669f6a6c3aa42bd45`  
		Last Modified: Thu, 26 May 2022 01:08:52 GMT  
		Size: 473.5 KB (473543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ab83c054d2538f1e65c6b7eff95818be5c1c158fe5a0f3c48d6ee224d00b9f`  
		Last Modified: Thu, 26 May 2022 01:08:53 GMT  
		Size: 9.5 MB (9541616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da637a94f7858ba885940bce3a24e00245063d0c7f4f6bfa3529f7e1141b4d3`  
		Last Modified: Fri, 27 May 2022 21:45:30 GMT  
		Size: 22.1 MB (22074115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f75d68c395cff0d56db4cceb309d787af741e996b2b15e866663e867d6ff37b`  
		Last Modified: Fri, 27 May 2022 21:45:26 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d945e04d52a2fb0f20064821d5cb26a281b222cca996a4867b97fa6d014496`  
		Last Modified: Fri, 27 May 2022 21:45:26 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; 386

```console
$ docker pull joomla@sha256:7bb86cbef9407e0ea9a221161d8b67c2a011299b08ce52127e67bb8ac31c0885
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59240997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79387bc23b228a75c72a3ab70795611e62e9421156ffe1230b73cdf5f30c6bd9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:56:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:56:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:56:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:56:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:56:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:56:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:23:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 25 May 2022 20:23:46 GMT
ENV PHP_VERSION=7.4.29
# Wed, 25 May 2022 20:23:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 25 May 2022 20:23:48 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 25 May 2022 20:23:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 20:23:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:31:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:31:14 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:31:14 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:31:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:31:16 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:31:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:31:18 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:31:19 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:31:20 GMT
CMD ["php-fpm"]
# Wed, 25 May 2022 23:36:46 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 25 May 2022 23:36:47 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 25 May 2022 23:36:49 GMT
RUN apk add --no-cache 	bash
# Wed, 25 May 2022 23:38:35 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Wed, 25 May 2022 23:38:35 GMT
VOLUME [/var/www/html]
# Fri, 27 May 2022 21:39:04 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 27 May 2022 21:39:05 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 27 May 2022 21:39:13 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 27 May 2022 21:39:15 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 27 May 2022 21:39:16 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 27 May 2022 21:39:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 May 2022 21:39:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eb700ff81c1dbea3f8e204a809be7b7431ba817b16c87c1efe84972e2fe6c1`  
		Last Modified: Wed, 25 May 2022 20:43:18 GMT  
		Size: 1.8 MB (1807504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaabb95698f746340e8771d50f4e356e03ad67347638c9d30dc7d3d7cdb3359`  
		Last Modified: Wed, 25 May 2022 20:43:18 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f127678bc84e9717b47e929fd82c70e9bc39b96e731eb561d466d4373561cd1`  
		Last Modified: Wed, 25 May 2022 20:43:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da884c158fed7b912ee52594f4f88d3eafe6744a7e66904b6bc4f57e59306c06`  
		Last Modified: Wed, 25 May 2022 20:47:44 GMT  
		Size: 10.4 MB (10438567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9802c8814d43788b8b51cc934a29da5fdbeff14e342219f19c0b84f875d15c`  
		Last Modified: Wed, 25 May 2022 20:47:41 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074de331469ea4bbf9f3d265aa54ef345ff3b93324d009558f6a395fe4d8710`  
		Last Modified: Wed, 25 May 2022 20:48:28 GMT  
		Size: 11.8 MB (11764487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09af158595ec60196fd004aa8b29063b9b5e472c492ac77a767b40441c4589d8`  
		Last Modified: Wed, 25 May 2022 20:48:26 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2674c8c0fc6ec334dca9d4a16523139c87fee4dff4a72516f8a511099a637`  
		Last Modified: Wed, 25 May 2022 20:48:26 GMT  
		Size: 18.3 KB (18258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a234743a1f339033602f97a5278a786870f674985c4972a678030af976345b64`  
		Last Modified: Wed, 25 May 2022 20:48:27 GMT  
		Size: 8.4 KB (8440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5da2a68a186c599561bdab41b3c3365555676d7e078d94a24ab2a46634d8af`  
		Last Modified: Wed, 25 May 2022 23:48:07 GMT  
		Size: 503.5 KB (503500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17f208bf4a89ac0aba5bd57826202694427cbe2d909dc7eb68582f6ce3e2a6`  
		Last Modified: Wed, 25 May 2022 23:48:08 GMT  
		Size: 9.8 MB (9817405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c67c29526c9f16c277d1e2a70a105f8b0d848606ecf16fdb1382d8bfd86d19`  
		Last Modified: Fri, 27 May 2022 21:44:27 GMT  
		Size: 22.1 MB (22074113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d60d1fb28c64bbc901ebe95add27dd3f43cc4f83d32a389611fca1c52d79c4a`  
		Last Modified: Fri, 27 May 2022 21:44:23 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27113b97e972ec4ece9cc94546d3afee3de23864c139206152b43318fb1e1ef`  
		Last Modified: Fri, 27 May 2022 21:44:23 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; ppc64le

```console
$ docker pull joomla@sha256:e4b676855dea7d2a303d02b0111747415bfd1608331e76bb9cb63ced0a8e6160
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59669095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa2ebaa8bda7d04c32dab134665c8a74903f3a306481118b94e04b4276f7639`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:57:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:57:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:57:43 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:57:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:57:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:57:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:57:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:57:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:39:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 25 May 2022 20:39:33 GMT
ENV PHP_VERSION=7.4.29
# Wed, 25 May 2022 20:39:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 25 May 2022 20:39:39 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 25 May 2022 20:43:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 20:43:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:54:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:54:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:54:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:54:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:54:32 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:54:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:54:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:54:42 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:54:45 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 02:39:55 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 26 May 2022 02:40:01 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 26 May 2022 02:40:17 GMT
RUN apk add --no-cache 	bash
# Thu, 26 May 2022 02:43:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 26 May 2022 02:43:26 GMT
VOLUME [/var/www/html]
# Fri, 27 May 2022 21:25:51 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 27 May 2022 21:25:54 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 27 May 2022 21:26:09 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 27 May 2022 21:26:12 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 27 May 2022 21:26:14 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 27 May 2022 21:26:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 May 2022 21:26:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091cbad9101b41d3fd65de74d3265b02346722f13f77c4a456e33979dd226da`  
		Last Modified: Wed, 25 May 2022 21:08:36 GMT  
		Size: 1.8 MB (1759345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e34510ef12ed73f2ed4ab7167c3408a7a0c69498928d0be0c6d46e2250ea3`  
		Last Modified: Wed, 25 May 2022 21:08:35 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbd0bbe87c55d5c71424cd10832856ec6580b2de2bf35112f9a41f574cef70f`  
		Last Modified: Wed, 25 May 2022 21:08:35 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782b33dbbd3bb1ce9d9a9f2c8631a1fb15a99edb0550457afb10267afa47b9f3`  
		Last Modified: Wed, 25 May 2022 21:13:20 GMT  
		Size: 10.4 MB (10438821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30069aee361914d9f9fd340a64b28541bdb4f5ba17c50a7bd07445e0f930a030`  
		Last Modified: Wed, 25 May 2022 21:13:19 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f779e4206091950579168e34b7c331b69389cfb6d7f4e9ad6551b4c635cba381`  
		Last Modified: Wed, 25 May 2022 21:14:13 GMT  
		Size: 12.2 MB (12216252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb07921867d8afdb49f4d544e8570627e5e1823c48c67a86b7a3c8f62d49636`  
		Last Modified: Wed, 25 May 2022 21:14:11 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c732eca29eb26e2c5f38434403262d4e12de5433940641b4dcde22d9651c133`  
		Last Modified: Wed, 25 May 2022 21:14:11 GMT  
		Size: 18.3 KB (18347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85595200d280a23deb9d36dfd2923ba4a6ce9c8253d0be121912e316a78218cd`  
		Last Modified: Wed, 25 May 2022 21:14:11 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ffbc870b6474e82da42aa1bacf0952019eb508ad840307af972a69fc4123a7`  
		Last Modified: Thu, 26 May 2022 03:01:02 GMT  
		Size: 533.7 KB (533675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2104d08e7e3b699adce7db2bf5f4c1292f42e0641250966be80e866059d92`  
		Last Modified: Thu, 26 May 2022 03:01:04 GMT  
		Size: 9.8 MB (9823157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac305735e3710b8eed676a2380d01106a204592b46722de902f731353486e2b3`  
		Last Modified: Fri, 27 May 2022 21:34:18 GMT  
		Size: 22.1 MB (22074387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a9982436b07e38bc179feedadcbd2b257ce73593c75a0399dc13279503cd38`  
		Last Modified: Fri, 27 May 2022 21:34:13 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c12798ba9ac3f5d1e562f9a62498303ff311dcc3bfab833885dcdbe37e64b4`  
		Last Modified: Fri, 27 May 2022 21:34:13 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; s390x

```console
$ docker pull joomla@sha256:164ecb8951b6e9919df602349a6b2ccb33e06b83398253e18a4652fb3886c789
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57656470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2e1ced289b10122372cbb7c051e2846298c2ca93014cf36015f12ed2a5a7e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:06:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 20:06:39 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 20:06:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 20:06:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 20:06:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 20:06:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:49:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 25 May 2022 20:49:06 GMT
ENV PHP_VERSION=7.4.29
# Wed, 25 May 2022 20:49:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 25 May 2022 20:49:07 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 25 May 2022 20:49:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 20:49:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:58:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:58:58 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:58:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:58:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:59:00 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:59:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:59:01 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:59:02 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:59:02 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 00:27:14 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 26 May 2022 00:27:15 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 26 May 2022 00:27:16 GMT
RUN apk add --no-cache 	bash
# Thu, 26 May 2022 00:28:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 26 May 2022 00:28:55 GMT
VOLUME [/var/www/html]
# Fri, 27 May 2022 21:42:26 GMT
ENV JOOMLA_VERSION=4.1.4
# Fri, 27 May 2022 21:42:27 GMT
ENV JOOMLA_SHA512=a9ffd64d8320d3df2f58df924b750f4b75a15eac194b4a8ef98671208ad2ca8a09a3ea6d55cce51eceded89eae7d6252ba64057b3e12ef88bc75a43d7ee6d70d
# Fri, 27 May 2022 21:42:46 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 27 May 2022 21:42:55 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 27 May 2022 21:42:56 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 27 May 2022 21:42:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 May 2022 21:42:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad757c376420c4bd689dd2059809802df6400dc63a1f808ebb6ca69780724e3`  
		Last Modified: Wed, 25 May 2022 21:13:30 GMT  
		Size: 1.8 MB (1765925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ece50bae8c0ec9d3501fc804150b9b5ad9fe9187347f2304690718df868b540`  
		Last Modified: Wed, 25 May 2022 21:13:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992853a158bd58244683eefc2e1a8c73fa903949f9422c6c9f2d55a4a83fc0f3`  
		Last Modified: Wed, 25 May 2022 21:13:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3ac7a79e5ce20c78a4ea5250ddfb568aaad254b411f4fea63e3c1ca05afd10`  
		Last Modified: Wed, 25 May 2022 21:17:16 GMT  
		Size: 10.4 MB (10438832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de31b7fb7e7b94f66292f1ac0687deed68d8d212bdb4dcce9d6a68609b05f62`  
		Last Modified: Wed, 25 May 2022 21:17:16 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82786633011ce3915a87d64dc43eb77df5fa99ae7a52b9eeedc427ed0964f9bc`  
		Last Modified: Wed, 25 May 2022 21:17:48 GMT  
		Size: 11.0 MB (11049482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34608c6a3c0fd1a652cdc8fab274ee0820f0daa2aa6b0d6ce375923118b6e143`  
		Last Modified: Wed, 25 May 2022 21:17:46 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8da7fe6cc9b2fe4fc239c8e73097130f1ecca381fd74009210dd5ddd2ded3be`  
		Last Modified: Wed, 25 May 2022 21:17:46 GMT  
		Size: 18.4 KB (18373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d879266c5d9f0c59b2005b634ca78ba47904132c35b21f73c5a5fd6d309b36f4`  
		Last Modified: Wed, 25 May 2022 21:17:46 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15677b79f0bf9bec676c43c1a5a5e871315e5018cca18edf6662e0b981302cb9`  
		Last Modified: Thu, 26 May 2022 00:42:00 GMT  
		Size: 483.6 KB (483586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e15caf049bc1205a9c821a3fab64bb143dc5414cee1167d93ecefa800c591`  
		Last Modified: Thu, 26 May 2022 00:42:01 GMT  
		Size: 9.2 MB (9230029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62f441f8b86a55539552f21cb7ad8ad446733f1b9ee8cae4aad8cea66200f4c`  
		Last Modified: Fri, 27 May 2022 21:50:36 GMT  
		Size: 22.1 MB (22074396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b4263cb22957ba72b2a75cc818e3298b163df926a53c69d12ce9eb6782a4c4`  
		Last Modified: Fri, 27 May 2022 21:50:33 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd264e748ebbb8b5374aa9428e7c26245a3c2c9e39b788c8b3a18cd3623b7864`  
		Last Modified: Fri, 27 May 2022 21:50:33 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
