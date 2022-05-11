## `joomla:php8.0-fpm`

```console
$ docker pull joomla@sha256:10c8b27d3008252aeb725a4d5e02435784c2fd736240aa51ba4c3f495c4e66d7
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

### `joomla:php8.0-fpm` - linux; amd64

```console
$ docker pull joomla@sha256:f21154243795edb7d5630108aa50f3e695df195b9675d7fa4009821a5f97960c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.6 MB (185586482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1304a37a2224a389222ff82266389420f8bfb46f6e77934c1c62dd59b40f28dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:17:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Apr 2022 11:17:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Apr 2022 11:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:18:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Apr 2022 11:18:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 20 Apr 2022 11:18:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 11:18:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 11:18:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Apr 2022 11:45:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 20 Apr 2022 11:45:05 GMT
ENV PHP_VERSION=8.0.18
# Wed, 20 Apr 2022 11:45:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Wed, 20 Apr 2022 11:45:06 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Wed, 20 Apr 2022 11:45:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Apr 2022 11:45:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Apr 2022 11:54:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Apr 2022 11:54:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Apr 2022 11:54:14 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Apr 2022 11:54:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Apr 2022 11:54:14 GMT
WORKDIR /var/www/html
# Wed, 20 Apr 2022 11:54:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 20 Apr 2022 11:54:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Apr 2022 11:54:15 GMT
EXPOSE 9000
# Wed, 20 Apr 2022 11:54:15 GMT
CMD ["php-fpm"]
# Thu, 21 Apr 2022 10:06:23 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 21 Apr 2022 10:06:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 21 Apr 2022 10:07:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 10:07:50 GMT
VOLUME [/var/www/html]
# Thu, 21 Apr 2022 10:07:50 GMT
ENV JOOMLA_VERSION=4.1.2
# Thu, 21 Apr 2022 10:07:50 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Thu, 21 Apr 2022 10:07:55 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 21 Apr 2022 10:07:56 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Thu, 21 Apr 2022 10:07:56 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 21 Apr 2022 10:07:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Apr 2022 10:07:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012a3732d045340a3dc134901bd26323e110832b987a23c9090004d618db2f8e`  
		Last Modified: Wed, 20 Apr 2022 12:31:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43092314d50ddcd60bd7952a240eed4ac448241b205a2dd92291219d977fb4d2`  
		Last Modified: Wed, 20 Apr 2022 12:31:48 GMT  
		Size: 91.6 MB (91602110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f615e42d863613d2afbf86fbbe2546444c6f983cfd2ba757a0533b3bc72b8dc`  
		Last Modified: Wed, 20 Apr 2022 12:31:34 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee26553a705529cc8737df265798edead4f7e6c6a82bc7f0fe1f4863a65c90d7`  
		Last Modified: Wed, 20 Apr 2022 12:36:51 GMT  
		Size: 11.2 MB (11190268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8af822388fdeeb8e5d24d8229ecb949990fed79f0d64687c7b64a269b6f245`  
		Last Modified: Wed, 20 Apr 2022 12:36:50 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0f8fc275607f1db8731457c15b535391d61d7904460b99eeda563e994036ad`  
		Last Modified: Wed, 20 Apr 2022 12:37:51 GMT  
		Size: 26.0 MB (25961593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bc14f4c7f57caf880fdff22f0b8b19df5eed6fc4cee254404c3e4fcf588517`  
		Last Modified: Wed, 20 Apr 2022 12:37:47 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b15b9b345c6a480fbf2356ee24abd1a942556d2a0b720737bdf2154642e35a`  
		Last Modified: Wed, 20 Apr 2022 12:37:47 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeece90d443ee4c3149f8dd5fe2f988afc2c94cff8f2e00f506157521795836`  
		Last Modified: Wed, 20 Apr 2022 12:37:47 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48ff466d7d8bdab4f713233f4d86aa734176d9f81853779467b2762662c8719`  
		Last Modified: Thu, 21 Apr 2022 10:17:56 GMT  
		Size: 3.1 MB (3094178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bb3efe1cb5d5c782b371c004426201bf56c689d005a28230ad995a8b5ef134`  
		Last Modified: Thu, 21 Apr 2022 10:17:58 GMT  
		Size: 22.3 MB (22344661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ba409e1307c6328e25c6f2a3214bddc241ab49ba940c1f03c6a422730f873e`  
		Last Modified: Thu, 21 Apr 2022 10:17:55 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe40ef5dd56a8342c1a8712a796ea06e4c14e70ad9bd47193ac0026a95367431`  
		Last Modified: Thu, 21 Apr 2022 10:17:55 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; arm variant v5

```console
$ docker pull joomla@sha256:a6a704b092f0de3b7f6daba3b2ff2fa03e4566cc0b8ea04bea7d954f13ef48ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163587911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf0fe3ae6397c3f7827f1f85b1a37c0554aaa4c40a5465bfbd868be82333894`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Apr 2022 07:16:42 GMT
ADD file:f20c57847025604e1ea1a848af3f090f71d78b5fc2eb2ac795822da94d6e6a0a in / 
# Wed, 20 Apr 2022 07:16:43 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 23:58:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Apr 2022 23:58:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Apr 2022 23:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 23:59:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Apr 2022 23:59:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 20 Apr 2022 23:59:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 23:59:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 23:59:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 00:47:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Apr 2022 00:47:10 GMT
ENV PHP_VERSION=8.0.18
# Thu, 21 Apr 2022 00:47:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Thu, 21 Apr 2022 00:47:11 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Thu, 21 Apr 2022 00:47:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 00:47:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 01:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 01:03:14 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 21 Apr 2022 01:03:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 01:03:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 01:03:17 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 01:03:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Apr 2022 01:03:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Apr 2022 01:03:19 GMT
EXPOSE 9000
# Thu, 21 Apr 2022 01:03:19 GMT
CMD ["php-fpm"]
# Thu, 21 Apr 2022 18:05:48 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 21 Apr 2022 18:05:49 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 21 Apr 2022 18:10:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 18:10:38 GMT
VOLUME [/var/www/html]
# Thu, 21 Apr 2022 18:10:39 GMT
ENV JOOMLA_VERSION=4.1.2
# Thu, 21 Apr 2022 18:10:39 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Thu, 21 Apr 2022 18:10:57 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 21 Apr 2022 18:10:58 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Thu, 21 Apr 2022 18:10:59 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 21 Apr 2022 18:10:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Apr 2022 18:11:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3edd9d296fa023e00f76828c9d6fd6cc5b03e626341a6a045c40d2ea16c32d08`  
		Last Modified: Wed, 20 Apr 2022 07:32:27 GMT  
		Size: 28.9 MB (28921085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3b92a382ea7fe97048f7942a8b716c9d41bca684f33190a1b6f222f9790be`  
		Last Modified: Thu, 21 Apr 2022 02:18:56 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e4cac9134496ebb2f101cb1e584faea40cd37a49f5e044337e02ef8d17d2b1`  
		Last Modified: Thu, 21 Apr 2022 02:19:46 GMT  
		Size: 73.7 MB (73683459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1a04c0b586dd8771be9ba83febdff607ee72bf05240eb26e7b97f725ca8aa0`  
		Last Modified: Thu, 21 Apr 2022 02:18:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9e940614b5cfd8d1acb634f2048bc496cdf289beb7c6227fce2dbaa70cb1be`  
		Last Modified: Thu, 21 Apr 2022 02:26:40 GMT  
		Size: 11.2 MB (11188923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89ef7e9821b0aa3eafd98cf0bcac72ddce853ac541669dbc934a040aa56c806`  
		Last Modified: Thu, 21 Apr 2022 02:26:36 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f99d8483e73565314d0729d5fc0856e9939c28184e9463292094e5ac2946bc`  
		Last Modified: Thu, 21 Apr 2022 02:28:19 GMT  
		Size: 24.5 MB (24543504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3806030a53266ddafa53b163418b5e620f64925569171acc4610b2d76de745`  
		Last Modified: Thu, 21 Apr 2022 02:28:02 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f2f733559b72af041dea1619191b5649c360207285e07ec70311e68fd0db2`  
		Last Modified: Thu, 21 Apr 2022 02:28:02 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcc568074d851d64b006be61fe4647a8fdd89b2385e068a635a8a6289213ad4`  
		Last Modified: Thu, 21 Apr 2022 02:28:02 GMT  
		Size: 8.6 KB (8575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4422a40f7fcd583eb7e4149b1d499b6ac8dc48fdea8ab8442bb7f161e894c86`  
		Last Modified: Thu, 21 Apr 2022 18:39:12 GMT  
		Size: 2.9 MB (2891594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7694be340d1ac3d3b640a29ceaa9d723bae1c35a7b268ef8f2e0aca3d0eab203`  
		Last Modified: Thu, 21 Apr 2022 18:39:30 GMT  
		Size: 22.3 MB (22344642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e09ee5321c708022ddcc21190f455f49dab776f7421fd75f19f37b78757ac7`  
		Last Modified: Thu, 21 Apr 2022 18:39:10 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14cdb9f197b991a3e8da6e5624cb2ed1dc96337757e6a0fead2a9450b222137`  
		Last Modified: Thu, 21 Apr 2022 18:39:10 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; arm variant v7

```console
$ docker pull joomla@sha256:dc8efeb2f9b48f4edeebc2d302660e55b86dc769f0d67c5f6976b9c365c46345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155973042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab52a5faf3b09f6a010ee9b6f0593faed71a7203986b0fcd01d18244abe02949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 14:16:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 21 Apr 2022 14:16:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 21 Apr 2022 14:17:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 14:17:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 21 Apr 2022 14:17:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 14:17:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 14:17:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 14:17:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 15:00:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Apr 2022 15:00:49 GMT
ENV PHP_VERSION=8.0.18
# Thu, 21 Apr 2022 15:00:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Thu, 21 Apr 2022 15:00:50 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Thu, 21 Apr 2022 15:01:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 15:01:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 15:14:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 15:14:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 21 Apr 2022 15:14:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 15:14:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 15:14:57 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 15:14:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Apr 2022 15:15:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Apr 2022 15:15:00 GMT
EXPOSE 9000
# Thu, 21 Apr 2022 15:15:01 GMT
CMD ["php-fpm"]
# Fri, 22 Apr 2022 16:29:59 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 22 Apr 2022 16:29:59 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 22 Apr 2022 16:34:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 16:34:35 GMT
VOLUME [/var/www/html]
# Fri, 22 Apr 2022 16:34:36 GMT
ENV JOOMLA_VERSION=4.1.2
# Fri, 22 Apr 2022 16:34:36 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Fri, 22 Apr 2022 16:34:55 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 22 Apr 2022 16:34:56 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 22 Apr 2022 16:34:56 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 22 Apr 2022 16:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 16:34:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b6b2706f2ab155a1aa75f913f2f6a946f438652f2588747c8457de78564ff2`  
		Last Modified: Thu, 21 Apr 2022 16:34:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d413824c0d6337c3b6aaea376d2d125d16991e18b1ee338d090a759467ae3b`  
		Last Modified: Thu, 21 Apr 2022 16:34:59 GMT  
		Size: 69.3 MB (69315918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311ab91865a3753968a48b7962ae371de7f1346692b824d03c5b550e6e4ed84d`  
		Last Modified: Thu, 21 Apr 2022 16:34:16 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321b60457750e02f156152867dc8f80e4622098914c9901176e4b953b052746`  
		Last Modified: Thu, 21 Apr 2022 18:22:52 GMT  
		Size: 11.2 MB (11188950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05c43064e368de4389d3245a9e6842a00dd6d90a35f5892adcc2068c41749d6`  
		Last Modified: Thu, 21 Apr 2022 18:22:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5063b9070b8eca7874a0f589c3d5820fa1682ba7c0efd8b1b6a0580a073e4f14`  
		Last Modified: Thu, 21 Apr 2022 20:04:37 GMT  
		Size: 23.8 MB (23752882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202c0a7e50ebcb1c933cca42f8fed04ffdbb911f4c0823359af68aa1eca89377`  
		Last Modified: Thu, 21 Apr 2022 20:04:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2324dd2b782d4df263aeba6c7f4ad1c4df0f2e16baa14cdf6d6b218079785a0e`  
		Last Modified: Thu, 21 Apr 2022 20:04:22 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef33879b2a065aef4a73569fc62d34a4f4c2807bdb1aaa79ad500017253f69`  
		Last Modified: Thu, 21 Apr 2022 20:04:22 GMT  
		Size: 8.6 KB (8575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29a8784cddfca7321a21dd3eca2d9ee1d90988c6dd63b2f7fd526559490272`  
		Last Modified: Fri, 22 Apr 2022 17:03:50 GMT  
		Size: 2.8 MB (2780187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86385c402e3b06a0e281d428875dcdf3b9e2e01ae2d25450d06b409888ae0fbb`  
		Last Modified: Fri, 22 Apr 2022 17:04:08 GMT  
		Size: 22.3 MB (22344638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18d9de54b5283ae334325559765598212b673af630caf9388c9bbb2d82352d1`  
		Last Modified: Fri, 22 Apr 2022 17:03:48 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed881af4c13e575bb4f0c33681ce6b0a054d243afe1ede16ba8b932b10ab48ac`  
		Last Modified: Fri, 22 Apr 2022 17:03:48 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:91d1cf77c976960fba9c6708bb7d3fb465c1630738efe019c5c1d6ed06abf146
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178114211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1040b2bed4d5b211bc1b5a3d971d2f751f3b568aceac26b2dedac8dd71eb5c37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:54:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Apr 2022 15:54:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Apr 2022 15:54:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 15:54:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Apr 2022 15:54:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 20 Apr 2022 15:54:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 15:54:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 15:54:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Apr 2022 16:28:57 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 20 Apr 2022 16:28:57 GMT
ENV PHP_VERSION=8.0.18
# Wed, 20 Apr 2022 16:28:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Wed, 20 Apr 2022 16:28:59 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Wed, 20 Apr 2022 16:29:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Apr 2022 16:29:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Apr 2022 16:37:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Apr 2022 16:37:19 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Apr 2022 16:37:19 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Apr 2022 16:37:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Apr 2022 16:37:21 GMT
WORKDIR /var/www/html
# Wed, 20 Apr 2022 16:37:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 20 Apr 2022 16:37:23 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Apr 2022 16:37:24 GMT
EXPOSE 9000
# Wed, 20 Apr 2022 16:37:25 GMT
CMD ["php-fpm"]
# Thu, 21 Apr 2022 11:51:58 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 21 Apr 2022 11:51:58 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 21 Apr 2022 11:53:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 11:53:37 GMT
VOLUME [/var/www/html]
# Thu, 21 Apr 2022 11:53:38 GMT
ENV JOOMLA_VERSION=4.1.2
# Thu, 21 Apr 2022 11:53:39 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Thu, 21 Apr 2022 11:53:46 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 21 Apr 2022 11:53:47 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Thu, 21 Apr 2022 11:53:48 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 21 Apr 2022 11:53:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Apr 2022 11:53:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12d3b4aaab6372eb007a3b03d4e9a17823b75d804263acbc9a03b2f3d593bc6`  
		Last Modified: Wed, 20 Apr 2022 17:18:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c2be72a6916b19486404e4d330c2e0a38171287eba1738db1a7ea91e55df9e`  
		Last Modified: Wed, 20 Apr 2022 17:19:10 GMT  
		Size: 86.7 MB (86716247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bf1b5854e24b3036bea49382784344c1d97960e743ddb2710a995c9b4cd14a`  
		Last Modified: Wed, 20 Apr 2022 17:18:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92215b65fcf3dc862ed040915e0f9e05ac8c31b2c30f85ec52df525d86607f04`  
		Last Modified: Wed, 20 Apr 2022 17:24:12 GMT  
		Size: 11.0 MB (10973314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82576f6d5fb4333adc39555dd7c94e2466fbcff139c8c85f9d8dabda58fda78`  
		Last Modified: Wed, 20 Apr 2022 17:24:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd990f5d754c6329c697c370c99ef0b660008436cf24cbe3c0ef221e41e86ba7`  
		Last Modified: Wed, 20 Apr 2022 17:25:20 GMT  
		Size: 25.2 MB (25174114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a75d5a7db08f4bf4f35ec115f3c537fa96cba802203614c07d379e34631cbf`  
		Last Modified: Wed, 20 Apr 2022 17:25:16 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b92b7207230170b231cdd84c1126e77f118bad3ef20864275b4449ae25d73e8`  
		Last Modified: Wed, 20 Apr 2022 17:25:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb67fa225f452d21a266027b97ee5ddd600bd4bc611e28f2fe6bfe740d1967a`  
		Last Modified: Wed, 20 Apr 2022 17:25:16 GMT  
		Size: 8.6 KB (8576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975783dd1f7c0134f9196cb6d03048eb666a960a5eadf9cda5ca0da222721713`  
		Last Modified: Thu, 21 Apr 2022 12:06:24 GMT  
		Size: 2.8 MB (2824520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1238204aefc0ab67373e2f9fd8d4858ae2d1d46b8284a7451533ed82661129b`  
		Last Modified: Thu, 21 Apr 2022 12:06:28 GMT  
		Size: 22.3 MB (22345561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad5a17db5204b6b19846c42cd06b9a54f63a5a2423a13ed877412c01cb8438c`  
		Last Modified: Thu, 21 Apr 2022 12:06:24 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd9b7f7b57b641c6aef67cc9b1e60db6ea85537d543f1d6e9ba5d2e97a3c9c2`  
		Last Modified: Thu, 21 Apr 2022 12:06:24 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; 386

```console
$ docker pull joomla@sha256:78cb435760fe695564f782806af11d2de806a56c728c15ae411a4aef647489ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187089206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa47844385275ae2dfac4cfd3f792a3a96125cd96e7175eff6944f762c842404`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:12:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 07:12:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 07:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:12:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 07:12:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 07:12:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 07:12:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 07:12:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 08:04:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 11 May 2022 08:29:40 GMT
ENV PHP_VERSION=8.0.18
# Wed, 11 May 2022 08:29:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Wed, 11 May 2022 08:29:42 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Wed, 11 May 2022 08:29:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 08:29:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 08:38:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 08:38:43 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 08:38:43 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 08:38:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 08:38:45 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 08:38:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 08:38:47 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 08:38:48 GMT
EXPOSE 9000
# Wed, 11 May 2022 08:38:49 GMT
CMD ["php-fpm"]
# Wed, 11 May 2022 19:32:20 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 May 2022 19:32:21 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 May 2022 19:33:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:33:47 GMT
VOLUME [/var/www/html]
# Wed, 11 May 2022 21:40:27 GMT
ENV JOOMLA_VERSION=4.1.3
# Wed, 11 May 2022 21:40:27 GMT
ENV JOOMLA_SHA512=7937355529688adffe2d470bd49da89cddef1b10eca6e3ef20acfd2ebfb695fa3fa346352a68bc094787dd48fe9a2d06371038ce8894cf5ebb0197b3b6140bef
# Wed, 11 May 2022 21:40:35 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 May 2022 21:40:36 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 May 2022 21:40:37 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Wed, 11 May 2022 21:40:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 21:40:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7e0ab62bdf2006dcf0edb4bfd75f18ad278cc2688d9df909a02a0a68ef2d93`  
		Last Modified: Wed, 11 May 2022 09:24:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eaa23ffdeeb3c581979e596c004018640f1930f73b1ed2bf4edc782bfb5eb8`  
		Last Modified: Wed, 11 May 2022 09:24:15 GMT  
		Size: 92.5 MB (92510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd517709db67f5f33db055442765cc831c277e3d797ce5def1cc069a78a5d93`  
		Last Modified: Wed, 11 May 2022 09:24:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f1b16efaaf1f2763aaa5a3a6982b6b0e06fb4b9b71dd436966084abb15d8f`  
		Last Modified: Wed, 11 May 2022 09:35:56 GMT  
		Size: 11.0 MB (10973254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7373c47373d587c1db050ca12694a438bdc2d561fc58726836b83180295c218d`  
		Last Modified: Wed, 11 May 2022 09:35:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2e6349f898c06a4be8631df3ce5f6745b21bb30c984bdd7e34af7487950058`  
		Last Modified: Wed, 11 May 2022 09:36:57 GMT  
		Size: 26.2 MB (26200234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2082ff5befe1a592441351883c2c2f4e8f54100edca562db1238d56456dcd6`  
		Last Modified: Wed, 11 May 2022 09:36:53 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83cf566ce6dcd8c3573f4e2e30f9a63d6ec0f7f05a30444c12bc34e5406052a`  
		Last Modified: Wed, 11 May 2022 09:36:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77552532a6ad3314becf4ed5e073f4b34f8d3be1cc96c19870a1b84f44c7212f`  
		Last Modified: Wed, 11 May 2022 09:36:54 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564e778018947a5019f9d22b8f8b165e9da18e0851c604372d0b51f4f5d52920`  
		Last Modified: Wed, 11 May 2022 19:45:50 GMT  
		Size: 2.9 MB (2898997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f93de5821b2087eebc56e873759d50e7abfeed9c22cee0bf1572e9150a1d1bc`  
		Last Modified: Wed, 11 May 2022 21:47:14 GMT  
		Size: 22.1 MB (22101663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4128cc5507f490fab810784b51ca2ee46161a6f8d9930e1f7782fdb98fbad72f`  
		Last Modified: Wed, 11 May 2022 21:47:10 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f42e7656e0372e305d02aee005b655469e4c10f8d6f37b2b22c51f657eabc7`  
		Last Modified: Wed, 11 May 2022 21:47:10 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; mips64le

```console
$ docker pull joomla@sha256:8f155daa451bf2fe2819487137b83170831d182f1454dbf8e0ec782322bafd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162537487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c285af084bf0c8743f2df228c245794aef2c14b975a3ffb044efbafe4767a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Apr 2022 14:28:35 GMT
ADD file:11939fa9b6e0a3bde2ba32552130208df232ae0dd139b9244b80fa309690d57f in / 
# Wed, 20 Apr 2022 14:28:39 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 17:59:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 21 Apr 2022 17:59:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 21 Apr 2022 18:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 18:00:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 21 Apr 2022 18:00:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 18:00:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 18:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 18:01:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 19:58:52 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Apr 2022 19:58:56 GMT
ENV PHP_VERSION=8.0.18
# Thu, 21 Apr 2022 19:58:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Thu, 21 Apr 2022 19:59:02 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Thu, 21 Apr 2022 19:59:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 19:59:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:40:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 20:40:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:40:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 20:41:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 20:41:05 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 20:41:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Apr 2022 20:41:15 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Apr 2022 20:41:19 GMT
EXPOSE 9000
# Thu, 21 Apr 2022 20:41:22 GMT
CMD ["php-fpm"]
# Fri, 22 Apr 2022 13:38:42 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 22 Apr 2022 13:38:46 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 22 Apr 2022 13:44:49 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 13:44:53 GMT
VOLUME [/var/www/html]
# Fri, 22 Apr 2022 13:44:56 GMT
ENV JOOMLA_VERSION=4.1.2
# Fri, 22 Apr 2022 13:45:00 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Fri, 22 Apr 2022 13:45:34 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 22 Apr 2022 13:45:40 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 22 Apr 2022 13:45:45 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 22 Apr 2022 13:45:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 13:45:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:211e565c951d5d12adf5ac13e34b5fdba747f88e6b462c2863538110b219144c`  
		Last Modified: Wed, 20 Apr 2022 14:39:17 GMT  
		Size: 29.6 MB (29641236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f739687e56cfb7a039de711643daf3c882b0f0040b289151a3f02e754bccd8fc`  
		Last Modified: Thu, 21 Apr 2022 23:16:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f566aca9c129a58c56dc58d051b7ab1ec32112f2d923b0f2a3acfe23a867d`  
		Last Modified: Thu, 21 Apr 2022 23:17:50 GMT  
		Size: 71.8 MB (71809771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5aa368f0ac8f0b25a917bc3a340bff52fbcc5d7c19d68996080dd575e7061`  
		Last Modified: Thu, 21 Apr 2022 23:16:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79532bd007260d4ac3721d96f670c7412b1fe07a1b2d06c606684baee208d6`  
		Last Modified: Thu, 21 Apr 2022 23:23:52 GMT  
		Size: 11.0 MB (10972092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e61e91092a8bc4973c0071fef0380f9ae0511054356298980dac36b6734fb7c`  
		Last Modified: Thu, 21 Apr 2022 23:23:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb70583913a84d6589fd8b887d0241ee918c66405a4501d4bdefd494553c4572`  
		Last Modified: Thu, 21 Apr 2022 23:25:22 GMT  
		Size: 25.0 MB (24957526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f7d3f5f23ae2136b785c4c9098d1f4b73d71c23369dffa0ea037de715792bf`  
		Last Modified: Thu, 21 Apr 2022 23:25:06 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e58400c25f78d806bfe2420b6e874e8f216402cf530cf3f1343d365975a48`  
		Last Modified: Thu, 21 Apr 2022 23:25:06 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00725ed72da300f853de6229e88e2e8c72840cda019f3aaed8eb90ac41e7c3fd`  
		Last Modified: Thu, 21 Apr 2022 23:25:06 GMT  
		Size: 8.6 KB (8576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad91c25411cefcb1ff484ea21ddab3125ac4ed15e01a1215a2c6884ab0d9f75`  
		Last Modified: Fri, 22 Apr 2022 14:17:43 GMT  
		Size: 2.8 MB (2796631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0b8d1862fa6de3a6c8c04205b2ac67f947f5622657be43ca43417300ddf47a`  
		Last Modified: Fri, 22 Apr 2022 14:17:56 GMT  
		Size: 22.3 MB (22345565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5637df4efe8a3204f078b9eba2558a0024eb3581ea2a41c2aac525b558b774ea`  
		Last Modified: Fri, 22 Apr 2022 14:17:40 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7821ea9b99dc9b2281572e1305101331c3b63c6815071ef11e879c0432fcaf`  
		Last Modified: Fri, 22 Apr 2022 14:17:40 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; ppc64le

```console
$ docker pull joomla@sha256:127ba050494829efc9f2b4a68362277c1df108e317c1fb48e614702faa25b701
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.7 MB (185721091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d56a2e62492152ea0a50a88a2ece9ba062e5dcf75f4cc200c747acaf3ae560f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Apr 2022 09:46:36 GMT
ADD file:8d406ebce4d9b0884d46ee25ec31fe7714726024b80aba9b408d81d39e2f6f8c in / 
# Wed, 20 Apr 2022 09:46:44 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 00:57:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 21 Apr 2022 00:57:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 21 Apr 2022 00:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 00:59:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 21 Apr 2022 00:59:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 00:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 00:59:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 00:59:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 01:50:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Apr 2022 01:50:19 GMT
ENV PHP_VERSION=8.0.18
# Thu, 21 Apr 2022 01:50:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Thu, 21 Apr 2022 01:50:30 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Thu, 21 Apr 2022 01:51:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 01:51:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 02:10:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 02:10:42 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 21 Apr 2022 02:10:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 02:10:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 02:10:57 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 02:11:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Apr 2022 02:11:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Apr 2022 02:11:14 GMT
EXPOSE 9000
# Thu, 21 Apr 2022 02:11:18 GMT
CMD ["php-fpm"]
# Fri, 22 Apr 2022 00:17:26 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 22 Apr 2022 00:17:27 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 22 Apr 2022 00:20:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:20:23 GMT
VOLUME [/var/www/html]
# Fri, 22 Apr 2022 00:20:26 GMT
ENV JOOMLA_VERSION=4.1.2
# Fri, 22 Apr 2022 00:20:28 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Fri, 22 Apr 2022 00:20:45 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 22 Apr 2022 00:20:50 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 22 Apr 2022 00:20:51 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 22 Apr 2022 00:20:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 00:20:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5e0d035960b14409a1ddb839de80aa08677b71addd5e94264ff9ee89a2523e5b`  
		Last Modified: Wed, 20 Apr 2022 09:56:59 GMT  
		Size: 35.3 MB (35285249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b3f143029a650945718f049f94d7fe10ce0282766d2ebfcf8287da753d20e1`  
		Last Modified: Thu, 21 Apr 2022 03:28:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96b8b4cf170474b37586f15f5b7e9c2281d256e2284358baf9435ef970ab7f`  
		Last Modified: Thu, 21 Apr 2022 03:28:18 GMT  
		Size: 86.6 MB (86625757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e21cfe9b423c803158576f2d25107d8f04a7e4fdb55b44038e731f061a924ab`  
		Last Modified: Thu, 21 Apr 2022 03:28:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d363bc05b8f20ca4a665795ffa263b8038c96b1ff51f725aee0146d81c0214d`  
		Last Modified: Thu, 21 Apr 2022 03:34:18 GMT  
		Size: 11.2 MB (11190459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d9af5569617fc3480550789bc0b21aaa931e7a9474c3ffb1a9d33b55ec6def`  
		Last Modified: Thu, 21 Apr 2022 03:34:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f8707ed6eb910c9f319bbadd1b37091ae6af0289dc7dcfc4494c78a2b49726`  
		Last Modified: Thu, 21 Apr 2022 03:35:33 GMT  
		Size: 27.0 MB (26955362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78846f1d3b2832aa0a9eb66794e97d62939f7e9af52e90199a119b6c87b79fd5`  
		Last Modified: Thu, 21 Apr 2022 03:35:27 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2640c83b18ff7b10f64ad0ea64c654590dfd142813332d1924dd2df53c48cb15`  
		Last Modified: Thu, 21 Apr 2022 03:35:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0f93dd73f53ac88764a944e7c258f4cef4210aecd51599574bd10860a7e5d5`  
		Last Modified: Thu, 21 Apr 2022 03:35:28 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7a92d8a2179bec5a70d8f42aee59782d3ffe44fe54a56bd77c65290d7f0fc4`  
		Last Modified: Fri, 22 Apr 2022 00:42:43 GMT  
		Size: 3.3 MB (3304920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d2221d79ce6e59a0e9b40c50c4069c1c56d1fa2542aa8f98c52744c1ba23e`  
		Last Modified: Fri, 22 Apr 2022 00:42:48 GMT  
		Size: 22.3 MB (22344637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084300bb0a77b8ce1bd2b72bae7a319a5070ef23f5065d04a434729d04bfceb7`  
		Last Modified: Fri, 22 Apr 2022 00:42:43 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c40f0f56a19e6ea913c11c16a214045609d125dd9e47041cb71b2e3c112974`  
		Last Modified: Fri, 22 Apr 2022 00:42:42 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php8.0-fpm` - linux; s390x

```console
$ docker pull joomla@sha256:27adf839a7a6499553f0d3f73c0f75acf9d25f774d451b879b975bc6cf137f10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162664656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b6a26e0556c840eed3e7f01d04b4eed2082737e3592761fc075cae432053a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:00:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 09:00:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 09:00:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 09:00:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 09:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:00:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 09:44:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 11 May 2022 10:03:50 GMT
ENV PHP_VERSION=8.0.18
# Wed, 11 May 2022 10:03:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Wed, 11 May 2022 10:03:51 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Wed, 11 May 2022 10:03:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 10:04:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 10:10:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 10:10:33 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 10:10:33 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 10:10:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 10:10:33 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 10:10:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 10:10:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 10:10:34 GMT
EXPOSE 9000
# Wed, 11 May 2022 10:10:34 GMT
CMD ["php-fpm"]
# Wed, 11 May 2022 18:43:44 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 May 2022 18:43:44 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 May 2022 18:45:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 18:45:01 GMT
VOLUME [/var/www/html]
# Wed, 11 May 2022 21:45:21 GMT
ENV JOOMLA_VERSION=4.1.3
# Wed, 11 May 2022 21:45:22 GMT
ENV JOOMLA_SHA512=7937355529688adffe2d470bd49da89cddef1b10eca6e3ef20acfd2ebfb695fa3fa346352a68bc094787dd48fe9a2d06371038ce8894cf5ebb0197b3b6140bef
# Wed, 11 May 2022 21:45:41 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 May 2022 21:45:49 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 May 2022 21:45:50 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Wed, 11 May 2022 21:45:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 21:45:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f812b6b58048d2311eb80f0410cb37f884343218ec756d933b109a1a394791dc`  
		Last Modified: Wed, 11 May 2022 10:54:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d24614089fafa2f33fbfb92b70dc612b0203daeed642445bd142cf9cdee9212`  
		Last Modified: Wed, 11 May 2022 10:54:26 GMT  
		Size: 71.6 MB (71621628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb678bab4e766e631c3f955141e51e923d3288e6ff9c307728a51d28d816c4`  
		Last Modified: Wed, 11 May 2022 10:54:16 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160fcf90fac13f031aeb3fafa264de1c949389708622be50965cf8d93f77cc7c`  
		Last Modified: Wed, 11 May 2022 11:02:23 GMT  
		Size: 11.2 MB (11189273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cff5c367178574559c2fc449d8cda42bcf0da22a327003b78e02881b661e68`  
		Last Modified: Wed, 11 May 2022 11:02:23 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8efc52f2e919875115adeb90eec6cef37901e565cc0d365cb88db5fafb89e2b`  
		Last Modified: Wed, 11 May 2022 11:03:01 GMT  
		Size: 25.0 MB (25036406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6204aab01893c237916198b89e4129954a41ecf2ee50ace606c2639cd307a5`  
		Last Modified: Wed, 11 May 2022 11:02:57 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cd39d9e4ebc0d83a0a25c16c9ce93cadc3384ba3134d0003830cfbdeaaac9b`  
		Last Modified: Wed, 11 May 2022 11:02:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b78ce3038e4181b471878dc42a0180a3c63803ca618aef2920992a78b66f2c9`  
		Last Modified: Wed, 11 May 2022 11:02:57 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597bdeb31a0acd04f768f27bae03021f3a7e6dd538870c96275f5f7ff00f3dc3`  
		Last Modified: Wed, 11 May 2022 18:55:45 GMT  
		Size: 3.0 MB (3047366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fd94e50d722ff38745d82afdae8c2aaa637c29a8d33fb238fbad8fe8a5ddba`  
		Last Modified: Wed, 11 May 2022 21:54:54 GMT  
		Size: 22.1 MB (22100542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8364038c0c17d5928013b10f8111ae7ceb0e7efcaf87aa998e60d7aded620bc`  
		Last Modified: Wed, 11 May 2022 21:54:50 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2bbb376741c92f28f75ab3dd0f237ea2ab0861f538d0e1a8f8bfd745d59092`  
		Last Modified: Wed, 11 May 2022 21:54:50 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
