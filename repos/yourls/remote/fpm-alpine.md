## `yourls:fpm-alpine`

```console
$ docker pull yourls@sha256:e1e4913a325e2f84e602ee1849b9abd2ce0ef832cbfdcae3e8f25d48e004518d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `yourls:fpm-alpine` - linux; amd64

```console
$ docker pull yourls@sha256:254e0447bf9449ec98a9b3b651a59372c7f97488dd86aaee20cf59c7e318b1c9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34713336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d6d5a9f789f8588c229bc8c0cfed3123621a9896bde8324b23226119620438`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:38:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 20:38:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 20:38:10 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 20:38:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 20:38:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 20:43:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 01:15:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:15:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:15:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 04:25:00 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Dec 2019 02:13:08 GMT
ENV PHP_VERSION=7.2.26
# Thu, 19 Dec 2019 02:13:08 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Thu, 19 Dec 2019 02:13:08 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Thu, 19 Dec 2019 02:13:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 19 Dec 2019 02:13:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Dec 2019 02:21:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Dec 2019 02:21:49 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 02:21:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Dec 2019 02:21:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Dec 2019 02:21:51 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 02:21:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Dec 2019 02:21:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 02:21:53 GMT
EXPOSE 9000
# Thu, 19 Dec 2019 02:21:53 GMT
CMD ["php-fpm"]
# Thu, 19 Dec 2019 06:21:48 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 19 Dec 2019 06:21:48 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Dec 2019 06:21:49 GMT
RUN apk add --no-cache bash
# Thu, 19 Dec 2019 06:21:50 GMT
VOLUME [/var/www/html]
# Thu, 19 Dec 2019 06:21:50 GMT
ENV YOURLS_VERSION=1.7.4
# Thu, 19 Dec 2019 06:21:50 GMT
ENV YOURLS_SHA256=ffdf0f94b66cdbeaaa62bed3fde14d4eeb2bb1669c3c342eef369ce6165a0276
# Thu, 19 Dec 2019 06:21:51 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 19 Dec 2019 06:21:52 GMT
COPY file:dae29f9c1e1fe04a79abdb2b0965f1a821bebbe26ab1e1e13cae7fe5fbaf788d in /usr/local/bin/ 
# Thu, 19 Dec 2019 06:21:52 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 19 Dec 2019 06:21:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 06:21:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9773e4044a213a29aa77e99239ac5e8f7f56877eab4f96530221d1323dae`  
		Last Modified: Mon, 21 Oct 2019 21:44:19 GMT  
		Size: 1.3 MB (1342556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ac5388d32433d5cbb16635a76d609f999bcb3ca7d1e5119e373f8da4de580`  
		Last Modified: Mon, 21 Oct 2019 21:44:19 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a226b9fe82df5bbc955b561faf3aa8df8a2faef7d2fd6cc00d95e855d4dd01`  
		Last Modified: Mon, 21 Oct 2019 21:44:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c546dddedcbc6df1bf1bfeacfaaa6cf6c3de22771a7515a2c3ac8e6a3a9962`  
		Last Modified: Thu, 19 Dec 2019 03:07:27 GMT  
		Size: 12.3 MB (12328342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46f0dc38157f40785eea18296dc5e48abe433f9a70adf83ab1acba9f1ba3027`  
		Last Modified: Thu, 19 Dec 2019 03:07:22 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13942b0504765aea8b065e6628ee3dcc132312fa2fda65ccd3878066274d073`  
		Last Modified: Thu, 19 Dec 2019 03:07:29 GMT  
		Size: 14.7 MB (14713572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2952fd49cbb4684289fa570fe17b2aece8c3e563d9824092f1d75f93630db1e`  
		Last Modified: Thu, 19 Dec 2019 03:07:22 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac55bd268390abea668eac58cf9152aeeca900da3c6f0fb404eee99c477867d`  
		Last Modified: Thu, 19 Dec 2019 03:07:22 GMT  
		Size: 72.1 KB (72081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2c1ba9ee32627a619005fb23a6eae311b381b03ce4d70921a7b8263c48b3d6`  
		Last Modified: Thu, 19 Dec 2019 03:07:22 GMT  
		Size: 7.8 KB (7787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670a90149358d8e2874a13a4ef382053769c29e4b7288a65d42991125714caf7`  
		Last Modified: Thu, 19 Dec 2019 06:22:31 GMT  
		Size: 363.8 KB (363792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1611e7ed06c6ef61105b046d22af5f67c6b30a74cb0c454c8367c1a84128b163`  
		Last Modified: Thu, 19 Dec 2019 06:22:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dec6bde10e557fc379431feb5e0037ad970cc16ed3ecdc60c0a780f03209a2`  
		Last Modified: Thu, 19 Dec 2019 06:22:29 GMT  
		Size: 612.4 KB (612369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ec872f9d995da6140e1779fef6cdfd476f5d5bd56c351293105c9d1cc3d564`  
		Last Modified: Thu, 19 Dec 2019 06:22:30 GMT  
		Size: 2.5 MB (2478266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e027be59c74a0ace13d39f0a889bf7a9b4705a84bb1222aa0ae69e3b11869163`  
		Last Modified: Thu, 19 Dec 2019 06:22:29 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88fd4c03ee7fbf26eaedb2b01e3d7d3de866ffcc58564f0cd031b9147ec2828`  
		Last Modified: Thu, 19 Dec 2019 06:22:29 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:ada376688c0483de752400a54c5a18a77c0753bc8d6ebe1b801d6af8b04f0e7c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33323517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a89469bc07b18050eb2e3b7354b43a16ad3d70ffe1c1c9edebe08ffac26fd42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 19:18:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 19:18:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 19:18:15 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 19:18:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 19:18:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 19:21:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 23 Oct 2019 23:53:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Oct 2019 23:53:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Oct 2019 23:53:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 00:26:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 18 Dec 2019 23:32:24 GMT
ENV PHP_VERSION=7.2.26
# Wed, 18 Dec 2019 23:32:25 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Wed, 18 Dec 2019 23:32:26 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Wed, 18 Dec 2019 23:32:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 18 Dec 2019 23:32:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Dec 2019 23:36:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 18 Dec 2019 23:36:07 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 18 Dec 2019 23:36:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Dec 2019 23:36:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Dec 2019 23:36:11 GMT
WORKDIR /var/www/html
# Wed, 18 Dec 2019 23:36:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Dec 2019 23:36:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Dec 2019 23:36:17 GMT
EXPOSE 9000
# Wed, 18 Dec 2019 23:36:18 GMT
CMD ["php-fpm"]
# Thu, 19 Dec 2019 01:47:25 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 19 Dec 2019 01:47:29 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Dec 2019 01:47:32 GMT
RUN apk add --no-cache bash
# Thu, 19 Dec 2019 01:47:34 GMT
VOLUME [/var/www/html]
# Thu, 19 Dec 2019 01:47:38 GMT
ENV YOURLS_VERSION=1.7.4
# Thu, 19 Dec 2019 01:47:40 GMT
ENV YOURLS_SHA256=ffdf0f94b66cdbeaaa62bed3fde14d4eeb2bb1669c3c342eef369ce6165a0276
# Thu, 19 Dec 2019 01:47:49 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 19 Dec 2019 01:47:54 GMT
COPY file:dae29f9c1e1fe04a79abdb2b0965f1a821bebbe26ab1e1e13cae7fe5fbaf788d in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:47:55 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 19 Dec 2019 01:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 01:48:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f0528fef0a6877c5926ffeb18b55e87dc4776e3fdaede41fb036329a75cc3`  
		Last Modified: Mon, 21 Oct 2019 20:02:17 GMT  
		Size: 1.3 MB (1295196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dccd8ebd353e14bda266ab0f1ad9c23bd12cc3f45cbb7986c7ae9e76f3050d`  
		Last Modified: Mon, 21 Oct 2019 20:02:16 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3ae71d8a6cd1d296213c9f1cbfc6ef1568f296a38cdd85d9d038b11eebc262`  
		Last Modified: Mon, 21 Oct 2019 20:02:16 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2ac1a444b7aa96a4cc4e0075ffd5840c59d2d037da7f49e4b4fcf760416a74`  
		Last Modified: Wed, 18 Dec 2019 23:56:45 GMT  
		Size: 12.3 MB (12328372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd083b14f847dbf922ef3529abeb7636b0a7d1e46307f5296f02ce042c2bed5`  
		Last Modified: Wed, 18 Dec 2019 23:56:40 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73428d34ec97393f535a2b2893b7142c652baf29abf3f43a38ce0d4ef0e8c011`  
		Last Modified: Wed, 18 Dec 2019 23:56:47 GMT  
		Size: 13.6 MB (13633863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb0fe0e8e56fe6dea0202e5de86d9088015035dfdf67603fd854a32c285e45`  
		Last Modified: Wed, 18 Dec 2019 23:56:40 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcec0459789280cde1e8d5b506c1761fd4020b3bfff550390ceb95f7a208fef2`  
		Last Modified: Wed, 18 Dec 2019 23:56:40 GMT  
		Size: 71.7 KB (71672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e58a73641b9fc91618de1cacfc9543f1e54c150dbab2ac4f4a528d181963673`  
		Last Modified: Wed, 18 Dec 2019 23:56:40 GMT  
		Size: 7.8 KB (7784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504d0c89aa934f08d35fed81b4a7ef9f18b82934d91fc714db4e2ce23beb0de8`  
		Last Modified: Thu, 19 Dec 2019 01:48:21 GMT  
		Size: 343.6 KB (343615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744f7fc784c4bf438948819c22223419c2ce96af0debd6c401816e3899e3e04a`  
		Last Modified: Thu, 19 Dec 2019 01:48:19 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e2d6ecd9f16193112349fced2aa7c4dc5bf6a349c23fce371ce8012031725`  
		Last Modified: Thu, 19 Dec 2019 01:48:19 GMT  
		Size: 585.9 KB (585940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0735421d5874c89a879be85fbaf6521a3e11558536e3222f8dbcbcb98833bebf`  
		Last Modified: Thu, 19 Dec 2019 01:48:19 GMT  
		Size: 2.5 MB (2478262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bacba10bbe5ff5ebbc8fa56746df1011be13868dee516e3e4efe3df0986656`  
		Last Modified: Thu, 19 Dec 2019 01:48:19 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3fa7976cc1607db2c6af1a212c9fc19617115b47e19ebac621a3f45b73dc99`  
		Last Modified: Thu, 19 Dec 2019 01:48:19 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:3700d5833ec8b301cc391bdd8146598665a6689aa52ec5bee2d0d2c0dfa2a8fd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32051149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49f77987f40361616e607cc7f4870b0b0fa5fe22d5da06012a82f97081db17ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:14:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 21:14:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 21:14:53 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 21:14:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 21:14:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 21:18:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 00:46:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 00:46:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 00:46:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 02:36:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 18 Dec 2019 23:59:04 GMT
ENV PHP_VERSION=7.2.26
# Wed, 18 Dec 2019 23:59:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Wed, 18 Dec 2019 23:59:07 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Wed, 18 Dec 2019 23:59:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 18 Dec 2019 23:59:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Dec 2019 00:02:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Dec 2019 00:02:19 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 00:02:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Dec 2019 00:02:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Dec 2019 00:02:28 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 00:02:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Dec 2019 00:02:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 00:02:33 GMT
EXPOSE 9000
# Thu, 19 Dec 2019 00:02:34 GMT
CMD ["php-fpm"]
# Thu, 19 Dec 2019 05:40:50 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 19 Dec 2019 05:40:59 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Dec 2019 05:41:06 GMT
RUN apk add --no-cache bash
# Thu, 19 Dec 2019 05:41:08 GMT
VOLUME [/var/www/html]
# Thu, 19 Dec 2019 05:41:09 GMT
ENV YOURLS_VERSION=1.7.4
# Thu, 19 Dec 2019 05:41:15 GMT
ENV YOURLS_SHA256=ffdf0f94b66cdbeaaa62bed3fde14d4eeb2bb1669c3c342eef369ce6165a0276
# Thu, 19 Dec 2019 05:41:22 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 19 Dec 2019 05:41:23 GMT
COPY file:dae29f9c1e1fe04a79abdb2b0965f1a821bebbe26ab1e1e13cae7fe5fbaf788d in /usr/local/bin/ 
# Thu, 19 Dec 2019 05:41:24 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 19 Dec 2019 05:41:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 05:41:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da38e013862bbbf80dcededb060890e1056b0a21fb5308d8d1aae6f4add3bc7`  
		Last Modified: Mon, 21 Oct 2019 22:14:03 GMT  
		Size: 1.2 MB (1205015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d960e879727868f38a6a22fb9058a4ee346b2c22f8d1eda7663c2cfbdb499b5e`  
		Last Modified: Mon, 21 Oct 2019 22:14:00 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14285e1740413252e3ef469fc4e2fcd966f5efef93572ad2292b4073e5d8b592`  
		Last Modified: Mon, 21 Oct 2019 22:14:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc2497190195da69d99b5a40d92f4afc594b4d0a99388bd1a9769539975a4ca`  
		Last Modified: Thu, 19 Dec 2019 00:32:25 GMT  
		Size: 12.3 MB (12328371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99097a4929226c8d124676b2d03a3ec82de46f721a5e45995e27e90875554e3`  
		Last Modified: Thu, 19 Dec 2019 00:32:18 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c01e24c11a2a24d1197e7dc8d78628eca5288cbf4e7e4e62ef8293a81622a6`  
		Last Modified: Thu, 19 Dec 2019 00:32:22 GMT  
		Size: 12.7 MB (12714380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c47f9dede229d210af9ccd972b4b48467ecd9a0a4a2e26b1623c5f356b20f77`  
		Last Modified: Thu, 19 Dec 2019 00:32:18 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac05720e4ec80a5e4d9b8ca48d36652e952bbd0180998c98ea6f2d283e9c19`  
		Last Modified: Thu, 19 Dec 2019 00:32:17 GMT  
		Size: 71.7 KB (71662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48b455056dece74701eb7d536219c02d5f99f61e7bd503f50639c875c9f53e0`  
		Last Modified: Thu, 19 Dec 2019 00:32:18 GMT  
		Size: 7.8 KB (7787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59487904132a65a890a88a2e9e406960601b07719a64e1bf6119024745ebae2`  
		Last Modified: Thu, 19 Dec 2019 05:42:34 GMT  
		Size: 320.2 KB (320214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef044822409acb8d8ba3886a724006e2f848e2a24c4637334b574505e13a7fa`  
		Last Modified: Thu, 19 Dec 2019 05:42:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3ff0d464b0a5b81be08b073a5baf5b6f0246119ffb47c3d55577fea12b4a40`  
		Last Modified: Thu, 19 Dec 2019 05:42:32 GMT  
		Size: 539.5 KB (539509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c4fb0846148ba8734ce0ba224c80551a060887e8b4beda00fda328c31bf3ae`  
		Last Modified: Thu, 19 Dec 2019 05:42:34 GMT  
		Size: 2.5 MB (2478262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0a97927d84f0082358e1f1a89569d5496c50c2046fc80d67203aa44c943952`  
		Last Modified: Thu, 19 Dec 2019 05:42:32 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7289b8b803fbba17d9899739b9acd63c837642460de78bb823187da034106d`  
		Last Modified: Thu, 19 Dec 2019 05:42:32 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:52572c23b6cf1277a9f878663a898cbba61a35d26e812e8e11e4341be07f89c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34394744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45578994fdc2bfdb351d72a65e6420500a7c01061b3a838b67e841fbd0223653`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:30:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 21:30:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 21:30:42 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 21:30:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 21:30:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 21:36:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 01:26:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:26:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:26:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 03:18:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Dec 2019 01:11:00 GMT
ENV PHP_VERSION=7.2.26
# Thu, 19 Dec 2019 01:11:01 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Thu, 19 Dec 2019 01:11:03 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Thu, 19 Dec 2019 01:11:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 19 Dec 2019 01:11:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:14:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Dec 2019 01:14:54 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:15:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Dec 2019 01:15:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Dec 2019 01:15:17 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 01:15:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Dec 2019 01:15:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 01:15:27 GMT
EXPOSE 9000
# Thu, 19 Dec 2019 01:15:30 GMT
CMD ["php-fpm"]
# Thu, 19 Dec 2019 07:34:23 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 19 Dec 2019 07:34:25 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Dec 2019 07:34:28 GMT
RUN apk add --no-cache bash
# Thu, 19 Dec 2019 07:34:29 GMT
VOLUME [/var/www/html]
# Thu, 19 Dec 2019 07:34:31 GMT
ENV YOURLS_VERSION=1.7.4
# Thu, 19 Dec 2019 07:34:32 GMT
ENV YOURLS_SHA256=ffdf0f94b66cdbeaaa62bed3fde14d4eeb2bb1669c3c342eef369ce6165a0276
# Thu, 19 Dec 2019 07:34:35 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 19 Dec 2019 07:34:36 GMT
COPY file:dae29f9c1e1fe04a79abdb2b0965f1a821bebbe26ab1e1e13cae7fe5fbaf788d in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:34:37 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 19 Dec 2019 07:34:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:34:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7559d755b5d17673ff70e73b3efc81dd3bd4ce4489eeb38533321f94cc3ebe`  
		Last Modified: Mon, 21 Oct 2019 22:31:02 GMT  
		Size: 1.4 MB (1352864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bf069919453424b5026db89f0b067a9234f9b089011a96855b488d18020924`  
		Last Modified: Mon, 21 Oct 2019 22:31:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d4149d516a6d5226b018c137de79dcd34670a6f862c40f5368bc157de9446a`  
		Last Modified: Mon, 21 Oct 2019 22:31:02 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cb49c9731186a8b40a8ec3c6e4c40a58b203caa365afd020945883f84621cc`  
		Last Modified: Thu, 19 Dec 2019 01:45:21 GMT  
		Size: 12.3 MB (12328382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfcbc6094014012fb61ccbec31dad2ed44bb4e2ffbda129ab138b5bed49668e`  
		Last Modified: Thu, 19 Dec 2019 01:45:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6f88ed5bcaa9a88a474a95181db2e8a641ee2ca332787abbc880c4da9c77f7`  
		Last Modified: Thu, 19 Dec 2019 01:45:22 GMT  
		Size: 14.5 MB (14451717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56823bc11170f56c606f123cbf5e4d04402ff03380aeee1deac4ad47aee9aca0`  
		Last Modified: Thu, 19 Dec 2019 01:45:17 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38439355a7a812d82b462b9f3ce317ecf4a88f9afe43d0af5db04cf7a78748c3`  
		Last Modified: Thu, 19 Dec 2019 01:45:18 GMT  
		Size: 71.2 KB (71165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7defa36d1b78fb2ada9051eab0e01af80973ea4ae142927cbc1932c655c966`  
		Last Modified: Thu, 19 Dec 2019 01:45:17 GMT  
		Size: 7.8 KB (7787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fad731c7a4f3b1196478ebd95d1100a3b5a9db447f4cc717cb7b14af70935`  
		Last Modified: Thu, 19 Dec 2019 07:35:40 GMT  
		Size: 355.6 KB (355642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce3ac6a762d64dc2bb5aa3f64df2e19e83993ee930e167d1becb3a82c8c465c`  
		Last Modified: Thu, 19 Dec 2019 07:35:39 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa02729b53612a7dc989f91cd37dc218383f3fa4e86b84d87cb7f5bbc4c46`  
		Last Modified: Thu, 19 Dec 2019 07:35:39 GMT  
		Size: 623.6 KB (623635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35767366ee82a9d44bc15baa66086b6be5b484be061f77f6cd28cbbb3ae56609`  
		Last Modified: Thu, 19 Dec 2019 07:35:39 GMT  
		Size: 2.5 MB (2478262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57e965a5a89fb606b5b2068b519003eeda3e3a05ec830c82203488b98b919b`  
		Last Modified: Thu, 19 Dec 2019 07:35:39 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14bbc6ca39f435b8aed7a692056107e0c30dbeb308e240eb80944b0a8e8c42a`  
		Last Modified: Thu, 19 Dec 2019 07:35:39 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:3785511849519632f440ed37b5898a8d8b9112b099afde842dc43d261157c48b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35208518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e1033fea63c7195e00b949d75d52eb0895416e8a396b29fbac0e387a22a1369`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:36:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 18:36:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 18:36:24 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 18:36:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 18:36:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 18:44:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 03:55:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 03:55:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 03:55:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 10:58:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Dec 2019 03:11:44 GMT
ENV PHP_VERSION=7.2.26
# Thu, 19 Dec 2019 03:11:44 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Thu, 19 Dec 2019 03:11:44 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Thu, 19 Dec 2019 03:11:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 19 Dec 2019 03:11:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Dec 2019 03:19:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Dec 2019 03:19:26 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 03:19:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Dec 2019 03:19:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Dec 2019 03:19:28 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 03:19:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Dec 2019 03:19:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 03:19:29 GMT
EXPOSE 9000
# Thu, 19 Dec 2019 03:19:29 GMT
CMD ["php-fpm"]
# Thu, 19 Dec 2019 06:54:03 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 19 Dec 2019 06:54:04 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Dec 2019 06:54:05 GMT
RUN apk add --no-cache bash
# Thu, 19 Dec 2019 06:54:05 GMT
VOLUME [/var/www/html]
# Thu, 19 Dec 2019 06:54:05 GMT
ENV YOURLS_VERSION=1.7.4
# Thu, 19 Dec 2019 06:54:06 GMT
ENV YOURLS_SHA256=ffdf0f94b66cdbeaaa62bed3fde14d4eeb2bb1669c3c342eef369ce6165a0276
# Thu, 19 Dec 2019 06:54:07 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 19 Dec 2019 06:54:07 GMT
COPY file:dae29f9c1e1fe04a79abdb2b0965f1a821bebbe26ab1e1e13cae7fe5fbaf788d in /usr/local/bin/ 
# Thu, 19 Dec 2019 06:54:07 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 19 Dec 2019 06:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 06:54:08 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb445f03290fbac06f1d4fd8350bdccf0f042078682f16ca78d11decb2072f93`  
		Last Modified: Mon, 21 Oct 2019 20:16:10 GMT  
		Size: 1.4 MB (1433654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec15cffb9cdd39c9ce1901ab9a8d40f68a406e79255a5995f04c6eb2ce4496`  
		Last Modified: Mon, 21 Oct 2019 20:16:09 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d85eba4a24ab26d8a873c36f3caeb67c15ce9d477047194007a6c37a12d7ef`  
		Last Modified: Mon, 21 Oct 2019 20:16:09 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152e1b218b460e4020cf645cacb18297e57a7fc5b60de3834eec678612291d7`  
		Last Modified: Thu, 19 Dec 2019 04:01:00 GMT  
		Size: 12.3 MB (12328360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7dd81d6e360773aa8c0611bfe224908de5a8a6997962823e009fc36999b7be3`  
		Last Modified: Thu, 19 Dec 2019 04:00:55 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a63c019b6f48a5ae404f764f2f59775a5967951b32565a7471f0e959d24bf2`  
		Last Modified: Thu, 19 Dec 2019 04:01:06 GMT  
		Size: 15.1 MB (15072024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f008bcb6248b8f832f9ed113f274f465b709c98b3a8ff162f1f1d6ff311d083`  
		Last Modified: Thu, 19 Dec 2019 04:00:56 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b499c88d1bd361c6c4ae28ad374bdfc96bb26bb5482836d89ef1104fba5a364`  
		Last Modified: Thu, 19 Dec 2019 04:00:55 GMT  
		Size: 71.2 KB (71227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c6f4a26816b52da1f5890030a96e65027a828c8d3f5409488fdd3d3850b2e2`  
		Last Modified: Thu, 19 Dec 2019 04:00:56 GMT  
		Size: 7.8 KB (7786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27fa5a1fcf424de3d31ebe657aed3a196e96ef2db4c67ed6132b3753ff45c71`  
		Last Modified: Thu, 19 Dec 2019 06:54:49 GMT  
		Size: 372.5 KB (372542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69463b1787ae37e8c7c9b8cfd34f4c46300476a9e95a2264a26e7b36d2fbd6`  
		Last Modified: Thu, 19 Dec 2019 06:54:48 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a4d7c4febd172ffb67b98360e908bf395a3578f10156845184bbb7d34d59ce`  
		Last Modified: Thu, 19 Dec 2019 06:54:48 GMT  
		Size: 651.3 KB (651284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1832d69039f76edb817a73238cd0da305f22087809f2960c22cc0f339e1202b1`  
		Last Modified: Thu, 19 Dec 2019 06:54:49 GMT  
		Size: 2.5 MB (2478267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83df74f44b8cbe6481e64a0aac62a0b2cb3a819f337f95fcbc730be21bd36a6`  
		Last Modified: Thu, 19 Dec 2019 06:54:48 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e91d70ab548dc5d9054fbd2aaf0a5ec0516b0698df1ec4f7a1fe1bbb40e66`  
		Last Modified: Thu, 19 Dec 2019 06:54:48 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:9f8394458c1a960da7876d670565b91ee8be8f75d08f442489da20f3b33f99a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (35970654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c733a2cb46579ec4dc24278f5a7f76a4d3bfb29d2ed4d0e1dd69b6894b4ee3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 19:21:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 19:21:36 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 19:21:44 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 19:21:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 19:21:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 19:26:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 01:21:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:21:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:22:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 03:29:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Dec 2019 01:08:19 GMT
ENV PHP_VERSION=7.2.26
# Thu, 19 Dec 2019 01:08:23 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Thu, 19 Dec 2019 01:08:26 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Thu, 19 Dec 2019 01:08:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 19 Dec 2019 01:08:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:13:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Dec 2019 01:13:16 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:13:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Dec 2019 01:13:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Dec 2019 01:13:28 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 01:13:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Dec 2019 01:13:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Dec 2019 01:13:41 GMT
EXPOSE 9000
# Thu, 19 Dec 2019 01:13:44 GMT
CMD ["php-fpm"]
# Thu, 19 Dec 2019 06:37:24 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 19 Dec 2019 06:37:33 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 19 Dec 2019 06:37:41 GMT
RUN apk add --no-cache bash
# Thu, 19 Dec 2019 06:37:44 GMT
VOLUME [/var/www/html]
# Thu, 19 Dec 2019 06:37:47 GMT
ENV YOURLS_VERSION=1.7.4
# Thu, 19 Dec 2019 06:37:51 GMT
ENV YOURLS_SHA256=ffdf0f94b66cdbeaaa62bed3fde14d4eeb2bb1669c3c342eef369ce6165a0276
# Thu, 19 Dec 2019 06:37:59 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 19 Dec 2019 06:38:02 GMT
COPY file:dae29f9c1e1fe04a79abdb2b0965f1a821bebbe26ab1e1e13cae7fe5fbaf788d in /usr/local/bin/ 
# Thu, 19 Dec 2019 06:38:04 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 19 Dec 2019 06:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 06:38:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d017d7c8fce6fee939d22f8de103798d1fac32dfbedd09930f5811e4f7cda31d`  
		Last Modified: Mon, 21 Oct 2019 20:21:02 GMT  
		Size: 1.4 MB (1386418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b567e7413433d6d9c79cf4a2dc4d7a1598e8ade914bccc7208d605aac6f74c3f`  
		Last Modified: Mon, 21 Oct 2019 20:21:00 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05644b5a1ce87db12e6dd89e77db169a1b80755f9809cb3b374254737f8d7d51`  
		Last Modified: Mon, 21 Oct 2019 20:21:00 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b952caa489dfb98f11ab190039de37f90d9da6c26000474f5c73a53d6f0c82`  
		Last Modified: Thu, 19 Dec 2019 01:55:15 GMT  
		Size: 12.3 MB (12328384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15788c0620317e702ce0cab49b54714cfd618bc003271fabe68ec65b5c08e9b0`  
		Last Modified: Thu, 19 Dec 2019 01:55:10 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef519265f11db163d23cb0cd5deff00cc56c731262a3e2738577456f292a266`  
		Last Modified: Thu, 19 Dec 2019 01:55:21 GMT  
		Size: 15.8 MB (15806251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21fc99559058375e7a0ae6c5324c19b4f4d6fd93e8e1bfb202b04c89fe8323b`  
		Last Modified: Thu, 19 Dec 2019 01:55:10 GMT  
		Size: 2.2 KB (2213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f57f9dd425f3556df5717eb2a52a27b6a40b36eec192307b89c754d26dc152`  
		Last Modified: Thu, 19 Dec 2019 01:55:10 GMT  
		Size: 71.9 KB (71933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709c92d8a4ed3caa40116a2b7657b2388b6eec2f7b88f0817f3f261823dc0370`  
		Last Modified: Thu, 19 Dec 2019 01:55:10 GMT  
		Size: 7.8 KB (7784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5cbe6477a919129d1455c4f135f626ec649687d3f3f279db2b0597a0569a99`  
		Last Modified: Thu, 19 Dec 2019 06:40:06 GMT  
		Size: 395.9 KB (395897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64920176ad386a8ae3df976a1224a7ff9b7e3724eceaad70f0aa1acf5ebe9c04`  
		Last Modified: Thu, 19 Dec 2019 06:40:03 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfef8f1699c185250b77003a142f07bc34469a9656ecd6121cbbfa998940ad5`  
		Last Modified: Thu, 19 Dec 2019 06:40:03 GMT  
		Size: 679.7 KB (679705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307030116639d50c3ef71301bc67a10d37c4d47c638eeb0710ee94bc09e7bc75`  
		Last Modified: Thu, 19 Dec 2019 06:40:03 GMT  
		Size: 2.5 MB (2478261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100d95773d197fff218a32515206b9e023046d3db79c30a6aa5c02d82236ece3`  
		Last Modified: Thu, 19 Dec 2019 06:40:03 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ccd49b4717b0896ab4230bf223af2dc2fbebde5338e4dd1819c019c6f7bb3`  
		Last Modified: Thu, 19 Dec 2019 06:40:03 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
