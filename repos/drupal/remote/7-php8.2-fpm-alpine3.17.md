## `drupal:7-php8.2-fpm-alpine3.17`

```console
$ docker pull drupal@sha256:2bec3d33405ea590bc2e74b4c506f1abda0b316eb1212a80714ab32fdf2b5995
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `drupal:7-php8.2-fpm-alpine3.17` - linux; amd64

```console
$ docker pull drupal@sha256:16ba76079fec7ab004177559ba582e6dcb573493b531fd906aa1a1949069cffc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40367930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ccd3b87ac9bfab9327a4d5a67c719a2cf65be1f789a33610f14203bcfad6e4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.12
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d409140a81c62f46aeb13593b4f71d44dfe26018d27aea968ccc0cf37ca63f0a`  
		Last Modified: Sat, 21 Oct 2023 06:27:11 GMT  
		Size: 4.0 MB (3966868 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3d975c886325f4cd819965bbfa3ee3a41d8635acbe5586307d01fd95204774c`  
		Last Modified: Sat, 21 Oct 2023 06:27:10 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:28c6b16bc660c086b6f1cb34456d304fa1062c10b31c12d3e0ac129b0f78b112`  
		Last Modified: Sat, 21 Oct 2023 06:27:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:254db1a99a01494a3260f2a65c704d743a92744ee50d4c4da8f1c2109de04772`  
		Last Modified: Sat, 28 Oct 2023 03:40:40 GMT  
		Size: 12.1 MB (12069504 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:724ca2f93768ef1b3252fa0816d3dddedd057ea145381073c10af1cb62bc522a`  
		Last Modified: Sat, 28 Oct 2023 03:40:38 GMT  
		Size: 495.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5395030a363f6119968034a611caae8692ebafec86f827fd67e089c1b5cde1c6`  
		Last Modified: Sat, 28 Oct 2023 03:41:06 GMT  
		Size: 15.3 MB (15301000 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:500beca1d3666ed8447bfb2814400c2634023bc8f038f10c1351c529126fbe41`  
		Last Modified: Sat, 28 Oct 2023 03:41:04 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e92bda9730d174def48456ff6014326cbaec83a2c99e7ea3017642c2b7de76ef`  
		Last Modified: Sat, 28 Oct 2023 03:41:04 GMT  
		Size: 19.0 KB (18985 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64b9b3cae24e816e821f27ce1295de2c0619b80be19aa3ca13456cd6e4e4cc54`  
		Last Modified: Sat, 28 Oct 2023 03:41:04 GMT  
		Size: 9.2 KB (9174 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:250daeb3689e0668559e3be7957af799c77e8dfc75a76b2c4811cfa6850e85bd`  
		Last Modified: Wed, 08 Nov 2023 20:25:40 GMT  
		Size: 2.2 MB (2208708 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3b82dcfc3d1456dccafdfe7f76353077f22073e40d09be281ce6881320c91ea`  
		Last Modified: Wed, 08 Nov 2023 20:25:40 GMT  
		Size: 311.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:11ae1cfc3efa5ff561e277b6a7b840d1c40cc03611cff16488b86cb614d8e8ef`  
		Last Modified: Wed, 08 Nov 2023 20:25:40 GMT  
		Size: 3.4 MB (3410295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:62737d32e8706cae635e8128a4f53934a9238bfbc71c0ff247e9195d3e975ad6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.9 KB (254945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c8986edd46d052ae8aecb11de6ab22cee0b709bdb6aa195a79a78596f66a26`

```dockerfile
```

-	Layers:
	-	`sha256:90c440dcb5a9df8079d28cd491f50de0628dc646a4a5cb2ef4ad344159ef1038`  
		Last Modified: Wed, 08 Nov 2023 20:25:40 GMT  
		Size: 232.1 KB (232097 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbe2eb6189d93fa901707073d1b27005dde43a27d18bb7f5cccced264d127570`  
		Last Modified: Wed, 08 Nov 2023 20:25:40 GMT  
		Size: 22.8 KB (22848 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.2-fpm-alpine3.17` - linux; arm variant v6

```console
$ docker pull drupal@sha256:990653cbf1dc000b03dbee000fce3d3c4d1a888f64c1159e400ecd70759fab7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37723687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60c84793c44825a65c29f040fd99b2e4126c04d2773853d4042a5922acaf0a2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.13
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3615ead72921cc0e7d9b570fd1cbf98286500906c9e85157bc0f7f9215b4f62`  
		Last Modified: Sat, 21 Oct 2023 03:22:13 GMT  
		Size: 3.6 MB (3620887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ddcbcd062e3baf30ecfb665bd8957b2a308e0ea23338eab716e5c697cc3a81`  
		Last Modified: Sat, 21 Oct 2023 03:22:12 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996322317f3e60398a7a63dcc220eabf2187328dca0c2c0eb96fcdd5d91984a`  
		Last Modified: Sat, 21 Oct 2023 03:22:12 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c80582fa7006b0ad92d2747622b2f8764a0a83014d87dd7dcfee606c39f92`  
		Last Modified: Mon, 27 Nov 2023 22:31:59 GMT  
		Size: 12.1 MB (12089665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344a4b224f2c0f7341779b8d10fbbacba02be540341ef36d73d3b93671dbd5dd`  
		Last Modified: Mon, 27 Nov 2023 22:31:57 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b77d08b7feb3ff213d89b2f08c0e081462f0a9f932a147b76fe288914816a69`  
		Last Modified: Mon, 27 Nov 2023 22:32:20 GMT  
		Size: 13.8 MB (13777915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4680714dc8fe2237164a9729db3faa78f76e4f67da0c8c485e48cff1eaa1fb5`  
		Last Modified: Mon, 27 Nov 2023 22:32:16 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36e5b0947a2523adf80218b70e71ba87e5bc5c468da741e1308c4df8b8b0a1`  
		Last Modified: Mon, 27 Nov 2023 22:32:17 GMT  
		Size: 18.8 KB (18779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef95c3123b6750286fbb3792edda3ce35d9c03985abea21811fda1094e4942fc`  
		Last Modified: Mon, 27 Nov 2023 22:32:17 GMT  
		Size: 9.2 KB (9174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd963d290142dac8d344db5f7295d1b45c93f95d1a65fa5da9b8645a40160db`  
		Last Modified: Tue, 28 Nov 2023 00:14:29 GMT  
		Size: 1.7 MB (1679733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babf7c7795169b986c7cf5c8b1e6c551b5239c86a9119fc9a7d6e15829f63e0d`  
		Last Modified: Tue, 28 Nov 2023 00:14:28 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2231d9668a526174c1b47452bbc9bf4ce96433fc8c81847497bd2bc9be68d106`  
		Last Modified: Tue, 28 Nov 2023 00:24:41 GMT  
		Size: 3.4 MB (3410296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.2-fpm-alpine3.17` - linux; arm variant v7

```console
$ docker pull drupal@sha256:d71269a7ea0b789cf3541a4749b9a62a363b6c0ae534855516ab406962dc2fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36191876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d2fc806b432a50e32b25ffa14a7a5b30f6f9af8e805851d493cfba839259f7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.12
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:b82e4fd40279a40aa2eecd301fabb2dca254727cc09daa8d0caf69ac28c44af1`  
		Last Modified: Mon, 07 Aug 2023 19:58:08 GMT  
		Size: 2.9 MB (2869425 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266755729fd4b431e323998f3335d60c48ca5b6b1e495b1841084469413cdf31`  
		Last Modified: Sat, 21 Oct 2023 03:44:24 GMT  
		Size: 3.3 MB (3348109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62e017575e43e4b32d3a5c7aa82e3964278cf4fbca4673ffa9821ad4ecb463c5`  
		Last Modified: Sat, 21 Oct 2023 03:44:24 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba28e04f456480646adaa0ccacf8b8f16d3071aa89bdbe881bcefb2036fea422`  
		Last Modified: Sat, 21 Oct 2023 03:44:23 GMT  
		Size: 268.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f5f4a8de26193c0d4e8613508daa91b5e045789216fc4929dbee4507f564a757`  
		Last Modified: Sat, 28 Oct 2023 04:06:22 GMT  
		Size: 12.1 MB (12069493 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6daaea568d7c9c32d3dbac4565fe35f72dfd4dd13fd2258977c91655d190b0f8`  
		Last Modified: Sat, 28 Oct 2023 04:06:21 GMT  
		Size: 498.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c0f21b49816680687dbc8aeabe91e511928fa439494cf7239b3c588deb98c21`  
		Last Modified: Sat, 28 Oct 2023 04:06:49 GMT  
		Size: 12.9 MB (12914777 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:607171e3867ffb4e8dcde0adeed80817b56ac50c33d1f648c2498f0954aace40`  
		Last Modified: Sat, 28 Oct 2023 04:06:46 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3a46fa930406196c73ef65a4871ba144cd03a74ed823f5f2fcd70dfde01f77c`  
		Last Modified: Sat, 28 Oct 2023 04:06:46 GMT  
		Size: 18.8 KB (18771 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2f0a503e36c4960cf6458091fb4e96a3b43ac3982f2ad6d36546f958155c848`  
		Last Modified: Sat, 28 Oct 2023 04:06:47 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a9f3e72e8e0bcfe758e6e872f87885730807d6f5b54755a26bcebe1c33747abe`  
		Last Modified: Wed, 08 Nov 2023 20:41:00 GMT  
		Size: 1.5 MB (1547040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2ca93883a5994e554e21dd01fd0ccdd6ce1527e3e64f18c6ecd9b560b55c3b8`  
		Last Modified: Wed, 08 Nov 2023 20:41:00 GMT  
		Size: 310.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce3d5090badef90595952b90124557fe6cbdcdd09858bbc719ca736180cdf026`  
		Last Modified: Wed, 08 Nov 2023 21:18:20 GMT  
		Size: 3.4 MB (3410296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:ae69c7ea6622d1385e65500c15520225a8eafc2aa3378426d65eede90fc56aee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 KB (250947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0982dead47c1caf1bd43303d62e91a4299be27ceea198ac0bdf6b3a4e6b7b9a0`

```dockerfile
```

-	Layers:
	-	`sha256:145afc950c7546ca6309c98d940eef413d779c444d41eec00ca5b95829deceef`  
		Last Modified: Wed, 08 Nov 2023 21:18:18 GMT  
		Size: 229.6 KB (229645 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:281a0f72f17f857f71d12128e0e4b8119f4e4712166d85704f0da66c3f5b3f42`  
		Last Modified: Wed, 08 Nov 2023 21:18:18 GMT  
		Size: 21.3 KB (21302 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.2-fpm-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:58c28413b9508e55a23d705de02b9d440fa737b156b6404b4f944ff0b935e0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40159375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca644cd2689833fb570bd9def431de3fb24d5993f83ad39c7388518d655e21f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.12
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b34a0f55e243236a510d854843712a9aa7159ab999cfda1110aa86715d5379c2`  
		Last Modified: Sat, 21 Oct 2023 05:47:16 GMT  
		Size: 3.8 MB (3809798 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4babc9015c2d2337c98044da97d8aa95024ab76852c6fcf6bf3ff14f02ab309`  
		Last Modified: Sat, 21 Oct 2023 05:47:15 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8990ce5d2eb593002dd6a3980d05121601226e231dc1b51ccd3ecdc06ebcd80e`  
		Last Modified: Sat, 21 Oct 2023 05:47:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81300d6020d14bc2779e04e080ebafac41d8258e870d96ae1e6a76fe59bcd051`  
		Last Modified: Sat, 28 Oct 2023 04:05:28 GMT  
		Size: 12.1 MB (12069499 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9302fcd0c677b6a53b65797152bf48a867b0606a7ee04914ed2f405f6d3fff92`  
		Last Modified: Sat, 28 Oct 2023 04:05:27 GMT  
		Size: 497.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17b6eba898d934f9411610012a67d7dde92ace5b7d008e1f66705f100b71f8ec`  
		Last Modified: Sat, 28 Oct 2023 04:05:53 GMT  
		Size: 15.1 MB (15133845 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc50bfa15c4495fb9aaa297301eb7433c7ccae16cf32126db80241f13c2c6982`  
		Last Modified: Sat, 28 Oct 2023 04:05:51 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:758a835557efabd5ebd32747d818dc14f025c21c8d6865a5c85fd877f38f6bea`  
		Last Modified: Sat, 28 Oct 2023 04:05:51 GMT  
		Size: 18.8 KB (18768 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7e9cae1059934e6ac8d2eecb70097b5c6f2448bb0339db856400fb7af8bb70e`  
		Last Modified: Sat, 28 Oct 2023 04:05:51 GMT  
		Size: 9.2 KB (9174 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e396c91180d084656b5bb26fddfa6f0d98e6aa33a2da311569f616ec225028bb`  
		Last Modified: Wed, 08 Nov 2023 21:02:23 GMT  
		Size: 2.4 MB (2444891 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62e1d5a5780bb1227fb309814b76ea61a9ede217f571c9826a6b9caa7a59f0f4`  
		Last Modified: Wed, 08 Nov 2023 21:02:23 GMT  
		Size: 312.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b6a4089edd6343b65d8a9ce0caf42fa893cd3cdaa81af545f411dbba2bd6031`  
		Last Modified: Wed, 08 Nov 2023 22:05:53 GMT  
		Size: 3.4 MB (3410320 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:324d10c32a4203230c7094e2842c44cae10a44792eac2a3641764c07d1a4ece4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 KB (250861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af29df92ec8eaa647a1dbfb278e3fe662eaaedad235427ecd9059cd35b58fae`

```dockerfile
```

-	Layers:
	-	`sha256:7c31d0b20facb31ce2e5ee07ba5b6905cb1b2da467458590447733f46e06cf78`  
		Last Modified: Wed, 08 Nov 2023 22:05:52 GMT  
		Size: 229.6 KB (229632 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e2034976f6fda934891bea341494f8950310f11bc38a8987cc5181ec94ad3e2`  
		Last Modified: Wed, 08 Nov 2023 22:05:52 GMT  
		Size: 21.2 KB (21229 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.2-fpm-alpine3.17` - linux; 386

```console
$ docker pull drupal@sha256:cf7d59d045ff58f83394be488e169d2a46eb2ecf7e43a48bdbf0d7e21232173a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40944658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ace307d0011b98a9c1019e35b8ce99f9ba1252ca6a672efb4af120c986d5715`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.12
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be77e393d6682467b55f831fba7245c492ff2ebb973f274c70a0599f86ae8320`  
		Last Modified: Sat, 21 Oct 2023 06:35:22 GMT  
		Size: 4.1 MB (4102087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3bf5db589daaa67b227ca91f01467309314a7bcaae01037a478e89635647e1d5`  
		Last Modified: Sat, 21 Oct 2023 06:35:21 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6de995542458f5727da8d83e6d9736b6d9b159a7ff19fc5675533a8afa30602b`  
		Last Modified: Sat, 21 Oct 2023 06:35:21 GMT  
		Size: 268.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab5b247bc8b7ccc23c0aaa2f4728880b3e4334b7bb6825854d979376c2c184ba`  
		Last Modified: Sat, 28 Oct 2023 05:33:22 GMT  
		Size: 12.1 MB (12069500 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86c0b0ca94eccf638d60ec5af920fb3aac384499ed7543d9d41c12ba8f031ea9`  
		Last Modified: Sat, 28 Oct 2023 05:33:21 GMT  
		Size: 496.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b2751379d7990bad7a0c2b5c603f18b23fdb859f5e58836371394066f95a7f52`  
		Last Modified: Sat, 28 Oct 2023 05:33:52 GMT  
		Size: 15.6 MB (15627865 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c097c06f10166bcb9fe655b0fdf62d7d2e72c69c18ed6e8a7f415b462668605`  
		Last Modified: Sat, 28 Oct 2023 05:33:48 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40331c2a1ed92b2bbefc045cad2f9e6b70ee5121287caec1dd461727c5a25974`  
		Last Modified: Sat, 28 Oct 2023 05:33:48 GMT  
		Size: 19.0 KB (18985 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f9159caab39400986085d5f0397e3bf82edc2838bac841c57d17eeb290fa976`  
		Last Modified: Sat, 28 Oct 2023 05:33:48 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e21a91d251cb464d69bd797157ee7d31eacfde4ee98ccdec6a66e33e14f0e16b`  
		Last Modified: Wed, 08 Nov 2023 20:25:49 GMT  
		Size: 2.3 MB (2288180 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579cf8b6dcd6f57ac1ebbd0c198cd55b6daa92c731e4845f21e4761d3f7e29d3`  
		Last Modified: Wed, 08 Nov 2023 20:25:49 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81722a88cfd706a682daa5f422920ea4bcc766b52706869bc0dafebbfc32fa28`  
		Last Modified: Wed, 08 Nov 2023 20:25:49 GMT  
		Size: 3.4 MB (3410295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:4fd12451cd73ce8e5c5a563a0613ae383246969e35d8a60d7d1e05eea9a229e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 KB (22610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afde82f733ee07f448d335ceac4aac16c48e4ffdbe27a18bc620c5bbec5efdc0`

```dockerfile
```

-	Layers:
	-	`sha256:3e33305f4e36f9c5bd39645023d84b28bc5bfd2ed8bb8f8aa343d30cf2e1b6a2`  
		Last Modified: Wed, 08 Nov 2023 20:25:48 GMT  
		Size: 22.6 KB (22610 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.2-fpm-alpine3.17` - linux; ppc64le

```console
$ docker pull drupal@sha256:8ea9ff4ec638da6cd8df0c31404b1ab397175032eb63992bee096d205b0361e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40493991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7644e23e2af9ac8e52ac3655a99922e935e6de30983fe19ad272e944a75c7c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.12
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e873c5cf6843a39c83c213ecc24b0ce88d22c597cb59c1b30eaf91ee60983432`  
		Last Modified: Sat, 21 Oct 2023 03:16:15 GMT  
		Size: 4.0 MB (3995064 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a6c74173d1cdae2d8dabd83394d41d1e351930fa23693f3d46bf78dbb89ca121`  
		Last Modified: Sat, 21 Oct 2023 03:16:14 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30228596168cc7b41cc835de78d55ba39b878894037e89ad156128301d96bad4`  
		Last Modified: Sat, 21 Oct 2023 03:16:14 GMT  
		Size: 270.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:308e546b5b0f53ffcc8f641499a5f8c0096fba4740f81e1fa52349137d859d3e`  
		Last Modified: Sat, 28 Oct 2023 03:20:51 GMT  
		Size: 12.1 MB (12069499 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fae67353adf5f0f8054d5bbd72b6d92caebe4585b3a1de86d169746237d391f3`  
		Last Modified: Sat, 28 Oct 2023 03:20:49 GMT  
		Size: 496.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6cde6a3380aac230f70deadd83e59643f2ff10da34b39dc9ab66737e29f7c78e`  
		Last Modified: Sat, 28 Oct 2023 03:21:26 GMT  
		Size: 15.7 MB (15662122 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef49f2ad7fa904c9fcec23c73623e87466cfa647e88767f7640fbb347152eff1`  
		Last Modified: Sat, 28 Oct 2023 03:21:23 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51c7cba12076fbd913388d9b417b3646a4e97fdb552c12e42abde66370ebbf00`  
		Last Modified: Sat, 28 Oct 2023 03:21:23 GMT  
		Size: 18.8 KB (18771 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c15169a37c51249aeb63ef6ba6487af47c98549b2789621608b1297e696fc7f`  
		Last Modified: Sat, 28 Oct 2023 03:21:23 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2936321c0563cf4ac32dc860358ab2c255cadd9eeeb1a86949735b387acfd2e5`  
		Last Modified: Wed, 08 Nov 2023 20:46:42 GMT  
		Size: 1.9 MB (1932892 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4d2eb93949012bd2bd9246c2086d8be3e46cffdec65c97d1d6f4a1538f2ab24`  
		Last Modified: Wed, 08 Nov 2023 20:46:42 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63542d253b2572e11f0ca49cf9526033e7b20955850ec3fc357fbb5075e69441`  
		Last Modified: Wed, 08 Nov 2023 21:42:40 GMT  
		Size: 3.4 MB (3410317 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:b7bf12b0f7792f4ca717cb5a155584bef05805ed11462eeb8dd1e08cd658be57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.3 KB (249264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a292577b2c185462fae04749dd45d96c5d4eff0d1016b1ac7c555fa5e391e6`

```dockerfile
```

-	Layers:
	-	`sha256:0ccd2422cebe414e19ce0817c11777b0de9cc31d1f1e1fd6a9d048fe7433b222`  
		Last Modified: Wed, 08 Nov 2023 21:42:39 GMT  
		Size: 228.0 KB (228011 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1396bcda9d853610ff1eb018252a398ba18028fd49b1eafe4a2209c1b1304142`  
		Last Modified: Wed, 08 Nov 2023 21:42:39 GMT  
		Size: 21.3 KB (21253 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.2-fpm-alpine3.17` - linux; s390x

```console
$ docker pull drupal@sha256:8bcc783244b57cd68797d0aa40674f9eb0113434117e816d4ec59289349e28a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38444432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3bc1676a8b531a991246c4f477d6345333a1398adac2171b46960671be95bf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.2.12
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:153856869a93ebfc3f61d3f5116b1550a1aebd971304ed195e66a4151a189042`  
		Last Modified: Sat, 21 Oct 2023 03:23:45 GMT  
		Size: 3.8 MB (3762212 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef93127a61d902b0f6d7e810968191c39e1ae40f7e4314f70b295007af54e7f0`  
		Last Modified: Sat, 21 Oct 2023 03:23:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:823533547a7c859ffaad5a027c6b4f8adec6cbdbc7472544cd88f0360c6cae08`  
		Last Modified: Sat, 21 Oct 2023 03:23:45 GMT  
		Size: 267.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b70e0f755eca468c397690e506fb3e23a7ecb2c005c744317f136b2dfd07b35`  
		Last Modified: Sat, 28 Oct 2023 04:46:05 GMT  
		Size: 12.1 MB (12069512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cddd7515c338ee1493d243ab2527bccd1d15020112294c4326d861c5b9f3a1d`  
		Last Modified: Sat, 28 Oct 2023 04:46:03 GMT  
		Size: 496.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:200de998c8242037298d30b2751a8d5e600c4fedd94d9ec6f12e35b105b2cfef`  
		Last Modified: Sat, 28 Oct 2023 04:46:27 GMT  
		Size: 14.2 MB (14181268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01b860e2497f759c57a127381f382a02ab897b9a98497972ab7150c8bc44fd78`  
		Last Modified: Sat, 28 Oct 2023 04:46:25 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29c45ef68f35a91b53d025c5f1bfea279ae44c6f08bb21bdfeae8564805feb98`  
		Last Modified: Sat, 28 Oct 2023 04:46:25 GMT  
		Size: 18.8 KB (18808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29d4ba665dbf8b28c3d4b350ce38e7beb7b1122d835268df20b9c9bcf74e47a1`  
		Last Modified: Sat, 28 Oct 2023 04:46:25 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e2173c98e5cefe3ff4af956d2b748dfcd9abf37cfa63f028e3076548402733`  
		Last Modified: Wed, 08 Nov 2023 20:38:36 GMT  
		Size: 1.8 MB (1812389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b54aadd96090ad7b209b3b976e8054d3d64b99db1deaa311efa6360a5aa2cfe`  
		Last Modified: Wed, 08 Nov 2023 20:38:36 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d106b6e2d9670f527863bacd9795cbcc65e1dc70dbcfb240264149ca7d7e4192`  
		Last Modified: Wed, 08 Nov 2023 21:15:18 GMT  
		Size: 3.4 MB (3410303 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:044ffe8b9ce4fb9b1ea5ae63dcfefa887016d7a10100fd64cf14f6195d840a0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 KB (249212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daefd4d9722e41c87d07c836e016a3d368407e4f53fc6dd12b3e91f2d428abe8`

```dockerfile
```

-	Layers:
	-	`sha256:a1220daf797d5b866e9c9c268704c67abe581ad7b99e902a620740541ab52bea`  
		Last Modified: Wed, 08 Nov 2023 21:15:18 GMT  
		Size: 228.0 KB (227989 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bdd5a525f2528b8b92d6269ed7d1657bfabcc54d1f17fed3fa5f4a7856abfeaf`  
		Last Modified: Wed, 08 Nov 2023 21:15:18 GMT  
		Size: 21.2 KB (21223 bytes)  
		MIME: application/vnd.in-toto+json
