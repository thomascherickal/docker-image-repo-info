## `drupal:fpm-alpine3.17`

```console
$ docker pull drupal@sha256:187f555b4c034d43ecdce56248088620e6feb7f17f5d51f0b14cd83db4fb1c82
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

### `drupal:fpm-alpine3.17` - linux; amd64

```console
$ docker pull drupal@sha256:47097744f4376cf5696a9dfbfc8b230b974ac154d44d1de3de229d5f1ebf382a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56211950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afefa09f55b24a544da23b78ef8ba89ef3ddaa57e17e78614ed065f801b47228`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 04:04:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 04:04:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 04:04:37 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 04:04:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 04:04:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 04:04:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 04:04:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 04:04:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 04:27:17 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:15:04 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:15:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:15:04 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:15:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 28 Oct 2023 02:15:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:22:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 02:22:32 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:22:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 02:22:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 02:22:34 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 02:22:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 02:22:35 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 02:22:35 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 02:22:35 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:b15504abedc11c4d5a9b9a289a74fd1bf4ebbbfe529a2285391bb27ca80457b9`  
		Last Modified: Wed, 08 Nov 2023 20:24:55 GMT  
		Size: 2.2 MB (2208699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a51a350e94d17590bf62bf17cd3487ea8e7a01c092b73997fe860c2f2ea2241a`  
		Last Modified: Wed, 08 Nov 2023 20:24:54 GMT  
		Size: 311.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d55125313b79357cc5aa77c4290c6e1f9b3512bf3fe2401aa696667eb614f0ac`  
		Last Modified: Wed, 08 Nov 2023 20:24:54 GMT  
		Size: 705.0 KB (705003 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e38404edfaffce795145be00d0c215605fbbd35cee27e02bff297018ce2351e5`  
		Last Modified: Wed, 08 Nov 2023 20:24:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca9f8257a47ddb58344303f32af3eb4265eec708b0a070c3b0860c1a2ad2c3c0`  
		Last Modified: Wed, 08 Nov 2023 20:24:56 GMT  
		Size: 18.5 MB (18549207 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:9923f8af8651ee0c793204a386a6148bd7774fc89aa7376a8641902b784961e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 KB (316159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f10cff4686bcfa7595131f24174e611c6075b18e880aeed55a8eeb5be1ab3e5`

```dockerfile
```

-	Layers:
	-	`sha256:7a1b2a6d610405454ce074ca2ed42db4dc6a08edfc12672ad0a6a549da18d25a`  
		Last Modified: Wed, 08 Nov 2023 20:24:54 GMT  
		Size: 280.4 KB (280360 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b895403a9179b847414ed7b9ea1c6dadc80b848d853204dcef4b7332634b6f09`  
		Last Modified: Wed, 08 Nov 2023 20:24:54 GMT  
		Size: 35.8 KB (35799 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:fpm-alpine3.17` - linux; arm variant v6

```console
$ docker pull drupal@sha256:86e3b8266768de83cc25487c6fe793c1e13aaeb23db5ad50274aca5f5b0860d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53568440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2845581f47301f4d473c9a0a00d5f3997d4f38f894fe0577e5ca54192b86e861`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:22:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:22:40 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:22:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:22:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:22:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:22:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:22:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:22:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:42:57 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.2.13
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 9000
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:a120fcaf8aab33f0cf41b93bcd22737056f4ec3a816fd8d44f2d8c44c8e9ef21`  
		Last Modified: Tue, 28 Nov 2023 00:14:29 GMT  
		Size: 705.0 KB (704998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7477582509129beec66fbba703c63fd27d392dcf659e30ddc4556a672e8a8726`  
		Last Modified: Tue, 28 Nov 2023 00:14:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf6c4b2d2d898776b96b6760bc45a3f1e968d548746bd00d4cc293474f59366`  
		Last Modified: Tue, 28 Nov 2023 00:14:34 GMT  
		Size: 18.5 MB (18549936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine3.17` - linux; arm variant v7

```console
$ docker pull drupal@sha256:0dc1c95600d490e054241032d78f0416e822fb1f7411c9fc94714e64dfe82da9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52036507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b40b9e5000b3f2c147f472b08751357773876473887db26e7a8108551f7147c3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:29 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Mon, 07 Aug 2023 19:57:29 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:48:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:48:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:48:55 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:48:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:48:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:48:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:48:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:48:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 02:07:53 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:54:44 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:54:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:54:44 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:54:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 28 Oct 2023 02:54:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:59:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 03:00:00 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 03:00:01 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 03:00:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 03:00:01 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 03:00:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 03:00:02 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 03:00:02 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 03:00:02 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:0004b630cc5117d1f5d294f05b00c70b82f38d7f53827091c0dba1099049deae`  
		Last Modified: Wed, 08 Nov 2023 20:41:00 GMT  
		Size: 705.0 KB (704997 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b6de1d20178dd0cc83134a0c731189c32be7acb1e46585ac8eb6c96bf9cb78a`  
		Last Modified: Wed, 08 Nov 2023 20:41:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbc69629e11e6ac2484942e9d1ba498fb3d7174704427101fb92c5eb44586715`  
		Last Modified: Wed, 08 Nov 2023 20:41:03 GMT  
		Size: 18.5 MB (18549815 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:f4927e0e63b9f2a4f67920e9ab9d4187949946281f825c129efb322e1397a98c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 KB (311626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4554a17a395a0f3c924e5f8827d8be16522d94186e7ea9a23180fdd4a81e2e`

```dockerfile
```

-	Layers:
	-	`sha256:6ee6a5f3ca4f527d447e4272d1805d51c4ed25ab13cb0c2a146a2182fd331177`  
		Last Modified: Wed, 08 Nov 2023 20:40:57 GMT  
		Size: 278.0 KB (277956 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5b17beee3284c61093eae92877d59c1cd1cc64ac0fc287eadf415701454f8aba`  
		Last Modified: Wed, 08 Nov 2023 20:40:57 GMT  
		Size: 33.7 KB (33670 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:fpm-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:01ba3f452e45a3f391334bb1c8093fced8b0fb556ee1bea637129bc335a4f8cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56003985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9edb60c63f85bd3d931b69954f0dcb87a99fcd757eb24013e6de4a7d48e536b0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:30:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 03:30:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 03:30:05 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 03:30:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 03:30:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 03:30:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:30:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:30:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 03:53:03 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:42:14 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:42:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:42:14 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:42:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 28 Oct 2023 02:42:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:49:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 02:49:39 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:49:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 02:49:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 02:49:40 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 02:49:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 02:49:40 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 02:49:40 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 02:49:41 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:67b61a47576bf8f54ce043a743efea94f05261a42280e05799d66191d839afb0`  
		Last Modified: Wed, 08 Nov 2023 21:02:24 GMT  
		Size: 705.0 KB (705001 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:daf1350f2a4b7de1e078bbae8641f93effe552286e2cb0b942094fc6ceed11bc`  
		Last Modified: Wed, 08 Nov 2023 21:02:24 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad7ba10cc88b19bc3b36b61635e0406cb0affd44371519ded88d8c6952714274`  
		Last Modified: Wed, 08 Nov 2023 21:02:26 GMT  
		Size: 18.5 MB (18549813 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:764d9760aeb014aaffb57e1971d9b35013ea4c3a59d5409c583e19d76cc3d862
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 KB (311451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce33b4cc082827778aa403d0f144f3ec7b6629f6777892c05ca89c5d71b6240`

```dockerfile
```

-	Layers:
	-	`sha256:f571f05c6262ffc8fd6fa05d0baac8701c9deb895539eee6b4366112e73cf92e`  
		Last Modified: Wed, 08 Nov 2023 21:02:20 GMT  
		Size: 277.9 KB (277907 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a3a342006006d9e81d65ae0ad2a2c7ee7618a3cf0a2333e4de99f3f2e41aa7a0`  
		Last Modified: Wed, 08 Nov 2023 21:02:20 GMT  
		Size: 33.5 KB (33544 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:fpm-alpine3.17` - linux; 386

```console
$ docker pull drupal@sha256:7914439794f8492e6e6f4c7e52a64a8a4ee143c053edac7edfefa4b367c71393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56789486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c4b8b4ee68cd29a79f04863ac08ad99166317c232a3915a256dfe60da89e53`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:30:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 02:30:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 02:30:25 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 02:30:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 02:30:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 02:30:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 02:30:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 02:30:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 03:08:38 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 03:14:06 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 03:14:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 03:14:07 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 03:14:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 28 Oct 2023 03:14:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 03:26:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 03:26:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 03:26:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 03:26:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 03:26:40 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 03:26:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 03:26:40 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 03:26:41 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 03:26:41 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:8b1c20acfd072746e654137d9cc38f67cddfe098a27bb798ee666a7185b43f6c`  
		Last Modified: Wed, 08 Nov 2023 20:24:05 GMT  
		Size: 2.3 MB (2288162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ea10927cc4162dc956d1beaf643c9c6b760d22341624ff9af7aa972a23ccb0a`  
		Last Modified: Wed, 08 Nov 2023 20:24:05 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62d1bd741d541729ed125d853b25ad3376ec7f4cb7aaecc37e7100322806b3f4`  
		Last Modified: Wed, 08 Nov 2023 20:24:05 GMT  
		Size: 705.0 KB (705007 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:330b09c500bfc2e3ae836e6237714bfa9e42483d7ba58f83c06350319f9650c4`  
		Last Modified: Wed, 08 Nov 2023 20:24:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59b4ca6b0c0726f8d173e7b1b535f4861121bd3a001c0b324f74427e3ae906d8`  
		Last Modified: Wed, 08 Nov 2023 20:24:08 GMT  
		Size: 18.6 MB (18550019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:3103afeade62672840e50c087bed98c0ec4dc17f4f7c3d60d6cf61875cdf2395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 KB (35526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91fe3f2a4b84007a74cc8e96437aa1444cf23c9de509f547ccd08fb7b006dbae`

```dockerfile
```

-	Layers:
	-	`sha256:871a7ae0e6911ac530e03278da6048cd618e10950826df913e32a42e98da23aa`  
		Last Modified: Wed, 08 Nov 2023 20:24:03 GMT  
		Size: 35.5 KB (35526 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:fpm-alpine3.17` - linux; ppc64le

```console
$ docker pull drupal@sha256:f98abb6ef7d411dfb0315695abf5be4a260c79a20d3ecf4de0b1e10ac094fffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56338406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a88546656811fafd078914cf2dfc7049f92a167ae5e3e0148ccc1103f19484`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:27:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:27:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:27:46 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:27:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:27:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:27:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:27:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:27:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:44:23 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:06:38 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:06:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:06:38 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:06:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 28 Oct 2023 02:06:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:12:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 02:12:01 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:12:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 02:12:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 02:12:03 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 02:12:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 02:12:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 02:12:05 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 02:12:05 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:ed8f469a14c06a527ec67b0de5ff0b7c4ce773c6bd8163f5e60ad6c3fec26f7e`  
		Last Modified: Wed, 08 Nov 2023 20:46:43 GMT  
		Size: 705.0 KB (705004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a1ed0b3f701ae6036a5cb2ee1fa5bc0d34c807e7fca23ba6988fb1bc00f3dae`  
		Last Modified: Wed, 08 Nov 2023 20:46:43 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27b71c9c704338623810b672411e1be5aada6db0ca2e0752fedd8f99ecc8d321`  
		Last Modified: Wed, 08 Nov 2023 20:46:44 GMT  
		Size: 18.5 MB (18549613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:6e028b82d04308631e5097225025eb8d7430be617e70f6d6475a7bf7f8bc5f62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.9 KB (309906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0c169cf0e441bf3f2045b6f2b9208370f1c974a1b5b5a9b0ff84e31ff5f88`

```dockerfile
```

-	Layers:
	-	`sha256:7ffb4e30709f29333f46554a49ad178bd7d66483166e3e222c901d17228eba70`  
		Last Modified: Wed, 08 Nov 2023 20:46:39 GMT  
		Size: 276.3 KB (276310 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:db984a4a971f5f996219829162407b247f43710890cdb294a4c6b986bd8a7af5`  
		Last Modified: Wed, 08 Nov 2023 20:46:39 GMT  
		Size: 33.6 KB (33596 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:fpm-alpine3.17` - linux; s390x

```console
$ docker pull drupal@sha256:6eb89aac286fa671a1c5a66140d431210f6752a7ff84c92c3b109b9459946ef6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54312834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a29bfd46330b6d63adbb40a3e73130e5724c5df5301a238c243c3b4e623652`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:27:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:27:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:27:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:27:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:27:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:27:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:27:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:27:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 01:46:12 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.2.13
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 9000
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:756792308e803599283d15bad30337ee60f15d834ed37e1db92477db88116635`  
		Last Modified: Mon, 27 Nov 2023 23:31:33 GMT  
		Size: 12.1 MB (12089679 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb579cc9b961a78356f406384c1ead330de424418a433590387a17ddb4948220`  
		Last Modified: Mon, 27 Nov 2023 23:31:32 GMT  
		Size: 498.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5020ba3fbea086f3074b593c5e87df579719ea23044b984c668c283f5dd35f92`  
		Last Modified: Mon, 27 Nov 2023 23:31:46 GMT  
		Size: 14.2 MB (14186182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9fdad2fa6ce7f038d202332b4bd450c1c8933800f3e5c0f15fc5cfd97d0cb`  
		Last Modified: Mon, 27 Nov 2023 23:31:43 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:35e33e560d006eeb2becad27c629d2da8cd947eccf84aef8ae1cb1d9aed66e86`  
		Last Modified: Mon, 27 Nov 2023 23:31:44 GMT  
		Size: 18.8 KB (18819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893590ee3d972736358ce8bdd5f8cb57cfc8bf3d9d15ecf5407c1335136b3c80`  
		Last Modified: Mon, 27 Nov 2023 23:31:43 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed648546904c9632a090d8a5ad1e93a17da2487ae10c93f5c524f3b54550fd73`  
		Last Modified: Tue, 28 Nov 2023 01:54:26 GMT  
		Size: 1.8 MB (1812368 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6402d6255d08f294ca7a2a88e871f8136db105eb9d16a1050e05631f27f1c127`  
		Last Modified: Tue, 28 Nov 2023 01:54:27 GMT  
		Size: 312.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aec9d56acba1835b8913867bf0d3d5bef5e13ecf6250b9bd9c080db160f39808`  
		Last Modified: Tue, 28 Nov 2023 01:54:27 GMT  
		Size: 705.0 KB (705002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:710cd8c7763e5d71d14ddcf95f42b04c8838c9bad8f1a598e2f350e77ff0bf9a`  
		Last Modified: Tue, 28 Nov 2023 01:54:27 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00b3179f866649da39dfad451c262ecd340f8a351fc0439dcb274a3d6511fc05`  
		Last Modified: Tue, 28 Nov 2023 01:54:28 GMT  
		Size: 18.5 MB (18548512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:0eb5f5a2e2c16a4835128c6d523d85ce7e38da64506022c31ba67e3e5eb6e058
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 KB (309778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67f84f2969845241f70d574acf0613e0d8aa3ccc9df6e9ef7745edd143b64de`

```dockerfile
```

-	Layers:
	-	`sha256:a9ea1ac32141b537552818186da2971ce1bb480e0a028bb08a0a102457249ab9`  
		Last Modified: Tue, 28 Nov 2023 01:54:25 GMT  
		Size: 276.3 KB (276252 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f74c8b5a06a71dab36aed951bb6400e4aa220ecd88a92063340b8ac9aabb7408`  
		Last Modified: Tue, 28 Nov 2023 01:54:25 GMT  
		Size: 33.5 KB (33526 bytes)  
		MIME: application/vnd.in-toto+json
