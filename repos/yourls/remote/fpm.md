## `yourls:fpm`

```console
$ docker pull yourls@sha256:2d60580e53ba53ea74128dbbf4fc678900455ece794a62cd522dea2edddf34b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `yourls:fpm` - linux; amd64

```console
$ docker pull yourls@sha256:88ee4885c1876288332f75824c74410053ada83d4e2d527ee2b0ef693d7ba70b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167738897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78275519fdd55139035724b49c268629b2f69f7231ea0f7ed282a0fff18b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 15:54:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 15:54:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 15:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 15:54:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 15:54:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 16:06:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 16:06:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 16:06:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 16:06:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 16:58:55 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 16:58:55 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 16:58:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 16:58:56 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 16:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 16:59:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 17:07:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 17:07:04 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 17:07:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 17:07:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 17:07:07 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 17:07:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 17:07:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 17:07:10 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 17:07:10 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 16:51:50 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 16:51:50 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 16:51:51 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 16:51:51 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 16:51:52 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 16:51:53 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 16:51:53 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 16:51:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 16:51:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2259392b425a174e24087b88998f9435dfee626ec8f78b8cc5cca621f7e5308b`  
		Last Modified: Fri, 03 Sep 2021 19:20:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb39fc3daf578abbdb986559d371815b4d0d565a6f27382537ba9efcfb96273`  
		Last Modified: Fri, 03 Sep 2021 19:20:48 GMT  
		Size: 91.6 MB (91605346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c501de24ca4a4f13ad18f4da04cabd46e327c4e2be77f23c696e71efff86d2d`  
		Last Modified: Fri, 03 Sep 2021 19:20:31 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eeea8e6a54cabf8956c7f32f1bc43d965408fc0cda057da52b03a931d39842`  
		Last Modified: Fri, 03 Sep 2021 19:25:35 GMT  
		Size: 11.0 MB (11021936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5172333cd41cc2509d55a0d00650f6c8b479a372373348bab081316686cf77`  
		Last Modified: Fri, 03 Sep 2021 19:25:31 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57ece6e9167c91c0f8c1c9afd0c12fff9ff9aaf4b15f6cd1cacfa652fdf6002`  
		Last Modified: Fri, 03 Sep 2021 19:25:36 GMT  
		Size: 30.5 MB (30462146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9583a802b4be25faec7ca5d65fe8d675871dfedeb3b4f5cf76cf69419787f582`  
		Last Modified: Fri, 03 Sep 2021 19:25:31 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00ead4df2b53644649cc7eae45968d7c30119eaf7c9ebe20508cb909e0ea7f4`  
		Last Modified: Fri, 03 Sep 2021 19:25:31 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e299a4e19d1c063f21b74e77078f4ee2f0681231aedc37678fe1e55df37d46`  
		Last Modified: Fri, 03 Sep 2021 19:25:31 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2934cddf26aa38b6737647beaa0906dd5a6773b4db3f0e028a4a1f47a0e672a`  
		Last Modified: Sat, 04 Sep 2021 16:52:55 GMT  
		Size: 693.0 KB (693000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871fb7b4cf31f409001312b32b186435b96987a5f2087092170e3578412a0740`  
		Last Modified: Sat, 04 Sep 2021 16:52:55 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3cce3ca56c8ccf630adc8781c92c8eeb83cbb439da6e6ff0691ca2f319a0a9`  
		Last Modified: Sat, 04 Sep 2021 16:52:59 GMT  
		Size: 2.6 MB (2572148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514d32e214b7fa06feccd20cccc35064e9865ba0315d9e1ed75eccf1e3ff650d`  
		Last Modified: Sat, 04 Sep 2021 16:52:55 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aafd2964cde9d8571c5ce6efbbda0690ea119c3f0c4eac263c6d7808f8d7cc`  
		Last Modified: Sat, 04 Sep 2021 16:52:55 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:93c8078dafe27c82a30225d47e0e9dd8487a323f3bc510daa6407cc37d42bdd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.3 MB (145325367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e7032ccb5185a8823cf646a6d6678a8e9771a32b76c2f1a5c1ad14a5d33237`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:28 GMT
ADD file:3370827f2aa0dc43cfc2dcb693f82d3f450a70850de7e2514117e366f660d302 in / 
# Fri, 03 Sep 2021 00:50:29 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:11:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 04:11:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 04:11:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:12:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 04:12:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 04:24:26 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 04:24:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 04:24:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 04:24:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 05:13:56 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 05:13:57 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 05:13:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 05:13:58 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 05:14:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 05:14:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 05:19:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 05:19:02 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 05:19:04 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 05:19:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 05:19:05 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 05:19:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 05:19:07 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 05:19:07 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 05:19:08 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 01:35:49 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 01:35:50 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 01:35:51 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 01:35:51 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 01:35:55 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 01:35:55 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 01:35:56 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 01:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 01:35:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f97b1d091d60e08b0ff779d3cf24a016e55312c03d0930408ff1e1f18d486139`  
		Last Modified: Fri, 03 Sep 2021 01:05:38 GMT  
		Size: 28.9 MB (28910713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0855b53c06c71ed242ae550f9010975ff3a38ad640fee0958ecc52b5e78302`  
		Last Modified: Fri, 03 Sep 2021 07:29:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168c68f9a53c8d179eb9ffe2d4edbb5fc9e2ed1d245215de94cc8b8aee9300d2`  
		Last Modified: Fri, 03 Sep 2021 07:30:05 GMT  
		Size: 73.7 MB (73670746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b119b13b86ab970aa45086e554b440387a7d6dc528d851152486fbc195e2eb25`  
		Last Modified: Fri, 03 Sep 2021 07:29:13 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15f95906d7abc715f27db09a89e5cf49474674fd277aae07f38ea86e38185b1`  
		Last Modified: Fri, 03 Sep 2021 07:37:33 GMT  
		Size: 11.0 MB (11020326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423713aced7980f95ab8e85247f7db0f24c7ef58499d9b238e4b55e3fe5006b2`  
		Last Modified: Fri, 03 Sep 2021 07:37:28 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eab26bb6affd461572d5094e439524d09d9f6f5480af2b811dec506176069f`  
		Last Modified: Fri, 03 Sep 2021 07:37:47 GMT  
		Size: 28.8 MB (28792893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1157ec34fb3a126c4f9096b7fe055d77fce5a06af2e6bba5adc8dc07961bd1b2`  
		Last Modified: Fri, 03 Sep 2021 07:37:28 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a342287f5a7c48c148ffe2c740c00e6cf040d4d27016e86e43dd3b572551dd20`  
		Last Modified: Fri, 03 Sep 2021 07:37:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fd2f1aa70c296260117401a0603ea9a3fae8ab40618a1a0850d7c9f74847c9`  
		Last Modified: Fri, 03 Sep 2021 07:37:28 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935eb71805cb568e0f5d17777eed4d4712248baad222b022642ebfe5dc78f173`  
		Last Modified: Sat, 04 Sep 2021 01:37:49 GMT  
		Size: 342.9 KB (342923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e44eb5f3d5a9423bf096a7d33c31801f1996c45e3dd4343e0cef1c05803a2dd`  
		Last Modified: Sat, 04 Sep 2021 01:37:49 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1854bc3214ebfee302a8411ef29c2ff8a5a62f29ff21ff526fdb8e28252bf`  
		Last Modified: Sat, 04 Sep 2021 01:37:51 GMT  
		Size: 2.6 MB (2572150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e260ba89a65259a39fe0de37ae9a43c8d8d5075671ce05375e531d5b574608`  
		Last Modified: Sat, 04 Sep 2021 01:37:49 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25f129b5f7d5aed5f51915a0499d0cba71bd48654750dd6f4914472802334e8`  
		Last Modified: Sat, 04 Sep 2021 01:37:49 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:8b42f01b7311a1afd396f17a6e12465928316073f20bd9d927e2937accaf8986
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137611092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed5f3fd080a0dd4d2410031438cc09a7b9eb043c77cc390e5270d4b9c7bfa0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 00:59:39 GMT
ADD file:94917ec8eb06f96483e43104557dd98e5160895900a9d49318eecbb3d5689d41 in / 
# Fri, 03 Sep 2021 00:59:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:19:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 13:19:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 13:19:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:19:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 13:19:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 13:31:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 13:31:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 13:31:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 13:31:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 14:15:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 14:15:11 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 14:15:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 14:15:12 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 14:15:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 14:15:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 14:19:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 14:19:57 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 14:19:58 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 14:19:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 14:19:59 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 14:20:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 14:20:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 14:20:02 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 14:20:02 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 19:44:19 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 19:44:20 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 19:44:21 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 19:44:21 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 19:44:25 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 19:44:25 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 19:44:26 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 19:44:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 19:44:27 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9bd46ffb253d51a8cc84bf034d289b4ca60344ca4446bf38633639b54c7c7ab9`  
		Last Modified: Fri, 03 Sep 2021 01:14:54 GMT  
		Size: 26.6 MB (26571627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98086d1d5d8748a43bc89bf79908db4dcd59985bc8a6ffbd735a3086b0458ce0`  
		Last Modified: Fri, 03 Sep 2021 16:29:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c9e09fff15b471e68b56ece698c546ca2645e0751d7dc552ccdb8c59bd2a82`  
		Last Modified: Fri, 03 Sep 2021 16:30:29 GMT  
		Size: 69.3 MB (69315381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750c1d85f381bb097a930260277acf05927eddcc909604fb67cb27a06bb0a230`  
		Last Modified: Fri, 03 Sep 2021 16:29:46 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eff08d43d61c469d8505e509f896f58f126b112d6ed91cb04c81e9f12221c5b`  
		Last Modified: Fri, 03 Sep 2021 16:38:12 GMT  
		Size: 11.0 MB (11020323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e134d987b940bac3099454dc36d293815a81c643976724d08d388a37225b29`  
		Last Modified: Fri, 03 Sep 2021 16:38:06 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e75fc7a7b804078f5812e826f4b514139e93f4d9901fca52238b57f35c7ca74`  
		Last Modified: Fri, 03 Sep 2021 16:38:23 GMT  
		Size: 27.8 MB (27802502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e80e615107814bcbf43505ce8347d001af2ff5215b665770ed10c3dee6b711`  
		Last Modified: Fri, 03 Sep 2021 16:38:07 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3941ef3543531ab1c3ebadeb55749fdaa487a85f5e13dd472657c5512be3e9e`  
		Last Modified: Fri, 03 Sep 2021 16:38:09 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2e8894c1b29ffd7f82e6b853123c27f19bf50bbeb312aab39eaf1724f7f608`  
		Last Modified: Fri, 03 Sep 2021 16:38:06 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bb14325ac82ff6759c6791968e33d47323540e473699c900847135c401d537`  
		Last Modified: Sat, 04 Sep 2021 19:46:44 GMT  
		Size: 313.5 KB (313489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbd8bc6d6196004f0322c27019a4d9b69aff3e8914a0d0db89b9fc3bbd776ac`  
		Last Modified: Sat, 04 Sep 2021 19:46:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c12042c32ba42fa73ff322fd09e904e230b91aad26cd4fc9f6b0a7cb6a88f9d`  
		Last Modified: Sat, 04 Sep 2021 19:46:46 GMT  
		Size: 2.6 MB (2572149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23eddec6b4d3a62e9c0d86769e76cd321aa050f6f342de0162a5326c6cb546`  
		Last Modified: Sat, 04 Sep 2021 19:46:44 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49769244ea6610acc7557cf2fdc8fb034ce2fbb9bc897d7b88437419dc218b3b`  
		Last Modified: Sat, 04 Sep 2021 19:46:44 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:dff0468bf3366fb6b35c52d2ca1bdd841c7339c2d3213e62ef730e623c9d2898
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160685213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b787059c44727836301ecb5bbf69151b36016334f0973b12f18818428308539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:33 GMT
ADD file:9600a4686ae105acffa54787a7c81f5252e90023cbcfbe37519150b954110c5c in / 
# Fri, 03 Sep 2021 00:40:34 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 08:06:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 08:06:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:06:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 08:06:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 08:17:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 08:17:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 08:17:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 08:17:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 08:58:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 08:58:59 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 08:58:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 08:58:59 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 08:59:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 08:59:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 09:02:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 09:02:42 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 09:02:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 09:02:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 09:02:43 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 09:02:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 09:02:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 09:02:44 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 09:02:44 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 01:44:08 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 01:44:09 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 01:44:09 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 01:44:10 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 01:44:11 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 01:44:11 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 01:44:11 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 01:44:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 01:44:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1901ca797b5ea06f6a4facc81ad772177fdd833ed4329dc86ef126078633b949`  
		Last Modified: Fri, 03 Sep 2021 00:48:51 GMT  
		Size: 30.1 MB (30055483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208c3dde644081fc0bf55738a8e668b9c3e2d1f0d6a1cd896fccff72d053a88`  
		Last Modified: Fri, 03 Sep 2021 10:26:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d35ae33d3a3b866de3d3541f9659050060c0e732b29aa00734d40eea2f99bcb`  
		Last Modified: Fri, 03 Sep 2021 10:26:37 GMT  
		Size: 86.9 MB (86920765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656c97547b711b8b733612392f1852b0f8c11acbe09c621a40323801c516d7de`  
		Last Modified: Fri, 03 Sep 2021 10:26:22 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9eb85d0d72f949f52af4a28dc589bf166a06c3b01405163038535cccb5a002`  
		Last Modified: Fri, 03 Sep 2021 10:31:48 GMT  
		Size: 11.0 MB (11021122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765a0095d32e4ca2154d2e3663596e0d8934f713391a857ac6b5c68af9bb9`  
		Last Modified: Fri, 03 Sep 2021 10:31:44 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d15cece30dcb7cec325a2db93301e85d22e670f7fac51ed66d1741d90b2b9a8`  
		Last Modified: Fri, 03 Sep 2021 10:31:49 GMT  
		Size: 29.7 MB (29748605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d970a6267ed6a2a07c972c26a760e3c5eb5e783c90433b17983494e0ed475d8b`  
		Last Modified: Fri, 03 Sep 2021 10:31:45 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1ba0682677f513831aa284cd49727a557469db0ba14e5b793b1a4c82080c36`  
		Last Modified: Fri, 03 Sep 2021 10:31:44 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70dbebb1ea34fa6ef6c376a230a182fa89ec89b6948206c222fe0374444ffb0`  
		Last Modified: Fri, 03 Sep 2021 10:31:45 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976eb2d0014e77f49d30934af4ffc69e8dbf9cab028b2ef417f85c480fc7556c`  
		Last Modified: Sat, 04 Sep 2021 01:45:41 GMT  
		Size: 351.5 KB (351485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35014050b6fa0b8300cd84ba8710d5f9e75ecec5fe183fa65d31847dbfc9b7f2`  
		Last Modified: Sat, 04 Sep 2021 01:45:41 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc74da29b8fd8d155c1efe123a460be8b30788d33c8a1e452ccbbb768dd6c7b`  
		Last Modified: Sat, 04 Sep 2021 01:45:42 GMT  
		Size: 2.6 MB (2572149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd7fb7ad8fb80f094f01bee9ef192ce902e2766a23c77a63ef32e385e6c8b68`  
		Last Modified: Sat, 04 Sep 2021 01:45:41 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d276b575be8f4b3e5e2b416ec052edcc9e128e7ffde822ac8f98f97fb95a4`  
		Last Modified: Sat, 04 Sep 2021 01:45:41 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; 386

```console
$ docker pull yourls@sha256:8d3d70c4ba3cfa6ff1699a9f5863a348d4954493688239918ceb48e291ac547d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.5 MB (170520015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9981b98980098c1e9616a905416bcb9c8a72d9a8814aa91b56e82645b1cd8c1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:52 GMT
ADD file:dcef0e50863a79295fdbbdad2086d337d6935a220550cb8adaedd7929bd7de63 in / 
# Fri, 03 Sep 2021 00:39:52 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:57:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 06:57:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 06:57:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:57:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 06:57:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 07:11:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 07:11:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 07:11:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 07:11:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 08:03:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 08:03:46 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 08:03:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 08:03:47 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 08:04:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 08:04:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:09:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 08:09:28 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:09:30 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 08:09:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 08:09:30 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 08:09:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 08:09:31 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 08:09:32 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 08:09:32 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 03:17:19 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 03:17:19 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 03:17:20 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 03:17:20 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 03:17:22 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 03:17:22 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 03:17:22 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 03:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 03:17:23 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e16e03ac165c3106d1f4265c32840999585f4c4f0e56bd13286caeef08c5be9a`  
		Last Modified: Fri, 03 Sep 2021 00:48:04 GMT  
		Size: 32.4 MB (32379875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c426639a80dc4c00780cd81e4cc98fd456fdb77860d03ff18f1e99c367a69788`  
		Last Modified: Fri, 03 Sep 2021 10:41:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d32a328bbb755d97d4b4fe8ba233c8473d3ab1f708851cf3ac63fccad0302b`  
		Last Modified: Fri, 03 Sep 2021 10:41:49 GMT  
		Size: 92.7 MB (92712721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309cb1c222cc4d605994e6e6f8fda2d134bd40a4c8fccc34b889580c9eeeda26`  
		Last Modified: Fri, 03 Sep 2021 10:41:11 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debd9c8379df9c179556abcdfa1aeb8d69cb2919f9df00c8fa537c69255e7b13`  
		Last Modified: Fri, 03 Sep 2021 10:48:48 GMT  
		Size: 11.0 MB (11021085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd57cd140bd4f3751bbed1cefde0ac0996f274b9bd09fbee11e480bdb5fcccf2`  
		Last Modified: Fri, 03 Sep 2021 10:48:43 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d7f475b4c1c913cb1e9f4eeffebec7d7a4319535ba4a041aa33ea47aeb9d73`  
		Last Modified: Fri, 03 Sep 2021 10:48:55 GMT  
		Size: 31.1 MB (31132502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb935e75e122655acd4490b341d22cd6bda1e5622cf881ac4c0efca598ac201`  
		Last Modified: Fri, 03 Sep 2021 10:48:43 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52903516c16c77a95bc40d5283e692883155e2955d7e433700a9f341d11075e5`  
		Last Modified: Fri, 03 Sep 2021 10:48:43 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935fb7efbf5ba36d0a658646304a6a1bb59fdcc575b945a29956a39884f3416c`  
		Last Modified: Fri, 03 Sep 2021 10:48:43 GMT  
		Size: 8.6 KB (8563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37b471dba357808066d2a5c580015bb962cc67c635f4442d87a07f560ebff8`  
		Last Modified: Sat, 04 Sep 2021 03:19:00 GMT  
		Size: 686.1 KB (686092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8109a6762ab93882728c2ce005bdfc4bc3d3063ac0f10ca552e22c70e76f0a1`  
		Last Modified: Sat, 04 Sep 2021 03:18:59 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd7b1eba3872a6d10d9b32a70c13dfe564d33ae265459885d1d7646b235021f`  
		Last Modified: Sat, 04 Sep 2021 03:19:00 GMT  
		Size: 2.6 MB (2572147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6edae909cfdb74e9e13d5b4188430961129d1ce7688a9e3dba3c3563c029f30`  
		Last Modified: Sat, 04 Sep 2021 03:18:59 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edbec88d51fdd92589ffefbb4104ace1e87fd53c72b949fb84bc6ceed23c0a1`  
		Last Modified: Sat, 04 Sep 2021 03:18:59 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:11fcb31e1015b15a6c593f947d4aaa2eb7be38975cd232e4841bcc379738f999
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (144970116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc25dfa502ae8292664ca89b7b45eb5d44534c08f04b685dc662ceb5103965dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:01 GMT
ADD file:e842559443fb9351f1a9ac9ce03dfe0b069d8b9c3409f8d9b21abcbdc2a437c5 in / 
# Fri, 03 Sep 2021 01:10:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 03:39:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 03:39:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 03:40:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 03:40:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 03:40:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 04:07:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 04:07:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 04:07:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 04:07:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 05:54:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 05:54:51 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 05:54:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 05:54:52 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 05:55:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 05:55:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:08:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 06:08:04 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:08:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 06:08:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 06:08:07 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 06:08:08 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 06:08:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 06:08:09 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 06:08:09 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 08:19:33 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 08:19:35 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 08:19:35 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 08:19:35 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 08:19:39 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 08:19:40 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 08:19:40 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 08:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 08:19:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2320664dc3760d5d905a15eef2bf52da0cbab097fb4fc626c1f96722a2e2188c`  
		Last Modified: Fri, 03 Sep 2021 01:18:25 GMT  
		Size: 29.6 MB (29627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddeccc4720571d71483acc1182db8d8d63700ae941f845925a5b89fd4c8d0c1`  
		Last Modified: Fri, 03 Sep 2021 10:15:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de30247ef2b7e693655ed84e97a561f010f2592c6d840d45b089364cdc378018`  
		Last Modified: Fri, 03 Sep 2021 10:16:49 GMT  
		Size: 72.0 MB (72015443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033f72181f7975d86559a816eb9cc3b8c318726580c6f4e44bdefce9908fe2c`  
		Last Modified: Fri, 03 Sep 2021 10:15:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f37c003ad46cdfb65ed8b3fc3ab8d6ddce07f3d030fca6692e2786f16696620`  
		Last Modified: Fri, 03 Sep 2021 10:25:09 GMT  
		Size: 11.0 MB (11019508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b074f29f5ef3fb548b3aba41cfbae7cf31cb1b6581a5f353bac5f2376b21b44`  
		Last Modified: Fri, 03 Sep 2021 10:25:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839b9662f648a5baca6082696850e97442360f485bd6c62489100a6300523cad`  
		Last Modified: Fri, 03 Sep 2021 10:25:25 GMT  
		Size: 29.4 MB (29370635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c2aa930fb2f10facab1ed34018c935c2dec73cf28601cee8d7cee8b34069c1`  
		Last Modified: Fri, 03 Sep 2021 10:25:04 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09377b80f5e04049562e9bac5f5950aa10c2bbe9ef6084c832670fd8ac15c85`  
		Last Modified: Fri, 03 Sep 2021 10:25:04 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cada28380b890bbf599145fcb743cd334ef53c0c7f7f25d507bed4421e92dd`  
		Last Modified: Fri, 03 Sep 2021 10:25:04 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11758ae5e724b535b21115c3ece5dfca34448e0483b552668b72c7d4e4d92cdb`  
		Last Modified: Sat, 04 Sep 2021 08:20:55 GMT  
		Size: 349.4 KB (349423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b0dab95744926fd18a0c9e0968371b355d9c2ef2ee6fc3912e7f52b8cc9738`  
		Last Modified: Sat, 04 Sep 2021 08:20:56 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d984dff8f1774777bf0e989a6c778133777dfa07a9d4fda53ccee334ead14db`  
		Last Modified: Sat, 04 Sep 2021 08:20:58 GMT  
		Size: 2.6 MB (2572113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c0de637d37e167e9d794a429ef382d55a2e18c7b960e9bdf093b30df2d6aa`  
		Last Modified: Sat, 04 Sep 2021 08:20:55 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6b81480e0548aec8976780132501aea378560d910604457db32e111253971d`  
		Last Modified: Sat, 04 Sep 2021 08:20:55 GMT  
		Size: 2.0 KB (2039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:05c699bb37f3210fe9b345aab61bf6c83b59e35fd797793b537a0530bb4757fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167652766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87130e10be7c9eb2160903329e81bca88a2e1062712764b19b5db359cae94461`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:11 GMT
ADD file:71b4f3130e43c12907b826b33d9869308eec40607243a12d904fe47311431db9 in / 
# Fri, 03 Sep 2021 01:23:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:39:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 11:39:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 11:41:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:41:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 11:41:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 11:59:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 11:59:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 11:59:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 11:59:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 13:10:39 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 13:10:42 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 13:10:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 13:10:47 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 13:12:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 13:12:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 13:16:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 13:16:48 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 13:16:55 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 13:16:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 13:16:59 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 13:17:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 13:17:08 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 13:17:10 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 13:17:13 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 11:48:16 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 11:48:32 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 11:48:40 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 11:48:43 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 11:48:50 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 11:48:52 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 11:48:53 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 11:48:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 11:49:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:be889fbf38c25cf263aa8d8c960d58470da7f841ab3f4949b8a1ac5c4514956c`  
		Last Modified: Fri, 03 Sep 2021 01:36:58 GMT  
		Size: 35.3 MB (35272405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9a3a7bdcc5e09f63ea4a3f403c5fb0ff46b25c93859d06be80f380cc83f690`  
		Last Modified: Fri, 03 Sep 2021 16:22:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f7118b88826130f05a6867f42c170ffda007d7dbd24545309b1d22a2452632`  
		Last Modified: Fri, 03 Sep 2021 16:24:04 GMT  
		Size: 86.6 MB (86624386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e3e6d795b768e15a082582e865400aed1c0ba996a28958ef763ef6cda0b48`  
		Last Modified: Fri, 03 Sep 2021 16:22:28 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be31dafac03cac4528a91f53e2cd92d17121d4361b77a51ec5313a4c83d3ad6`  
		Last Modified: Fri, 03 Sep 2021 16:32:29 GMT  
		Size: 11.0 MB (11022276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a220feb2fa340e1b1d31b2d3e224bed119513216bac1808787211cff181a1a6`  
		Last Modified: Fri, 03 Sep 2021 16:32:23 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f01524be5e62a13e82743dc65e7b644b407cc5cd57fd64477794debf01023f9`  
		Last Modified: Fri, 03 Sep 2021 16:32:40 GMT  
		Size: 31.7 MB (31741673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b173704ba2bb837a0895c45083642bdfeb2594d569a41574e31e551ef371a0`  
		Last Modified: Fri, 03 Sep 2021 16:32:23 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638514eb125918fb7b755e962fab55c4ce30840a14f8d8d477bf795283bb0e4e`  
		Last Modified: Fri, 03 Sep 2021 16:32:23 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635a03af0c75715a3079f95de6499b1da63be930e36d06d3dae9281cbbd6769e`  
		Last Modified: Fri, 03 Sep 2021 16:32:23 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0b920b3aa34823fcfa0283d9a120451b5f31f20360ad7599a860011b29514d`  
		Last Modified: Sat, 04 Sep 2021 11:50:31 GMT  
		Size: 404.3 KB (404270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c05bcf3b97a7a131cd9abcc30237488811f537c69170bf84ba1a25dd619c943`  
		Last Modified: Sat, 04 Sep 2021 11:50:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b48f4e27bb37df23444b8f9223fa4048faa6545b393a3c66640d0811a4dc8c3`  
		Last Modified: Sat, 04 Sep 2021 11:50:32 GMT  
		Size: 2.6 MB (2572148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce56de1b3b1aa13d1912db7e491fa77c90fd6455acbcafc5b9464d7289733d9`  
		Last Modified: Sat, 04 Sep 2021 11:50:31 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba30eb2295becb7b3076aa5adba2481d603c1fc9ce4fd5c931494b91026a077`  
		Last Modified: Sat, 04 Sep 2021 11:50:31 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; s390x

```console
$ docker pull yourls@sha256:40e24f807af833d8a13b2668934abc3f00150db43222305efd1b7038e51516ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144462896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608ff5ef7d9749b3510f21821b2282e143817b0611cc8b65af8ae972f994d213`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:48 GMT
ADD file:9e72d98b2c920e433c6b776ed8eaf6a90cbf367d0ee37a8461d191499be72d39 in / 
# Fri, 03 Sep 2021 00:43:52 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:48:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 08:48:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 08:49:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:49:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 08:49:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 09:04:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 03 Sep 2021 09:04:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 09:04:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 09:04:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 09:59:36 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 03 Sep 2021 09:59:37 GMT
ENV PHP_VERSION=8.0.10
# Fri, 03 Sep 2021 09:59:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.10.tar.xz.asc
# Fri, 03 Sep 2021 09:59:38 GMT
ENV PHP_SHA256=66dc4d1bc86d9c1bc255b51b79d337ed1a7a035cf71230daabbf9a4ca35795eb
# Fri, 03 Sep 2021 10:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 10:00:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 10:06:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 10:06:34 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 03 Sep 2021 10:06:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 10:06:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 10:06:37 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 10:06:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 03 Sep 2021 10:06:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 10:06:40 GMT
EXPOSE 9000
# Fri, 03 Sep 2021 10:06:41 GMT
CMD ["php-fpm"]
# Sat, 04 Sep 2021 02:00:07 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 04 Sep 2021 02:00:08 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Sep 2021 02:00:09 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 04 Sep 2021 02:00:10 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 04 Sep 2021 02:00:12 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 04 Sep 2021 02:00:13 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 04 Sep 2021 02:00:13 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 04 Sep 2021 02:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:00:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:33fe066e16e87fca4bcb280b7ec53d44c561299928e592068e985314cf93215b`  
		Last Modified: Fri, 03 Sep 2021 00:52:58 GMT  
		Size: 29.7 MB (29650625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21b1207f1fa6570c494278708a52572e3410b6d2caf07d5244ed0ad1f512fb2`  
		Last Modified: Fri, 03 Sep 2021 12:42:23 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466ee241a5736fb11f7726cedd6a92f4e9f15aef11e248f0439bda0788d1a2`  
		Last Modified: Fri, 03 Sep 2021 12:42:34 GMT  
		Size: 71.6 MB (71623349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d36fd8ed70be33246601a1fcda01906ff1efb2a19145f86f9c04af5627c831`  
		Last Modified: Fri, 03 Sep 2021 12:42:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4221b92e685bacca8b6486785b05035ec88513e4a13a60c0461b98aa3bfacacb`  
		Last Modified: Fri, 03 Sep 2021 12:46:54 GMT  
		Size: 11.0 MB (11020760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbdc2017b478e286c3ca402633e20544d0d3f73d16768eaa3bcef784c762ac`  
		Last Modified: Fri, 03 Sep 2021 12:46:52 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a420c1fe9db272cd4bfe809854bd5220faec904be1f6a6b03f26f4161e4794d9`  
		Last Modified: Fri, 03 Sep 2021 12:46:56 GMT  
		Size: 29.2 MB (29225176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bc1f9f0ed5dbec3740dccee7e594bd4896a96f08921dc9358c96000f544ec6`  
		Last Modified: Fri, 03 Sep 2021 12:46:52 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6a67bad456d6b1d5ca5dfb75a4035450cf43f54a11e03fe7c30cbdaffaaae`  
		Last Modified: Fri, 03 Sep 2021 12:46:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f2696cb1c07d5ddf350641a4315b40850abc29eaa9b4bcf6cb3aa66fb02353`  
		Last Modified: Fri, 03 Sep 2021 12:46:52 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd380c645aacbd0595a2bd8c18b4e567fe1d16172cd8fa26fbd8e983039e111`  
		Last Modified: Sat, 04 Sep 2021 02:01:38 GMT  
		Size: 355.2 KB (355229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31f39367489609eb7b5556da87b3d92d9ef5fac648188861339061b7fdf4c26`  
		Last Modified: Sat, 04 Sep 2021 02:01:38 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508d4b3418c4b01bddc1c95d0abfa1da82c6a30030ca8c804e81e5cc1db542bd`  
		Last Modified: Sat, 04 Sep 2021 02:01:39 GMT  
		Size: 2.6 MB (2572149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5496d512eaabb1ea65d6c27e3f24a2d9ff2c8df995a9d7310cf30878c1454c8d`  
		Last Modified: Sat, 04 Sep 2021 02:01:39 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08650a79d7872ad96138a481208eab7a92b3dc4952173328b4147468ffe6576`  
		Last Modified: Sat, 04 Sep 2021 02:01:38 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
