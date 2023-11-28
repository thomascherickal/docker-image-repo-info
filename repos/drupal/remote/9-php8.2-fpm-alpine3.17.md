## `drupal:9-php8.2-fpm-alpine3.17`

```console
$ docker pull drupal@sha256:c3894ea42485c23c3cc0e6dacc53bfccae726f52d2dd7037e7f0e4083c4c2382
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

### `drupal:9-php8.2-fpm-alpine3.17` - linux; amd64

```console
$ docker pull drupal@sha256:a36456447b48a0ed4ab27b70dd452509389085566d77e465b297275556bf704a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60568750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8399246a317db5a43b81b0aaec21874846bf2ee3981aeb00590edf5b771d16e3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:acbc27033c688cb004403aee2db368decbfbe391bcba451dd1d0004860978448`  
		Last Modified: Tue, 28 Nov 2023 00:18:50 GMT  
		Size: 12.1 MB (12089671 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e814f526ba05f87c29b8f1728a1a30f54ee388030e58204f81070709550b7b9`  
		Last Modified: Tue, 28 Nov 2023 00:18:49 GMT  
		Size: 498.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5061eefa56de6ed799dd4025a656a371e921efecb108519f29d71eb0fde5fc1`  
		Last Modified: Tue, 28 Nov 2023 00:19:08 GMT  
		Size: 15.3 MB (15306658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:290495951b84285a1d0e682193747546b22a1faae604679fa036728c1fd18895`  
		Last Modified: Tue, 28 Nov 2023 00:19:06 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23a69e9a5994b110ffb831daeab6d54dfd1c270e735a036b09ce7c3e51fb2907`  
		Last Modified: Tue, 28 Nov 2023 00:19:06 GMT  
		Size: 19.0 KB (18986 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0af6b42d2f1223324d1d1048c8fd579f85534b3417d074c8b29b9fa022b64015`  
		Last Modified: Tue, 28 Nov 2023 00:19:06 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:593a63d08b1b4b6739eb764c31e5b8e356cd41cf231db74f67e76e55395bec0d`  
		Last Modified: Tue, 28 Nov 2023 02:24:19 GMT  
		Size: 2.2 MB (2209002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5412145721af4dc1f38a4c763070b3d85456e6e17553dee83970913519e39981`  
		Last Modified: Tue, 28 Nov 2023 02:24:19 GMT  
		Size: 309.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a62cc1631c7a2bdc5526cab5109890e6038efca5831062357b7d1a9bfea24b71`  
		Last Modified: Tue, 28 Nov 2023 02:24:19 GMT  
		Size: 705.0 KB (704990 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb3e4fa9d2d64f6fa866c548870d004ee156729dbac8d484f12e57a4c1992881`  
		Last Modified: Tue, 28 Nov 2023 02:24:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc31a9e46982bae9f589fc91ae91db7c5c8a24714a3722944785036e7f3c2ed`  
		Last Modified: Tue, 28 Nov 2023 02:24:20 GMT  
		Size: 22.9 MB (22879891 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:f68d6e602137955e75a0463d3b3ac76c9a3d5052d0b783bc1f571cbe08edcb79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.4 KB (315428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2929bcc76713e5738d1b4f2fe6ba88845d061bef126f590afcd3276c15c0dd4`

```dockerfile
```

