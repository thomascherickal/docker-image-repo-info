## `drupal:php8.0-fpm-alpine3.15`

```console
$ docker pull drupal@sha256:0774c137b32bc736a1d083b37490bb7be88a2307a7c425cf38cbe6d6f38dcdf1
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

### `drupal:php8.0-fpm-alpine3.15` - linux; amd64

```console
$ docker pull drupal@sha256:cbccb100197cc14ee53ff9c754b3968ee602f140a60dde00426e44c2d562610d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52880016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b645c13c9cfaf9f3f98dec454bebddea3551411ee04f8573c91d596b4da0f1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:34:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 23:34:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 23:34:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 23:34:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 23:34:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 23:34:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:34:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:34:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Oct 2022 19:56:35 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 28 Oct 2022 19:56:35 GMT
ENV PHP_VERSION=8.0.25
# Fri, 28 Oct 2022 19:56:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 28 Oct 2022 19:56:35 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 28 Oct 2022 19:56:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 28 Oct 2022 19:56:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:04:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Oct 2022 20:04:31 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:04:32 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Oct 2022 20:04:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Oct 2022 20:04:33 GMT
WORKDIR /var/www/html
# Fri, 28 Oct 2022 20:04:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 28 Oct 2022 20:04:33 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Oct 2022 20:04:34 GMT
EXPOSE 9000
# Fri, 28 Oct 2022 20:04:34 GMT
CMD ["php-fpm"]
# Fri, 28 Oct 2022 21:20:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 28 Oct 2022 21:20:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Oct 2022 21:20:09 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 28 Oct 2022 21:20:09 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 28 Oct 2022 21:20:09 GMT
WORKDIR /opt/drupal
# Fri, 28 Oct 2022 21:20:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 28 Oct 2022 21:20:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442a61c63ceec3c20b6f19e35cb326055977dd34ecd556ce0b1f259b4deb2811`  
		Last Modified: Fri, 07 Oct 2022 01:01:58 GMT  
		Size: 1.7 MB (1714315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ecb9ad4887ee043c35bdc43fbcbe19410538db2a2dfcc338b7a19d667f6b0d`  
		Last Modified: Fri, 07 Oct 2022 01:01:58 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa18066724a6bc8d6344f4910a873654708fdaaedc58dadef81ecfa31625752`  
		Last Modified: Fri, 07 Oct 2022 01:01:57 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6ce66691c2a9afafcc4f26f2287f96a17b07054d29239436f3b7d888d0faa`  
		Last Modified: Fri, 28 Oct 2022 20:23:15 GMT  
		Size: 10.8 MB (10823056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4e8b23fea234d92db5ca8f09fea3db09d1bdff6304b6f5f3b91121629334f1`  
		Last Modified: Fri, 28 Oct 2022 20:23:14 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbabce31665c8cbc52d00adda465bef596ee40458162069f3deef11a1b68ac0c`  
		Last Modified: Fri, 28 Oct 2022 20:23:33 GMT  
		Size: 12.3 MB (12300759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab592875b03d8d4924c0013fbcb3f3bf0202d62d499db8075bffe8030963ac1`  
		Last Modified: Fri, 28 Oct 2022 20:23:31 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671946f07085637b9215bb9422823780fd546155d32da2cbadbf8f5469058b8a`  
		Last Modified: Fri, 28 Oct 2022 20:23:31 GMT  
		Size: 18.7 KB (18727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2208b4985147164d065663439df351298317439dc3b871b24e733cd1fd56f380`  
		Last Modified: Fri, 28 Oct 2022 20:23:31 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95afbaac18786c395c4ff7d27dfd7fb5159b4152fd455d1fc213d3135a20f7b6`  
		Last Modified: Fri, 28 Oct 2022 21:41:31 GMT  
		Size: 2.6 MB (2593251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9346e6b2a553b9063d0f3cfc2771c1f828fb424b089e285800408ec7eceac5aa`  
		Last Modified: Fri, 28 Oct 2022 21:41:30 GMT  
		Size: 321.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa70ece5f39d6142ad0c1dd29015ba01156c4ac9108d9786268766ed4c9a435`  
		Last Modified: Fri, 28 Oct 2022 21:41:31 GMT  
		Size: 695.2 KB (695181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119c339c37ab47058af1289022d0590e2116b1021bad74977736541073f714c9`  
		Last Modified: Fri, 28 Oct 2022 21:41:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e62ee910fdcd859d6e4acba464553c261c534f6ef8eb4b2638f5d3a63453c4`  
		Last Modified: Fri, 28 Oct 2022 21:41:36 GMT  
		Size: 21.9 MB (21897698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.15` - linux; arm variant v6

```console
$ docker pull drupal@sha256:3a6c5bef316644ed5e4994afe38aca3923040b0069c730cb0d20daddb95f39d7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52040659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb8f43f7eae1d65b405ef17dfa5bb36395c8f07d3fa3e4ca37a14f4b74e2b3e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 05:34:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 11 Nov 2022 05:34:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 11 Nov 2022 05:34:45 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 11 Nov 2022 05:34:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Nov 2022 05:34:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Nov 2022 05:34:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Nov 2022 05:34:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Nov 2022 05:34:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Nov 2022 06:20:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 11 Nov 2022 06:20:26 GMT
ENV PHP_VERSION=8.0.25
# Fri, 11 Nov 2022 06:20:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 11 Nov 2022 06:20:26 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 11 Nov 2022 06:20:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 11 Nov 2022 06:20:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Nov 2022 06:27:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Nov 2022 06:27:39 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 11 Nov 2022 06:27:40 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Nov 2022 06:27:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Nov 2022 06:27:41 GMT
WORKDIR /var/www/html
# Fri, 11 Nov 2022 06:27:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Nov 2022 06:27:41 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Nov 2022 06:27:41 GMT
EXPOSE 9000
# Fri, 11 Nov 2022 06:27:41 GMT
CMD ["php-fpm"]
# Fri, 11 Nov 2022 12:46:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 11 Nov 2022 12:46:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 11 Nov 2022 12:46:27 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 11 Nov 2022 12:46:27 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 11 Nov 2022 12:46:27 GMT
WORKDIR /opt/drupal
# Fri, 11 Nov 2022 12:46:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 11 Nov 2022 12:46:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6930cede459fa8f23f7b3f26a9d8abc4beffdea4d3c3743041b8e94fbf674d8`  
		Last Modified: Fri, 11 Nov 2022 07:01:06 GMT  
		Size: 1.7 MB (1703994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407b25a2a074978c2a25e52feb214ba44cfb832f8e64e8ae7ff0a5ee3faa64da`  
		Last Modified: Fri, 11 Nov 2022 07:01:05 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af096e8217aeda7d39eda90fc3452672311a5dd216ac7c937b7f4a7f229dafe`  
		Last Modified: Fri, 11 Nov 2022 07:01:05 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e068dfdd691642e4bbd5f1c1c5191f67424e913fcf3d9c5ff9f517c5a9b10`  
		Last Modified: Fri, 11 Nov 2022 07:07:01 GMT  
		Size: 10.8 MB (10823058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cdfc0a64b803ed0ec6b9c74907163729eba8755c48739b34f547d5d3845112`  
		Last Modified: Fri, 11 Nov 2022 07:07:00 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e21da98e02b7a0347339bf5ad4feef6c74ec5d5dfb2693a1fcf2421eae1ee7`  
		Last Modified: Fri, 11 Nov 2022 07:07:25 GMT  
		Size: 12.2 MB (12219612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085b788a89aa8971e8b3929fd883a4ff3072b18a76843efe546db933d0b00624`  
		Last Modified: Fri, 11 Nov 2022 07:07:22 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d368e18179dc055b91234430fd2625b0c944ac4406f74573afa7a1ba8adafe2`  
		Last Modified: Fri, 11 Nov 2022 07:07:22 GMT  
		Size: 18.7 KB (18695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e220c1b04e61aeeec69438a886ec8b22cd497a6fa74cd79bab95b6b0e75d9cb0`  
		Last Modified: Fri, 11 Nov 2022 07:07:22 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6c4fe7a1bef298a7d30b475be638dd420691f0e2061e82e361d261a601ddd1`  
		Last Modified: Fri, 11 Nov 2022 13:01:33 GMT  
		Size: 2.0 MB (2037945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff49ffbeec73953759076e80689212ed39b944c031ba855a9d89752b5a27814`  
		Last Modified: Fri, 11 Nov 2022 13:01:33 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f58de1e077b8a6971b037614fcad63fc7cf378eae54df5dfefeceff0c309d8`  
		Last Modified: Fri, 11 Nov 2022 13:01:33 GMT  
		Size: 695.2 KB (695182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cc4b1d536518bdb992b31229b266c162207ae3370cffcd7fc8ff29b6009016`  
		Last Modified: Fri, 11 Nov 2022 13:01:33 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921be7eb82f9139da0c3b8a37adb421fd7be22c74a111e0054bb3c385f88149`  
		Last Modified: Fri, 11 Nov 2022 13:01:41 GMT  
		Size: 21.9 MB (21897641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.15` - linux; arm variant v7

```console
$ docker pull drupal@sha256:6a9ec385e1cd7a78eb2a9a0c673e7490abe1d40c275d83ae0d1e7a2672913d70
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49870548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0427d0e21a304d428ca39521b52f6a13b61fe9c2cd47059985f5f666075c8a07`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 00:18:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 26 Oct 2022 00:18:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 26 Oct 2022 00:18:05 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 26 Oct 2022 00:18:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Oct 2022 00:18:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Oct 2022 00:18:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Oct 2022 00:18:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Oct 2022 00:18:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Oct 2022 19:34:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 28 Oct 2022 19:34:44 GMT
ENV PHP_VERSION=8.0.25
# Fri, 28 Oct 2022 19:34:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 28 Oct 2022 19:34:45 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 28 Oct 2022 19:34:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 28 Oct 2022 19:34:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Oct 2022 19:42:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Oct 2022 19:42:24 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Oct 2022 19:42:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Oct 2022 19:42:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Oct 2022 19:42:25 GMT
WORKDIR /var/www/html
# Fri, 28 Oct 2022 19:42:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 28 Oct 2022 19:42:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Oct 2022 19:42:26 GMT
EXPOSE 9000
# Fri, 28 Oct 2022 19:42:26 GMT
CMD ["php-fpm"]
# Fri, 28 Oct 2022 20:36:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 28 Oct 2022 20:36:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Oct 2022 20:36:41 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:36:41 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 28 Oct 2022 20:36:41 GMT
WORKDIR /opt/drupal
# Fri, 28 Oct 2022 20:36:57 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 28 Oct 2022 20:36:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7799733802847967d1737565864607db569fc9d474807963f8bd9e43ebc3ada`  
		Last Modified: Wed, 26 Oct 2022 03:40:34 GMT  
		Size: 1.6 MB (1571630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73bc60ead6a73f4fb88af62246bd08151563acc48dda72513c26e08ce9ac2ae`  
		Last Modified: Wed, 26 Oct 2022 03:40:33 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f91a6dfd19d77843a8d8a69f8cc88f1cceb9f7c98118cdcb05891ce7ff4836`  
		Last Modified: Wed, 26 Oct 2022 03:40:33 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a642c4be4ddb474d91a041966f3bccd7ef82638dffd7485828bc64b4d4a9176b`  
		Last Modified: Fri, 28 Oct 2022 20:14:29 GMT  
		Size: 10.8 MB (10823036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e965dda37698f04e5c509432d5941a09f87379810004accfc9e7981f85e6bdf4`  
		Last Modified: Fri, 28 Oct 2022 20:14:26 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ca5b9c79a4f108241671da665f5afc96d1a206b33e320885a942c68e52b44`  
		Last Modified: Fri, 28 Oct 2022 20:14:51 GMT  
		Size: 10.5 MB (10541565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3148a8324134a1e02c59911083a7a5ee2d85eedc09f4f76077d5a21eca3b0be`  
		Last Modified: Fri, 28 Oct 2022 20:14:49 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea63e7d70b94c76ddce6dc05ecc902ad1e389ea8f14721a6fd932ae3bf4c166`  
		Last Modified: Fri, 28 Oct 2022 20:14:49 GMT  
		Size: 18.7 KB (18705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bb718db926421b42564b84b7a275c231c67c7baf59e0b0ca3be6760177f46f`  
		Last Modified: Fri, 28 Oct 2022 20:14:49 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c48069cdf3e83adf6260e7fbba8187b9346f2edd7135e69f3057fcf135c6a`  
		Last Modified: Fri, 28 Oct 2022 21:20:49 GMT  
		Size: 1.9 MB (1874234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ec0dbbb9df731af3eefd2bb537226b5795bcea5a09f834453d12da44e994cc`  
		Last Modified: Fri, 28 Oct 2022 21:20:49 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f67af7abb0770dc5dd14ee6299d4daa1fcefe44b835a9e315341d8d1af56431`  
		Last Modified: Fri, 28 Oct 2022 21:20:49 GMT  
		Size: 695.2 KB (695179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3befe628a96577004b61c14f2bd1b77bab68e31f7b43577edb702991c58d6a`  
		Last Modified: Fri, 28 Oct 2022 21:20:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325a2904b91910f19e7e66b4690439a0186800f6f386d79d24ba0c4121f044d2`  
		Last Modified: Fri, 28 Oct 2022 21:20:57 GMT  
		Size: 21.9 MB (21897696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:c7e9ddb27002ab2f70a9cb57cbfa04440f93d57a8ea83321bace4431cbcdc366
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53001656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98c3f2341400dae5edad5d49977887e92cc76f4c9f662abc893802e9d371f82`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 09:34:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 11 Nov 2022 09:34:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 11 Nov 2022 09:34:54 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 11 Nov 2022 09:34:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Nov 2022 09:34:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Nov 2022 09:34:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Nov 2022 09:34:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Nov 2022 09:34:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Nov 2022 10:19:22 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 11 Nov 2022 10:19:22 GMT
ENV PHP_VERSION=8.0.25
# Fri, 11 Nov 2022 10:19:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 11 Nov 2022 10:19:22 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 11 Nov 2022 10:19:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 11 Nov 2022 10:19:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Nov 2022 10:24:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Nov 2022 10:24:24 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 11 Nov 2022 10:24:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Nov 2022 10:24:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Nov 2022 10:24:26 GMT
WORKDIR /var/www/html
# Fri, 11 Nov 2022 10:24:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Nov 2022 10:24:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Nov 2022 10:24:26 GMT
EXPOSE 9000
# Fri, 11 Nov 2022 10:24:26 GMT
CMD ["php-fpm"]
# Fri, 11 Nov 2022 12:53:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 11 Nov 2022 12:53:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 11 Nov 2022 12:53:35 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 11 Nov 2022 12:53:35 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 11 Nov 2022 12:53:35 GMT
WORKDIR /opt/drupal
# Fri, 11 Nov 2022 12:53:45 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 11 Nov 2022 12:53:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5acfa70a19877408a767c3496a70a7f9044442b68a6eac3bf2a541032cdb7e`  
		Last Modified: Fri, 11 Nov 2022 10:51:31 GMT  
		Size: 1.7 MB (1715309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da01d3647a74c1f480632ff5a528f948030d7bcf445b74d0513481ff0a81720a`  
		Last Modified: Fri, 11 Nov 2022 10:51:32 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0915366a71de4e5af5c675c00400d106a8d23a490e0500ee6e0e252fed1dfd7`  
		Last Modified: Fri, 11 Nov 2022 10:51:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e3b65cbafcdc4a3a707b5e559a3e9599bfacb210fe5ff959bd8016785b189f`  
		Last Modified: Fri, 11 Nov 2022 10:56:40 GMT  
		Size: 10.8 MB (10823078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87bec13cb0c5ff63b13525ea8464ce5a4911b972fc01f33312fd2896df00a4b`  
		Last Modified: Fri, 11 Nov 2022 10:56:39 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122bac2248c978cf968e30c949494eb137a3e3c0fa775dd2ba392d9ec9dae5ef`  
		Last Modified: Fri, 11 Nov 2022 10:56:58 GMT  
		Size: 12.9 MB (12902169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd2157d8a260ff4f31414fbbfc42fa1fd29013a2851098696acaae5163acbb3`  
		Last Modified: Fri, 11 Nov 2022 10:56:56 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48327c6d46ccec42e475ee92ab3ba64bb373393d7fd4bb50b56eee5e523e98ef`  
		Last Modified: Fri, 11 Nov 2022 10:56:56 GMT  
		Size: 18.7 KB (18693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78f6ce6ec0120fefee8380f06399240db87714c687fe6467fdd7cffb434453c`  
		Last Modified: Fri, 11 Nov 2022 10:56:56 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b268d327ac1421fe04816ea2d390760fded8f768ff1c5c111389e31d6fc0959`  
		Last Modified: Fri, 11 Nov 2022 13:07:20 GMT  
		Size: 2.2 MB (2217688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa587ae5c38ba63eac90d93d320812d79cf4d23e7d1791beb422e043977abc0`  
		Last Modified: Fri, 11 Nov 2022 13:07:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95dad002a3d35599d2637ab493e82a4b37cfc3efd15d0f16af2e309e828c41c`  
		Last Modified: Fri, 11 Nov 2022 13:07:20 GMT  
		Size: 695.2 KB (695183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7033f2c03129b770caf59309be4455e8b88fe038d10b05267828c426ce32b24d`  
		Last Modified: Fri, 11 Nov 2022 13:07:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9167ee57d1ce5d9c2b5c7ef0c599638d6792907fe4078308105f9af723961992`  
		Last Modified: Fri, 11 Nov 2022 13:07:24 GMT  
		Size: 21.9 MB (21897578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.15` - linux; 386

```console
$ docker pull drupal@sha256:b9f8a808e11dd93094de23de8a0f08ef42b19d19cb00ed7fc7f2d960a29fbf3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53315185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490e8e0d673f32be320d3fb4176d7e59d07679a1754a51cc416403a3788aaee8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:14:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 21:14:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 21:14:21 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 21:14:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 21:14:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 21:14:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 21:14:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 21:14:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Oct 2022 20:20:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 28 Oct 2022 20:20:24 GMT
ENV PHP_VERSION=8.0.25
# Fri, 28 Oct 2022 20:20:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 28 Oct 2022 20:20:26 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 28 Oct 2022 20:20:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 28 Oct 2022 20:20:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:27:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Oct 2022 20:27:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:27:23 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Oct 2022 20:27:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Oct 2022 20:27:25 GMT
WORKDIR /var/www/html
# Fri, 28 Oct 2022 20:27:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 28 Oct 2022 20:27:27 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Oct 2022 20:27:28 GMT
EXPOSE 9000
# Fri, 28 Oct 2022 20:27:29 GMT
CMD ["php-fpm"]
# Fri, 28 Oct 2022 21:34:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 28 Oct 2022 21:34:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Oct 2022 21:35:01 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 28 Oct 2022 21:35:01 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 28 Oct 2022 21:35:02 GMT
WORKDIR /opt/drupal
# Fri, 28 Oct 2022 21:35:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 28 Oct 2022 21:35:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bc5695a671be5ab49e8ef9515c45bac9868ef6942e7eba7847b6da07ad66a3`  
		Last Modified: Thu, 06 Oct 2022 22:47:55 GMT  
		Size: 1.8 MB (1814937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1cf10e2861b18fd0893eede83d16bb09da2377a48f51f2548edc988b8671c1`  
		Last Modified: Thu, 06 Oct 2022 22:47:54 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a46660760b73ac2d1b70f96a2768c2d134fe41fb72e20f52e83e1c4836ecaac`  
		Last Modified: Thu, 06 Oct 2022 22:47:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcd28438445f5a4474352f85140cc6cdb1c1b61ad2782a1cb3549f01dc14775`  
		Last Modified: Fri, 28 Oct 2022 20:54:12 GMT  
		Size: 10.8 MB (10822826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8193a331eb5019783fe8a58fe5bffb1a37b9913e484ba6cfdf7b1fa31070403e`  
		Last Modified: Fri, 28 Oct 2022 20:54:10 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deb6a82fe131b0d84aaad618ed1663092bfa89a4a9c4af991fbf3ba871bdc0b`  
		Last Modified: Fri, 28 Oct 2022 20:54:33 GMT  
		Size: 12.6 MB (12587894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c75b3e9177348d1d1dcba5bfbb21e7c5a1d4078122dec432a656baa129fd8a`  
		Last Modified: Fri, 28 Oct 2022 20:54:31 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecbec363a27a7673a3dd0e6f27333d350f40bb82ab6d4a21e287d80a1aa6b2`  
		Last Modified: Fri, 28 Oct 2022 20:54:31 GMT  
		Size: 18.6 KB (18624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770dec215e90704ec57d8ed240e1b2f874e3082da6450a384d89843504d18c1`  
		Last Modified: Fri, 28 Oct 2022 20:54:31 GMT  
		Size: 8.6 KB (8567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19eb19f750d95cde944ba7ad856ffa69bec53c5778131e140120c409b6dce2e`  
		Last Modified: Fri, 28 Oct 2022 22:07:36 GMT  
		Size: 2.6 MB (2635136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62419603fb159cfacff1518e5a1b269f926690bf8f05583451fac90998a2a31`  
		Last Modified: Fri, 28 Oct 2022 22:07:35 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11136fa52a2936455df85d9b53f8d46a162d5829b4283a26549737e71d79ab61`  
		Last Modified: Fri, 28 Oct 2022 22:07:36 GMT  
		Size: 695.2 KB (695184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f7c16c3760f3857e2b02e7834e50e4c7e17c3281351d7d819b12f8ca7b5520`  
		Last Modified: Fri, 28 Oct 2022 22:07:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935b7b79c3a3c2629f13e81a8482d4f3d9672e55972f0e1fe8ed15b82398824c`  
		Last Modified: Fri, 28 Oct 2022 22:07:41 GMT  
		Size: 21.9 MB (21898662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.15` - linux; ppc64le

```console
$ docker pull drupal@sha256:f5e9be45a3d91ea63aa09c29cd66710c73549b3401a011ed92f2f99974434c24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53213939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8d451af335f03222f4b94ac22ec020dc045250ce5bf3839e39e01871a06987`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 00:16:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 00:16:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 00:16:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 00:16:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 00:16:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 00:16:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 00:16:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 00:16:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Oct 2022 19:55:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 28 Oct 2022 19:55:33 GMT
ENV PHP_VERSION=8.0.25
# Fri, 28 Oct 2022 19:55:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 28 Oct 2022 19:55:33 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 28 Oct 2022 19:55:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 28 Oct 2022 19:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:05:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Oct 2022 20:05:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:05:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Oct 2022 20:05:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Oct 2022 20:05:28 GMT
WORKDIR /var/www/html
# Fri, 28 Oct 2022 20:05:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 28 Oct 2022 20:05:30 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Oct 2022 20:05:30 GMT
EXPOSE 9000
# Fri, 28 Oct 2022 20:05:30 GMT
CMD ["php-fpm"]
# Fri, 28 Oct 2022 21:11:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 28 Oct 2022 21:11:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Oct 2022 21:11:45 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 28 Oct 2022 21:11:45 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 28 Oct 2022 21:11:46 GMT
WORKDIR /opt/drupal
# Fri, 28 Oct 2022 21:12:10 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 28 Oct 2022 21:12:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95c73f7a3c32a8bc59a8cfd4ba6b491407a1ab76333dff422ca76f9b298f4f`  
		Last Modified: Fri, 07 Oct 2022 02:14:32 GMT  
		Size: 1.8 MB (1762301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8742d5d79b941a6dbaebe4c0c07389415e5fc9874cf767d1a09a4e847c89ad55`  
		Last Modified: Fri, 07 Oct 2022 02:14:32 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1140a353543e91674064708467958bbfae46120db8560786aeafd2cae15c784c`  
		Last Modified: Fri, 07 Oct 2022 02:14:32 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fabc3951c2a427765ad543d3fd68294bd5ce17b3711ac47badbcfe77476492`  
		Last Modified: Fri, 28 Oct 2022 20:30:14 GMT  
		Size: 10.8 MB (10823072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5e1b2529be529f91d8c5cbf8bf67f09594d9d16a56ba55f7675bab2693e02e`  
		Last Modified: Fri, 28 Oct 2022 20:30:13 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdb1baa1e9c64ba358434192ef47a7da130fcfbaedc3cc10e202ac9ac6d2cac`  
		Last Modified: Fri, 28 Oct 2022 20:32:54 GMT  
		Size: 12.7 MB (12719167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1201eb889d2c99577c0eee4e480ff27c49a92fb42d7806b1dbeb1545b4c1a6`  
		Last Modified: Fri, 28 Oct 2022 20:32:50 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757c23721197029407b383448b01f266971a4d907dd78a96a3e00bf228fdca2e`  
		Last Modified: Fri, 28 Oct 2022 20:32:50 GMT  
		Size: 18.7 KB (18719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076109074ae0f08669de6ad3bacccaab49256c6ceec8e37940dfd30968b29ed7`  
		Last Modified: Fri, 28 Oct 2022 20:32:50 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7cd9d8f10f2f4af2be585edbef5a0c9eebbdbc1f0663d1dc6d17b90a2fd80f`  
		Last Modified: Fri, 28 Oct 2022 21:43:11 GMT  
		Size: 2.5 MB (2471322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e5ce27c4a7ee66ffc9a079a494e52d94d23d3ec987d1160b372dc8a10137fc`  
		Last Modified: Fri, 28 Oct 2022 21:43:11 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b981c4b89e38781fb9a0d4a9759384df982f2ca017f189bf506d2d9629a1216`  
		Last Modified: Fri, 28 Oct 2022 21:43:11 GMT  
		Size: 695.2 KB (695181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c6b3559a89821ec76703a953e59ce91a92d09570a831b2c82e55804579a97b`  
		Last Modified: Fri, 28 Oct 2022 21:34:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823b5cfe0b6c08fd3b0bedb3ce009385115b5ad3f0ae1e57d4cc8137f1c78991`  
		Last Modified: Fri, 28 Oct 2022 21:43:34 GMT  
		Size: 21.9 MB (21897666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.15` - linux; s390x

```console
$ docker pull drupal@sha256:1d5ad84180808cd69b703e28a24841ba981ff1d27f6081104149f57d8b410580
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51656923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32131d907764c6759b538529aa7012095f8f1f28c5a143e13097be5efd5a0e16`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:41:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 01:41:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 01:41:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 01:41:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 01:41:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 01:41:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 01:41:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 01:41:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Oct 2022 19:30:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Fri, 28 Oct 2022 19:30:24 GMT
ENV PHP_VERSION=8.0.25
# Fri, 28 Oct 2022 19:30:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.25.tar.xz.asc
# Fri, 28 Oct 2022 19:30:24 GMT
ENV PHP_SHA256=a291b71d0498707fc5514eb5b9513e88f0f1d4890bcdefd67282ded8a2bfb941
# Fri, 28 Oct 2022 19:30:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 28 Oct 2022 19:30:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Oct 2022 19:36:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Oct 2022 19:36:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Oct 2022 19:36:29 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Oct 2022 19:36:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Oct 2022 19:36:29 GMT
WORKDIR /var/www/html
# Fri, 28 Oct 2022 19:36:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 28 Oct 2022 19:36:30 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Oct 2022 19:36:30 GMT
EXPOSE 9000
# Fri, 28 Oct 2022 19:36:30 GMT
CMD ["php-fpm"]
# Fri, 28 Oct 2022 20:26:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 28 Oct 2022 20:26:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Oct 2022 20:26:24 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 28 Oct 2022 20:26:24 GMT
ENV DRUPAL_VERSION=9.4.8
# Fri, 28 Oct 2022 20:26:24 GMT
WORKDIR /opt/drupal
# Fri, 28 Oct 2022 20:26:35 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 28 Oct 2022 20:26:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4016245521e8cb672f9b3d3192e643407660e1415a632bc4b0c2a90e3623d58`  
		Last Modified: Fri, 07 Oct 2022 03:28:01 GMT  
		Size: 1.8 MB (1774941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74f4aa98ca85719e45f5094ba35ecb50114c5487399b322bca2000d6b216608`  
		Last Modified: Fri, 07 Oct 2022 03:28:01 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d3c1f2848261ceb82465b2fca705caae3fdfdfaf9e7d96134d73bfeb6855f3`  
		Last Modified: Fri, 07 Oct 2022 03:28:01 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb6f5e7cd4ad2e8284946ef6cd085128d1a3edc6a10c235599528ba2fb2124d`  
		Last Modified: Fri, 28 Oct 2022 19:55:03 GMT  
		Size: 10.8 MB (10823069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009c3b796720fa72151ce48c717572b447f69c5e9c92713c81adb35ed4e2629`  
		Last Modified: Fri, 28 Oct 2022 19:55:02 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e1390cfac37acb55ed092c32d31d3417185c0f813917ac9216dc9c1b180208`  
		Last Modified: Fri, 28 Oct 2022 19:55:18 GMT  
		Size: 11.6 MB (11564498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55aa0ccc963bc8f07b238599984d1d197496b5d1d6bbc3d4fb0033c30b3e46bd`  
		Last Modified: Fri, 28 Oct 2022 19:55:16 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab48124dd28da4ff7d73a8894373c09a14411860b630e2370d91ed2d51d733e9`  
		Last Modified: Fri, 28 Oct 2022 19:55:16 GMT  
		Size: 18.7 KB (18738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b4671474c57e472b88351e0d62814c2eb286f053b6791f1906231aafec60c`  
		Last Modified: Fri, 28 Oct 2022 19:55:16 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ecfff7985e48c68317166d95dc8e47f0e5a2e816c92a23d9fba02d81bda024`  
		Last Modified: Fri, 28 Oct 2022 20:46:43 GMT  
		Size: 2.3 MB (2263235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8908f9b590ed725de2ff64145dd8794674a8c1cfe378b5c0a09ceba35ba66475`  
		Last Modified: Fri, 28 Oct 2022 20:46:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eab2f3f4fe5b5abf5137b95170126524677315f003caaa88529b5fdd6881ea`  
		Last Modified: Fri, 28 Oct 2022 20:46:43 GMT  
		Size: 695.2 KB (695184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8acf1fd2711060be0f217466f6dda3b5a796e9221238534ac1139b21871aa`  
		Last Modified: Fri, 28 Oct 2022 20:46:43 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2004a0586d5f71b5c33aa48e370c09a2ec523728e58a17d1a6f48ec1abac5797`  
		Last Modified: Fri, 28 Oct 2022 20:46:47 GMT  
		Size: 21.9 MB (21897655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
