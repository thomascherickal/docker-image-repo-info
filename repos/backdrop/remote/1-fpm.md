## `backdrop:1-fpm`

```console
$ docker pull backdrop@sha256:e09e407466973ddaded9b2e33c50c7660a94b64da6779b11cd4aabacf4b9c009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1-fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:74db87216ae6b831700872a6d796d1772935381c1ae32c961610423ebbf265b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170222940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae4e19849c81ca9949d5b6856a022faad44b3e9d04d92c5deaaec1d220055cee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 19:13:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 19:13:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 19:13:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 19:13:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 19:13:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 19:13:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 19:13:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 19:13:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 20:54:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Mar 2022 20:54:56 GMT
ENV PHP_VERSION=7.4.28
# Tue, 01 Mar 2022 20:54:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 01 Mar 2022 20:54:56 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 01 Mar 2022 20:55:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 20:55:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 08:14:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 08:14:00 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 08:14:01 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 08:14:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 08:14:02 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 08:14:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 08:14:03 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 08:14:03 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 08:14:03 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 11:54:17 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 11 Mar 2022 11:54:17 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 11:54:17 GMT
ENV BACKDROP_VERSION=1.21.3
# Fri, 11 Mar 2022 11:54:18 GMT
ENV BACKDROP_MD5=a93fe043630a617f6ae0977aaae3e919
# Fri, 11 Mar 2022 11:54:20 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 11 Mar 2022 11:54:21 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 11 Mar 2022 11:54:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 11:54:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418d05f34fc8335597544e0da692b7ccf95143c7c111e6d72d927272eaff9338`  
		Last Modified: Tue, 01 Mar 2022 22:04:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12340edc305c0436d312e2c4234ef0f16eff268086be6e5952ba72bb7c7d4d22`  
		Last Modified: Tue, 01 Mar 2022 22:05:12 GMT  
		Size: 91.6 MB (91604106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a3ac779969d3e1cf988bf619cab2f3c65376f2fa36b03d08b4c7ba76bfa34`  
		Last Modified: Tue, 01 Mar 2022 22:04:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18572f9f6e410eb15e71ca1cdca5a287d10f96f746ec18d0c16e952c915edbb3`  
		Last Modified: Tue, 01 Mar 2022 23:41:47 GMT  
		Size: 10.7 MB (10736374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede550c3fba02df82ee5e3cb1f4178e1930dfd2e73c52851951cb78c4c7bbd87`  
		Last Modified: Tue, 01 Mar 2022 23:41:45 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34204f4395ec2c6584b54570718b288b60410aeefa5d27b73f51a1dd1ce6602`  
		Last Modified: Fri, 11 Mar 2022 11:28:17 GMT  
		Size: 25.4 MB (25397006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8508437755458e4cea9319cfe3fc46bf21583ec1d57d1137429306bfb74223`  
		Last Modified: Fri, 11 Mar 2022 11:28:12 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c6bbbac3b7adb0f55c632effa64b251d7825a1ed55d78ed55412efe77efdd5`  
		Last Modified: Fri, 11 Mar 2022 11:28:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bdfe481508c5d0dc77a58f657fd352f661dc5487eebcf5b44f37bed75ba4fc4`  
		Last Modified: Fri, 11 Mar 2022 11:28:13 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48750a7fd2124f00cf2a1065603bdbd0f5f5902c6693eaa6b7cc767210272f7f`  
		Last Modified: Fri, 11 Mar 2022 11:55:25 GMT  
		Size: 2.4 MB (2388068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dcaf8ed8d73fec0b693021cddba14f95e180b3fb31047f4ca54c7940a96875`  
		Last Modified: Fri, 11 Mar 2022 11:55:27 GMT  
		Size: 8.7 MB (8718050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd27b332e66ea1fe9f97788ea76dbfaf8ed1dc952c28ca2411ca7906c12afe8a`  
		Last Modified: Fri, 11 Mar 2022 11:55:25 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1-fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:675e161696089649bb1c8a23cd04e6e4f24f2c4d2377b2391563005f51317e96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.3 MB (163318109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e3e874322c2bb4be5f1ca7ec1abf2a04c503d6bba81f3661c314f2e9d11ab3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 16:21:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 16:21:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 16:21:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 16:21:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 16:21:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 16:21:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 16:21:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 16:21:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 17:28:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Mar 2022 17:28:03 GMT
ENV PHP_VERSION=7.4.28
# Tue, 01 Mar 2022 17:28:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 01 Mar 2022 17:28:05 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 01 Mar 2022 17:28:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 17:28:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 04:56:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 04:56:42 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 04:56:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 04:56:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 04:56:44 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 04:56:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 04:56:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 04:56:47 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 04:56:48 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 10:33:26 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 11 Mar 2022 10:33:26 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 10:33:27 GMT
ENV BACKDROP_VERSION=1.21.3
# Fri, 11 Mar 2022 10:33:28 GMT
ENV BACKDROP_MD5=a93fe043630a617f6ae0977aaae3e919
# Fri, 11 Mar 2022 10:33:32 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 11 Mar 2022 10:33:33 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 11 Mar 2022 10:33:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 10:33:34 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33762069c180ac7a2bd850df459df42f7dac21d9a3ca6d6b138bd972ceb3b2`  
		Last Modified: Tue, 01 Mar 2022 18:17:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94fc40547e2c4be338f062fc29bcd2c7f19345badf0ff429726978f764df45e`  
		Last Modified: Tue, 01 Mar 2022 18:17:39 GMT  
		Size: 86.9 MB (86920736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63844f2b3ed82fda7e922caee6208b748ab2244bc614e0c7e140f8d6401b15e6`  
		Last Modified: Tue, 01 Mar 2022 18:17:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9550c477b741a2bcaf807025a1e25964c7c38879671cc1f429d60bf1aa699c6b`  
		Last Modified: Tue, 01 Mar 2022 18:25:52 GMT  
		Size: 10.5 MB (10519621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7f22ad991e8e4aeac5a96637143a2cbe86b4dd09392d4a3634630ab5fc048`  
		Last Modified: Tue, 01 Mar 2022 18:25:50 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9e185d4d5d195a92127bc27a794f155d2b6ae2ee02696289547381b64c385e`  
		Last Modified: Fri, 11 Mar 2022 10:00:32 GMT  
		Size: 25.0 MB (24951562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990232a810ad769915b90748403d4dcc645f1e7c5a94a468c055f940e55bd8ab`  
		Last Modified: Fri, 11 Mar 2022 10:00:28 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc82dc7520c48874b23ab612c249985503cd616e1e1a11e6fbdac4be4ae8ac3`  
		Last Modified: Fri, 11 Mar 2022 10:00:28 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb24b8a6d18d76b895026055947015354c8aeabbe1f771322988f6c0bb2276`  
		Last Modified: Fri, 11 Mar 2022 10:00:28 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd026fdfe82e13615f01e166e9fc7a60966bd00f7fbcf8c6e230199e0d2be997`  
		Last Modified: Fri, 11 Mar 2022 10:34:47 GMT  
		Size: 2.1 MB (2139014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a6135e864268daba8e46dc57fafe1915419cb7e0e865109daef987c3d679e5`  
		Last Modified: Fri, 11 Mar 2022 10:34:49 GMT  
		Size: 8.7 MB (8717280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff47de35c39ebae30de6900ebdbc45399bd81694985d5ec44c342b78e897c17`  
		Last Modified: Fri, 11 Mar 2022 10:34:47 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