-	Layers:
	-	`sha256:78b3ca42f9f4ba83ad979b63ead086bb3487f8781470fe8767550504f04aacc5`  
		Last Modified: Tue, 28 Nov 2023 02:24:19 GMT  
		Size: 281.2 KB (281249 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:600d1a30c70f7b584430f20bf50eef747f2dd4f63aeb09d4c60114a8c303d9d5`  
		Last Modified: Tue, 28 Nov 2023 02:24:19 GMT  
		Size: 34.2 KB (34179 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-alpine3.17` - linux; arm variant v6

```console
$ docker pull drupal@sha256:da64bf0d68e03e1e2d9704633655da5d2ae16e465b70b13d9624d0a03168a612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57898220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8d3d6c47a0812b7c5e2d1fe7cdd3b401b685bd9bb3f6f23e957c543482caf9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:69d5f81f837544a93fd18363ad4666666495f1cb361bfc306aeb45d9ecafa527`  
		Last Modified: Tue, 28 Nov 2023 00:21:55 GMT  
		Size: 22.9 MB (22879716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.2-fpm-alpine3.17` - linux; arm variant v7

```console
$ docker pull drupal@sha256:3226423ffa6d0765721e0b770f7de1a9a26113aecdeb61b7a22214426f5adec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56394455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0bd4cd6729c54bfd94bbe3909052bcecb726ea6691ac7a9b4850e4ed037de4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:29 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Mon, 07 Aug 2023 19:57:29 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:957ee77fcb48a7e768270e3c9136e5bf3586df5345df11cfdaff931cc987af5d`  
		Last Modified: Mon, 27 Nov 2023 23:56:04 GMT  
		Size: 12.1 MB (12089657 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:860129441585641845afc1eadced14dd3af45e2f2a4dd02be4854edb9631ae06`  
		Last Modified: Mon, 27 Nov 2023 23:56:03 GMT  
		Size: 500.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6273ad80b5ecf2b166da247f157c21d0fa412bdef51427bd69de0d337555c371`  
		Last Modified: Mon, 27 Nov 2023 23:56:21 GMT  
		Size: 12.9 MB (12922604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb1e72095d8ba100195394bd9af71dd6647d332ba4f15b49d6ae2457b789a96`  
		Last Modified: Mon, 27 Nov 2023 23:56:19 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58ebb2aaf120e311554fca749103cc1b603909444509d075deced128bb1fbbcd`  
		Last Modified: Mon, 27 Nov 2023 23:56:19 GMT  
		Size: 18.8 KB (18781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46b80daefe025a231d09b6a136e0e940f7977f29c64c07a04e86637befe8e1ba`  
		Last Modified: Mon, 27 Nov 2023 23:56:19 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9321a371b932a5d7df245091bd8e3226107642ad3945106edba4abd7e7eba364`  
		Last Modified: Tue, 28 Nov 2023 03:36:16 GMT  
		Size: 1.5 MB (1547068 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50517e305bd79b6a782dd01c70de75e13a8c53a952e9492086cf156a4ce68eb1`  
		Last Modified: Tue, 28 Nov 2023 03:36:16 GMT  
		Size: 308.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47512289e99f92790e22f749b3c959d58ed8d880baca99a84dbeb098ba0ca8d8`  
		Last Modified: Tue, 28 Nov 2023 03:36:17 GMT  
		Size: 705.0 KB (705003 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a831232c28004cf27e747f8aefb20c37725a50eb5290301db7ef135cc8fc304`  
		Last Modified: Tue, 28 Nov 2023 03:36:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f37ee9d717fd7c05b681173c9cc6cce362205df68ae5024824cbfda4a3c1a101`  
		Last Modified: Tue, 28 Nov 2023 03:57:27 GMT  
		Size: 22.9 MB (22879731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:e40b150a99e7f58f2990d770cfcb59cdb6f9b1267cfb945160ca0a80a813f5d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.2 KB (309190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abce4a0f92c6bcce3cedd65ffc105f7e65a77ee19c7808b965e4d48560717724`

```dockerfile
```

-	Layers:
	-	`sha256:758a22abdd59f3d6a112821a7199d159e409ade27e8a13e8adf4971fd1c5e95b`  
		Last Modified: Tue, 28 Nov 2023 04:26:17 GMT  
		Size: 278.8 KB (278805 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cf21ff4d8f70584bacd10ad2e48240c09ff9d73d7c582542f37bb02e53fa156e`  
		Last Modified: Tue, 28 Nov 2023 04:26:17 GMT  
		Size: 30.4 KB (30385 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:3cb3e59596baf6ff139dbc849d064bc5e92ed24441b9a8f4dc1e8caa4d5b4cbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60363701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705dc1da2438cb5d6780510bff8c058a49d0dc0379035a0f87e3b7aadecd1b05`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:4d7104e80fddc06a09524f1fe96ee22799e1cc7b6744f59555bddba2c03794a2`  
		Last Modified: Mon, 27 Nov 2023 23:44:05 GMT  
		Size: 12.1 MB (12089669 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a472df87372fc1ef4dbb06b61b42886670823fec217fa5b911364a1935cd5bd`  
		Last Modified: Mon, 27 Nov 2023 23:44:04 GMT  
		Size: 498.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d001655e8dfe22ba4006fcf79659d124e49cbb280dc1841150d42656e9b53f9`  
		Last Modified: Mon, 27 Nov 2023 23:44:21 GMT  
		Size: 15.1 MB (15142955 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23a6c0ddede8d3c22f47534e0780237464d686a4c787fcea1e6f001ecd179403`  
		Last Modified: Mon, 27 Nov 2023 23:44:19 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6bae4ee6e24fc298ce3dba28090fde023de2af817e40998928c11d902ec911b`  
		Last Modified: Mon, 27 Nov 2023 23:44:19 GMT  
		Size: 18.8 KB (18785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21f1f24fdad449c78199c346c0aa75eb4bed83840e18a60247cdef3a474e3940`  
		Last Modified: Mon, 27 Nov 2023 23:44:19 GMT  
		Size: 9.2 KB (9173 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7fa12f5e8737faa130d1ea91bb2b23224d8e00cbe63751e51c2990a0861d474a`  
		Last Modified: Tue, 28 Nov 2023 03:57:12 GMT  
		Size: 2.4 MB (2445222 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:214b240a6736cae5b231127b3ed543c3c82859ab479847f0adc8cbf2cf76ab10`  
		Last Modified: Tue, 28 Nov 2023 03:57:12 GMT  
		Size: 310.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84b46923819c5cc08645096c611abf6463c8bb228401065e78a718741de14300`  
		Last Modified: Tue, 28 Nov 2023 03:57:13 GMT  
		Size: 705.0 KB (705003 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2707f61180adcd01da03fa907314d3b2e1f11f7594547d65587adcfd368c255d`  
		Last Modified: Tue, 28 Nov 2023 03:57:13 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c408ede66bb9528bac7c3b3e9c27b5b5e8fcc2e4b1277d7e606f56711488e8e8`  
		Last Modified: Tue, 28 Nov 2023 04:38:59 GMT  
		Size: 22.9 MB (22879902 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:ebcfd54aab3b709a233c220895e04ee2a2ea614fa18ee3260a2405bb6fec38cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 KB (309075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b82ebe30ec10a5b1ef14210461906c4294a122510420b6057ec71313898b2c9`

```dockerfile
```

-	Layers:
	-	`sha256:abf74fa3b560a766e6d4c2a66b38458490d0699e21c598747a7068706a9fd253`  
		Last Modified: Tue, 28 Nov 2023 04:38:58 GMT  
		Size: 278.8 KB (278786 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9a3d50cb94fa9ee7691aa7483218e6f53f0a371165caf394d9e6b9947931329c`  
		Last Modified: Tue, 28 Nov 2023 04:38:58 GMT  
		Size: 30.3 KB (30289 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-alpine3.17` - linux; 386

```console
$ docker pull drupal@sha256:002c313655d530a9faadbc141f2e6a9a641f5da8f2af519ba9dea92dee28f887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61119407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ae36a0f92616ed58cc046b384605a023548bf4855324603ed08876bbfdc3e4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.12
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:60ad002c7729a83b39395e2507ade183f70f4392a769c8b1f329e99544594c64`  
		Last Modified: Wed, 08 Nov 2023 20:27:57 GMT  
		Size: 2.3 MB (2288185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5d8057f79521a4cc5772801eaac1131e8da86c4f75c22f420e522544df6dc27`  
		Last Modified: Wed, 08 Nov 2023 20:27:57 GMT  
		Size: 312.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65a14a8542cdff43a257693d33ecf873b4730eec43d5f0ca5239032adc9eab84`  
		Last Modified: Wed, 08 Nov 2023 20:27:57 GMT  
		Size: 705.0 KB (705001 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a28a788cafd370682e1fc2df4af3ede60ea6fcb8404864abaef4b566ded4cf3d`  
		Last Modified: Wed, 08 Nov 2023 20:27:57 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6db71f1883a9a2fae7832318480d839417404713559fdfdd3f2a52d484dccb0b`  
		Last Modified: Wed, 08 Nov 2023 20:28:00 GMT  
		Size: 22.9 MB (22879924 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:205ab394f3b7b30c154dd8651645af89e0c8ced30b4dfc437452d5d6b6390779
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 KB (33932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6fa2005e9ee2c1316e6ca85dc5bd324d43460591924bbebece44974ae222d2`

```dockerfile
```

-	Layers:
	-	`sha256:085846aad1fb4eb4b1b0b44ea3f29169bd087f2781d89a4d75a8dd81231a70bf`  
		Last Modified: Wed, 08 Nov 2023 20:27:56 GMT  
		Size: 33.9 KB (33932 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-alpine3.17` - linux; ppc64le

```console
$ docker pull drupal@sha256:0a6b27b71630e7091a349524b9b4e9654621898fea5c309b985b715509a001ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.7 MB (60694240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0acb81d7f3fbc859f4b7377d8c5a1bf68d6d01aba9307627e9ae96e6ea7d70`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:5677b867a8e923419f4c954194a8136780fba8b75b7a12a11010e8da053baf8d`  
		Last Modified: Mon, 27 Nov 2023 23:56:49 GMT  
		Size: 12.1 MB (12089664 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f56fb607d6d837017a91a5955bf4bf782309c8d7b1415c0ca3fefa1540ab0cbc`  
		Last Modified: Mon, 27 Nov 2023 23:56:48 GMT  
		Size: 499.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df9e76bd3c1201d691b7a53bd99abc9d30d9d54edf46329bf4b4a4501feddffd`  
		Last Modified: Mon, 27 Nov 2023 23:57:09 GMT  
		Size: 15.7 MB (15667481 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d72a799c2fb1bdf92cf1ed1ff9a1751197c1ea3cd5d20574c1e977e2b555759`  
		Last Modified: Mon, 27 Nov 2023 23:57:06 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87180ecc8925eaf44e91c20e717d6a644f18d3f4f30fa9165aee48f30af646b8`  
		Last Modified: Mon, 27 Nov 2023 23:57:06 GMT  
		Size: 18.8 KB (18780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2c73cd1f252cc04492c283ca0d7e03221b3ce51fa6be3da3f18ef3471cd62d9`  
		Last Modified: Mon, 27 Nov 2023 23:57:06 GMT  
		Size: 9.2 KB (9178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9952687bd80a27032448a6e042a6bb9843eb87269028fedf8dabf80c9b1f27b`  
		Last Modified: Tue, 28 Nov 2023 04:36:29 GMT  
		Size: 1.9 MB (1932897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4822a69e20a020cf8398e42c2255a39e99ec5006dffebcb329bff4e737804c80`  
		Last Modified: Tue, 28 Nov 2023 04:36:29 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0d41d31df6bd6ce47d768a1536ff22d36f54a9e0e27af7f20e9deddecc4fa18`  
		Last Modified: Tue, 28 Nov 2023 04:56:30 GMT  
		Size: 705.0 KB (705002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69e504e020b9130623118d565d27971653100b2ed4000d98bdc41018e4eb4245`  
		Last Modified: Tue, 28 Nov 2023 04:56:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16041f1f7cda2c577e7be8562ea17683ca40bbb1ea0f4208690e22a8cb18d910`  
		Last Modified: Tue, 28 Nov 2023 05:27:24 GMT  
		Size: 22.9 MB (22879916 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:122517c75cd2f77b93e123e93f82f9d68bdbd530f10f438d0cce27402caadccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.5 KB (307490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68477361698026be334fbb6d8cbffce1f9eb45293cf27c601bc845e90e9dd3a7`

```dockerfile
```

-	Layers:
	-	`sha256:91780ce23c21c052e70b66f6aa42889d768284c1f88c9c4d6ccb1fed6dc31991`  
		Last Modified: Tue, 28 Nov 2023 05:27:23 GMT  
		Size: 277.2 KB (277169 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d1a0c2ff0d1c968e8a1b56f0ef3a70d80e8fa631cddf70736be9b9281001e341`  
		Last Modified: Tue, 28 Nov 2023 05:27:22 GMT  
		Size: 30.3 KB (30321 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-alpine3.17` - linux; s390x

```console
$ docker pull drupal@sha256:749ddcd56d194cd0514be0d8b267670a7620651058a3c9f2d3f9abce659a54f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58644211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8c0cc5558f4caf174c6020b92304a9fc9d5091a57ed9f0d20333cc6b632e8d2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
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
	-	`sha256:1e378647b4c3a24bcfadf9a1660bf2d49d581a2b207503c9193a4e4d81a83d5a`  
		Last Modified: Tue, 28 Nov 2023 02:15:37 GMT  
		Size: 22.9 MB (22879889 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-alpine3.17` - unknown; unknown

```console
$ docker pull drupal@sha256:4490ec282e8bca99bf54c4dbe7cd65e3e94728b05c3a3dcb8659862e9ec327e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.4 KB (307420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66d01c7feaed74b322fdfa8cf35387a42a5116cd416a87ecb0fa9b9dcc17bd0`

```dockerfile
```

-	Layers:
	-	`sha256:353d0b2f4f219a7d172136e96c70d04995f1c897d5d835e80a555cf56d9d95c8`  
		Last Modified: Tue, 28 Nov 2023 02:15:37 GMT  
		Size: 277.1 KB (277141 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7fe10736d9c62a2c9dd1eed17d4932105462ecb9579a895f2fdc53796209792e`  
		Last Modified: Tue, 28 Nov 2023 02:15:36 GMT  
		Size: 30.3 KB (30279 bytes)  
		MIME: application/vnd.in-toto+json
