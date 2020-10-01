## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:40c82d17ec3c74c5349255552472f3208756f7c8d267da6cc017cedbe7cca89d
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

### `adminer:fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:9c42b4c000a7b48d4de981c0ec8cb26ccede6fc17e87ff5f45722ffe454d3696
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34013658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec4db9a39ef16695ffcadadd033f77a0c524d1753ca032ae2d4b0fcf5811fff`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 19:00:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 19:00:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:00:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:00:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 19:00:54 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 19:53:09 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 19:53:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 19:53:09 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 19:53:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:53:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:01:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:01:20 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:01:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:01:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:01:21 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 20:01:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 20:01:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 20:01:23 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 20:01:23 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 23:18:29 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 23:18:30 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 23:18:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 23:18:58 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 23:18:58 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 23:18:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 23:18:58 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 23:19:00 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 23:19:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 23:19:00 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 23:19:00 GMT
USER adminer
# Thu, 03 Sep 2020 23:19:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3732f4f24f83b49c19059c39a2a2258206dd16ce2bb7c4254dc2994f106fc73`  
		Last Modified: Thu, 03 Sep 2020 22:51:29 GMT  
		Size: 10.3 MB (10317338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb8848bd3048f554f1c32203ea5c7715d9fa4001940aa6e89054b474a651c64`  
		Last Modified: Thu, 03 Sep 2020 22:51:27 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ca18042f4430e5bed3734b4759e16d5295e971641e0f8ff906576e7f2a9c9c`  
		Last Modified: Thu, 03 Sep 2020 22:51:32 GMT  
		Size: 14.6 MB (14632991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdaa57ecb0d84b37792506b80b8a2851bde1d47f0b295b349e31f24531dff13`  
		Last Modified: Thu, 03 Sep 2020 22:51:27 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e8ed5f1133d3b0aafcc612ad4e086f3af8f07c5488a50f6daa032c97aceef`  
		Last Modified: Thu, 03 Sep 2020 22:51:27 GMT  
		Size: 17.0 KB (17018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206bc7d2ac834db51386e667aaac3606eb29eb7e2afa2b4d682712e5ecaac2a0`  
		Last Modified: Thu, 03 Sep 2020 22:51:27 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d6ab60779c710e322e757bd6fe0ccc63536cff184afc3b0b8bfe813d4c882`  
		Last Modified: Thu, 03 Sep 2020 23:19:28 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4f9b7e030c94e8d0f4d969a0322ad22642768c3a096abd18d76daca094919c`  
		Last Modified: Thu, 03 Sep 2020 23:19:28 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615e70b253b6feff374f09a1e1c98ba545b8bad5654c60e7a85be6a70e681931`  
		Last Modified: Thu, 03 Sep 2020 23:19:29 GMT  
		Size: 4.3 MB (4320976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650528f2f5ffcb17f3fc507e129959e445d86b2830367fb8fe59a1d0d77a35bc`  
		Last Modified: Thu, 03 Sep 2020 23:19:28 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d519eda2fdee10308dfa256e20a80dc95b03a505d8e4625039b5bccfe107e99`  
		Last Modified: Thu, 03 Sep 2020 23:19:28 GMT  
		Size: 570.7 KB (570684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a05c3952d0f5477d2f20539d962aff98cf6be811ebd6be240da2aacb9baeada`  
		Last Modified: Thu, 03 Sep 2020 23:19:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v6

```console
$ docker pull adminer@sha256:9c42f336d5c11f6e4fbfa77f94e126800b450e1cc3d199b7a0b63a3650abae25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32511248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1fb3fbdacb31ce895404ebca33c34ab31db0dc129092cc0423e26a090e1d3c8`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:20:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:20:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:20:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:20:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:20:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 19:15:15 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 19:15:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 19:15:38 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 19:16:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:16:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:21:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 19:21:46 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:22:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 19:22:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 19:22:50 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 19:23:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 19:23:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 19:24:00 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 19:24:10 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 22:10:03 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 22:10:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 22:12:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 22:12:26 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 22:12:36 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 22:12:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 22:13:03 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 22:13:51 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 22:14:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:14:26 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 22:14:40 GMT
USER adminer
# Thu, 03 Sep 2020 22:14:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5713afad55adb5542a74cb3d581dd5a174abd90eb7e074131c5e4cf7675796`  
		Last Modified: Thu, 03 Sep 2020 20:58:02 GMT  
		Size: 10.3 MB (10317371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f420acb2d594e5d4c5ab10aa702fbaedd1ba33577ae8b62f6169d80e130333`  
		Last Modified: Thu, 03 Sep 2020 20:57:57 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5785457fe29efc913ffa288540f3563aa361f9cc7ee908847d1a15f946169a1`  
		Last Modified: Thu, 03 Sep 2020 20:58:02 GMT  
		Size: 13.7 MB (13651850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91c4d328622ebf9dade0f65f6c4849810ce6bcd45f26545e190e21057ec149`  
		Last Modified: Thu, 03 Sep 2020 20:57:56 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee4cfd9f59647f321f8d34f96adf50b3ca3c74e5997a8d335ce222acaf98b02`  
		Last Modified: Thu, 03 Sep 2020 20:57:56 GMT  
		Size: 17.0 KB (16973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3821eae7a11b075e5f26f360de2dbc9409ee04692820ef12a1ccc95486bf1`  
		Last Modified: Thu, 03 Sep 2020 20:57:56 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c910718c23cb7b88b2ed5c950772b5e679ae8cf877d6232d2032215a0ab2630`  
		Last Modified: Thu, 03 Sep 2020 22:16:01 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdba6a61933fe6dfad334b90833aad040c7b15bee32eafced6cc4850cf832862`  
		Last Modified: Thu, 03 Sep 2020 22:15:58 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca80ea7add6e121a4f4247d21921b0807f6959b7a2a1c81804ad872c1c62380`  
		Last Modified: Thu, 03 Sep 2020 22:15:58 GMT  
		Size: 4.0 MB (4024287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f592b5130ecd2cde24f3a54b1fc6fd35f2b6c82b4a0b8441d589c39415f8275f`  
		Last Modified: Thu, 03 Sep 2020 22:15:58 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20d57e5026586b9990d055447d5bbc0d74e041ff9292ef9a586bfb1d69c437`  
		Last Modified: Thu, 03 Sep 2020 22:15:58 GMT  
		Size: 570.8 KB (570776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09bb1f84735863fa3ee9bc37f7ca53b2743d6a5b7e032a178fbbdb2c78e6f6b`  
		Last Modified: Thu, 03 Sep 2020 22:15:58 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:14e0afdc71189e4207731b20763adae90454205a62d4e1866aa00a89371d7c7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31236487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f0c3416b7242f9bdef88a98422911dae9d69686591cd2ae3be7c9da7c80e366`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:38:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:38:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:38:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:38:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:38:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 20:55:05 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 20:55:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 20:55:20 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 20:55:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:56:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:59:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 21:00:12 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 21:00:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 21:00:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 21:01:05 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 21:01:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 21:01:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 21:01:54 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 21:02:01 GMT
CMD ["php-fpm"]
# Fri, 04 Sep 2020 01:38:35 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 04 Sep 2020 01:39:05 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 04 Sep 2020 01:40:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 04 Sep 2020 01:40:53 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 04 Sep 2020 01:41:01 GMT
ENV ADMINER_VERSION=4.7.7
# Fri, 04 Sep 2020 01:41:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Fri, 04 Sep 2020 01:41:17 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Fri, 04 Sep 2020 01:41:51 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 04 Sep 2020 01:42:09 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 04 Sep 2020 01:42:21 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 04 Sep 2020 01:42:35 GMT
USER adminer
# Fri, 04 Sep 2020 01:42:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd053e856fd9851b47d3e4ba722958e2941002353eb3941bfe1f10f4950e701d`  
		Last Modified: Thu, 03 Sep 2020 23:29:47 GMT  
		Size: 10.3 MB (10317354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562f5c922a943495cfe3aea57723aa3a62c34ed20caef1df6e6f2c704ad2f57b`  
		Last Modified: Thu, 03 Sep 2020 23:29:41 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ea77b063adfde562dff3ffaf7913100c0d1578b6675dfeabdcb0d0e69ff374`  
		Last Modified: Thu, 03 Sep 2020 23:29:47 GMT  
		Size: 12.8 MB (12771737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01828949796000635a0595d51d33f9702ab8e29d69b5cc9a759e45b10b1bca97`  
		Last Modified: Thu, 03 Sep 2020 23:29:41 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e9e0b4846dcb6227843397a3bcba8183cf22cb708a2bcdf8781bcaacea9bb`  
		Last Modified: Thu, 03 Sep 2020 23:29:41 GMT  
		Size: 17.0 KB (16956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd0249337b6b8958919ce891b5cf779db99f276dc27eb178d882fa907c1b5ca`  
		Last Modified: Thu, 03 Sep 2020 23:29:41 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bffe18e841947a8accefab9d4e93ecad418570bc9a365f2fca1aabe1a3d591`  
		Last Modified: Fri, 04 Sep 2020 01:43:56 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e74b78c8cc5f805951b0aa0ae223c655fe21969efa259e647cb6c7de0ef988`  
		Last Modified: Fri, 04 Sep 2020 01:43:52 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f12541049511052b6df990b36edc4090b2739fc6696c6e641123a6bfaed4b70`  
		Last Modified: Fri, 04 Sep 2020 01:43:53 GMT  
		Size: 3.9 MB (3922107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90808c23a8dc9b6ac33aa3d81436869f36997d684dcded7ec82e14568f492b4`  
		Last Modified: Fri, 04 Sep 2020 01:43:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc81b5ebb3739a46800d3d7d101f8f5845e63447d72fad512b69b4d4ef074ab`  
		Last Modified: Fri, 04 Sep 2020 01:43:53 GMT  
		Size: 570.8 KB (570773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bcd3a9780e36e8b97a53b0438b19951b3ae73b9b85dae97af2087779fccb2c`  
		Last Modified: Fri, 04 Sep 2020 01:43:52 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:220127d4bfee0337dbbeaabd916859a4cbceb8bd236ed6bea4ca6049257e20c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33752684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a619aa56afcf86eb3699cb2562b2f2a7cf1fd0ed487066c7e57ca941d56dbaa`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:45:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 19:54:11 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 19:54:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 19:54:12 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 19:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:54:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:58:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 19:58:49 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:59:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 19:59:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 19:59:35 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 19:59:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 19:59:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 20:00:05 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 20:00:15 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 22:16:08 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 22:16:36 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 22:17:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 22:17:52 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 22:18:05 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 22:18:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 22:18:19 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 22:18:55 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 22:19:06 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:19:15 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 22:19:23 GMT
USER adminer
# Thu, 03 Sep 2020 22:19:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036cdcf4ba76a56a0963a72479b2ab999aeb12c690481ea79abd06356c4f823`  
		Last Modified: Thu, 03 Sep 2020 21:48:57 GMT  
		Size: 10.3 MB (10317381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f59e05ab5929068d18d86a524b6f219e677287ee019a4f67c69caf9abe519`  
		Last Modified: Thu, 03 Sep 2020 21:48:53 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c19109dc7498984dcd92ea03055e7c556d76be607f7f99e8a2ba137a83ce0b6`  
		Last Modified: Thu, 03 Sep 2020 21:48:57 GMT  
		Size: 14.4 MB (14449883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d625dc6f77d5324a1f4eb486fda13286757fb45f12b0d564537c80d5233c69b1`  
		Last Modified: Thu, 03 Sep 2020 21:48:53 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2324f230fcc521afe2ddd7552d3fbd08536dca676c9950d81f50e332909bfb`  
		Last Modified: Thu, 03 Sep 2020 21:48:54 GMT  
		Size: 17.0 KB (17027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7be432a86d7e458348db45930704813a0fc764ddbcafbc66c5d7821bbd57b7`  
		Last Modified: Thu, 03 Sep 2020 21:48:53 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173e5a6fc223cc6d719e4a5c944e6ca6a2c6da3a40e09d7a4565dae1fe265723`  
		Last Modified: Thu, 03 Sep 2020 22:20:23 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786d5109852bf5db2db63db03eb1d4e4a4b18551c839b496b56af3495388641e`  
		Last Modified: Thu, 03 Sep 2020 22:20:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e32bef39b150be4f91dc7bee23f9318551d41a8a36aefb32185caafa6b9418`  
		Last Modified: Thu, 03 Sep 2020 22:20:21 GMT  
		Size: 4.3 MB (4330247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b824671f85201910e497aa7b898a38613a7253231bfc6626fde5b4049bc82a7`  
		Last Modified: Thu, 03 Sep 2020 22:20:20 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463c01d8970fa0b7c2ea02916ba83b2e426d68009097dcb273a9f5608b325236`  
		Last Modified: Thu, 03 Sep 2020 22:20:21 GMT  
		Size: 570.8 KB (570770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d0b97826535fe48a85210ed99328d4df182ff90ec2860b2d869def8b77884`  
		Last Modified: Thu, 03 Sep 2020 22:20:20 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:c4aff3e785c4840ece3287074508b9175c06be8f4f405816e299e6b75c0d1298
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34695771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf9eb18261104232d6b322ec58bfde72e6c1bae0be6d41f97772a73e66873c1`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 19:03:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 19:03:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:03:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:03:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 19:03:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 20:31:04 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 20:31:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 20:31:04 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 20:31:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:31:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:41:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:41:19 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:41:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:41:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:41:21 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 20:41:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 20:41:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 20:41:22 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 20:41:22 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 23:52:28 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 23:52:28 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 23:52:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 23:52:58 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 23:52:59 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 23:52:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 23:52:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 23:53:00 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 23:53:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 23:53:01 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 23:53:01 GMT
USER adminer
# Thu, 03 Sep 2020 23:53:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d22dfefd558d06232f42d796c11be20f4811742b692a05c071f7cc758eb63ca`  
		Last Modified: Thu, 03 Sep 2020 23:23:18 GMT  
		Size: 10.3 MB (10317343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a39f0fee451eec1887179a6d2fdd847b49bb7b138fdb68d014ecfac3e98ece`  
		Last Modified: Thu, 03 Sep 2020 23:23:14 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9a6913b79fbf27091274391ed22992cfeb2b40ca04b8ad1335302488e044f9`  
		Last Modified: Thu, 03 Sep 2020 23:23:24 GMT  
		Size: 15.0 MB (15025449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19851b9c2a57f8229c8c06440e24379ab446222c79c945424f5dc58e05bbd533`  
		Last Modified: Thu, 03 Sep 2020 23:23:14 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5e26f205b9eadde946ee3485ceb50c9c351e07c194018548892b3dec22c9f2`  
		Last Modified: Thu, 03 Sep 2020 23:23:14 GMT  
		Size: 17.0 KB (16980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010aa6fa6e94296e508343a672f00fe1fd64df21f5895df5a322918a1aaeb71c`  
		Last Modified: Thu, 03 Sep 2020 23:23:14 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d342ebcd6d3daa4f7d354c97ce15ae39456a76fb28e94f40b5ff940f2eeb1635`  
		Last Modified: Thu, 03 Sep 2020 23:53:32 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76929b808101b5816379d6f91c141ed5f74ab113a67ffb26e35b595c678901f8`  
		Last Modified: Thu, 03 Sep 2020 23:53:31 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d02ee228d52f920dd6982b212fc2d8028c51d81df4b1dedf9d6c0479d731c0`  
		Last Modified: Thu, 03 Sep 2020 23:53:33 GMT  
		Size: 4.5 MB (4516887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e915db02ae59063321477151da97a1c761ad3e593fd8451397cb540c21796c6`  
		Last Modified: Thu, 03 Sep 2020 23:53:31 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f142847478fe3f3797551646805ab7891aaec6436bc6c264aba8a689ba877b19`  
		Last Modified: Thu, 03 Sep 2020 23:53:32 GMT  
		Size: 570.7 KB (570681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab75f7eb316181ff7ed55d1e2fdf4301cfe952697d7cfebbfb56ce387e5d96b`  
		Last Modified: Thu, 03 Sep 2020 23:53:31 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:9cd203c21db2d881123b8f385e73fd5406f6230f6218dc716c60f72325165cd6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35089898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a6dc6bed4e39a63c2a6d48b399f4ceadaa5988390574d077f36a7ffb1ad929`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:50:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:50:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:50:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:50:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:50:52 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 20:17:12 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 20:17:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 20:17:22 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 20:17:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:17:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:21:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:21:45 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:22:03 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:22:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:22:20 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 20:22:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 20:22:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 20:22:52 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 20:22:56 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 23:38:59 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 23:39:18 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 23:40:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 23:40:16 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 23:40:20 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 23:40:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 23:40:31 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 23:40:43 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 23:40:45 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 23:40:49 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 23:40:54 GMT
USER adminer
# Thu, 03 Sep 2020 23:40:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13a9d0918eb5eb80bc3791371f161c63a25145d15a34a6069bae85d4b74d11`  
		Last Modified: Thu, 03 Sep 2020 22:20:49 GMT  
		Size: 10.3 MB (10317379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b975ffbfdba14d65c2d6a09cec921b03477cb753812374b30affeabf2c00ec`  
		Last Modified: Thu, 03 Sep 2020 22:20:43 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f14ba07d33e383d3ee1aced6bc3e261aa8af1e66d31b15253feb17606c89e2`  
		Last Modified: Thu, 03 Sep 2020 22:21:02 GMT  
		Size: 15.6 MB (15622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8117d8e0719b05c2c094713aa368b8b51d21a769ea2ad049594efa8e69a128b`  
		Last Modified: Thu, 03 Sep 2020 22:20:42 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194e34b2ab764ea33a72e76929b4e3699adeb705c0dd279ed82c557600698fd0`  
		Last Modified: Thu, 03 Sep 2020 22:20:43 GMT  
		Size: 17.0 KB (17025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56b5d8127deeed309a76d54ee592aee909ba7fe7653488f3994403604d761c`  
		Last Modified: Thu, 03 Sep 2020 22:20:43 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d984463319c648d0d4b9f6320ea32161523a625c46241ea676ba9b1ce96285`  
		Last Modified: Thu, 03 Sep 2020 23:42:05 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57646820f85ec30201eb1341a313a482f3fcdf64c5696605d4a4b4905cbd69`  
		Last Modified: Thu, 03 Sep 2020 23:42:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f9252bb284471a94bc2bf12d1f9a206d911e9e819f05ee16187c70f659a18c`  
		Last Modified: Thu, 03 Sep 2020 23:42:03 GMT  
		Size: 4.4 MB (4357687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc9e1dbdc344c8555453beaa78435c027f938e2c9cdacd0fb2cee22ddc91369`  
		Last Modified: Thu, 03 Sep 2020 23:42:01 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15255211853decd7340ea051637f41fa8ad6d3a4797864e635ebefc5d0b0236`  
		Last Modified: Thu, 03 Sep 2020 23:42:03 GMT  
		Size: 570.8 KB (570768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079a362143de1ae0527ce2373274793aa0d1fdf46c4e2cc11ae8a13a2d33028d`  
		Last Modified: Thu, 03 Sep 2020 23:42:01 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:f6702a555abc5ac657e38c09d934e1c4ea1df8e85419e95d5abf3c9056f9db19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.2 MB (33188917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08fd443b02a60ca2b86d36e45e23d7fcee7a8a42fae78a4e3c3745c661649fe`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:32:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:32:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:32:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:32:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:32:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 18:56:17 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 18:56:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 18:56:18 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 18:56:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Oct 2020 18:56:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:59:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 18:59:05 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:59:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 18:59:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 18:59:06 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 18:59:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 18:59:07 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 18:59:07 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 18:59:07 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 20:45:56 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 01 Oct 2020 20:45:56 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 01 Oct 2020 20:46:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 01 Oct 2020 20:46:13 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 01 Oct 2020 20:46:14 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 01 Oct 2020 20:46:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 01 Oct 2020 20:46:14 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 01 Oct 2020 20:46:15 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 01 Oct 2020 20:46:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 01 Oct 2020 20:46:16 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 01 Oct 2020 20:46:16 GMT
USER adminer
# Thu, 01 Oct 2020 20:46:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4342c41160d81e66233efcc35bd1437e778a047d4649105fb67c421f11d74381`  
		Last Modified: Thu, 01 Oct 2020 20:05:10 GMT  
		Size: 10.3 MB (10320992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b45519053c0933b8d3115c2c50afc1fca3d4aae77facd11f3f4e9524340f3c7`  
		Last Modified: Thu, 01 Oct 2020 20:05:05 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5301011cb3c2d663affc9e97b98f0d5e130d208b57a7da24eec41d87c8fef`  
		Last Modified: Thu, 01 Oct 2020 20:05:09 GMT  
		Size: 14.2 MB (14160775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a053171cf0c9918b5794e978d95ecb31b21293d0746aa98778de6bcbcd69d342`  
		Last Modified: Thu, 01 Oct 2020 20:05:04 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe1f0c26b02cbf9b742548fbf507cc4335a4971477186002707f04b68d39df2`  
		Last Modified: Thu, 01 Oct 2020 20:05:04 GMT  
		Size: 17.0 KB (17041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb8e81f4c05a8f429aaea95036f06c52f90267c3ed34d2b82bf7a4ccc6552bb`  
		Last Modified: Thu, 01 Oct 2020 20:05:05 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6d14ebf850d4ff330624320fe80d7390f2feb54b9f0a0fe55c64b74d3be973`  
		Last Modified: Thu, 01 Oct 2020 20:47:04 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2d1ec6d4a036d61e2f7e99fcebb2c82d9cfbd0b5df593cc6d4f6ca93894dfb`  
		Last Modified: Thu, 01 Oct 2020 20:47:00 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631e49164001e119375f9ef15e1e784deedfd30964844ca46eb73eb6d5c45143`  
		Last Modified: Thu, 01 Oct 2020 20:47:01 GMT  
		Size: 4.2 MB (4153993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109194ca5c3b6c22eb9f8052afcc05aa6c2151315b4ef0514559b139f071d45`  
		Last Modified: Thu, 01 Oct 2020 20:47:01 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d393c478238cc4f0a88307981d021130fbfa4be46a2d2c05afc24b63783729`  
		Last Modified: Thu, 01 Oct 2020 20:47:01 GMT  
		Size: 570.8 KB (570770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcccfe497cfc00b551905d0f1832aa6462b97148b345b5faf58434c703eef049`  
		Last Modified: Thu, 01 Oct 2020 20:47:00 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
