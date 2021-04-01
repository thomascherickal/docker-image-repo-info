## `matomo:4-fpm`

```console
$ docker pull matomo@sha256:7bd5c167433a3d21d81e79b49d9181197035fd9039ed3823b0af4b743340f876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `matomo:4-fpm` - linux; amd64

```console
$ docker pull matomo@sha256:52715a3208f1109307980ed14fb613beab49a71b67543237d3a15efe4ed5ffe1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161209131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e5749c67b51aedad6b17d5be00b726802d1b973f02f10a176bfdcc99488bf4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 09:51:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 09:51:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 09:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:51:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 09:51:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 10:04:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 10:04:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 10:04:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 10:04:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 10:24:38 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 10:24:39 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 10:24:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 10:24:39 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 10:24:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 10:24:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 10:30:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 10:30:58 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 10:30:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 10:30:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 10:30:59 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 10:31:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 10:31:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 10:31:00 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 10:31:00 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 06:50:32 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 01 Apr 2021 06:53:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 06:53:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 06:53:46 GMT
ENV MATOMO_VERSION=4.2.1
# Thu, 01 Apr 2021 06:54:08 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 06:54:09 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 01 Apr 2021 06:54:10 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 01 Apr 2021 06:54:10 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 06:54:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 06:54:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854fb08fe05067d46212fe0b4eef9b8904ba306bcd8b189884684e157639b00d`  
		Last Modified: Wed, 31 Mar 2021 11:22:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d099f6707d86ef1d69cb731a4162989a7a90160ef73c7f1fc4ec8e4fb6cf6999`  
		Last Modified: Wed, 31 Mar 2021 11:22:20 GMT  
		Size: 76.7 MB (76679701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038e5b09075278999e42de226a764ed2ffffc1467e95126feba28817c6b61596`  
		Last Modified: Wed, 31 Mar 2021 11:22:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c625a0ff934dfe39befa65f46404907efbf7aabfc520db14d68aaa63e9c1e62`  
		Last Modified: Wed, 31 Mar 2021 11:26:58 GMT  
		Size: 10.7 MB (10656366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c2dd1e32d1154ee1562e07b78ee0d11fd20bfaf5cb0e7f3a5922f84d2f233f`  
		Last Modified: Wed, 31 Mar 2021 11:26:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e85fbcce44f903742183092282ccfd0adc847d34c614fc912162a05c1653f7e`  
		Last Modified: Wed, 31 Mar 2021 11:26:58 GMT  
		Size: 28.6 MB (28572511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9675c8079d855f4115de7c1ebc348a335e096c44060b7997e8f5e9b0abddbee0`  
		Last Modified: Wed, 31 Mar 2021 11:26:52 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979fdf4722eeeda3e8df3222d9a10f8e3ccd1114f301fdbce11bb73afb520cf`  
		Last Modified: Wed, 31 Mar 2021 11:26:51 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4752052969ccd1b79e0c07262d3b2b33c5475041e0cd01552464be61f7804682`  
		Last Modified: Wed, 31 Mar 2021 11:26:52 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aa5acf5cde70e695a9078f0f098772b4ae32078a73fa0ae0d0da9a56ed9381`  
		Last Modified: Thu, 01 Apr 2021 06:55:49 GMT  
		Size: 3.1 MB (3143326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db0846c2d8e74744a81c1bb0e963e31678cd047fd90553a5a3e588552f9ef6e`  
		Last Modified: Thu, 01 Apr 2021 06:55:48 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e25460af86406bf84ff035bd46feb53ca3ca9f017c8dd90e20004e7f12bf0c`  
		Last Modified: Thu, 01 Apr 2021 06:55:53 GMT  
		Size: 15.0 MB (15005119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd23cdecdb4b58fbff436f1eacce0c66135e9e78835905ff2900ee42560b05`  
		Last Modified: Thu, 01 Apr 2021 06:55:48 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6efa25760ea2b881a85987982dd0bbcce2041862ca1f22c91ce86d8bdbc64be`  
		Last Modified: Thu, 01 Apr 2021 06:55:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; arm variant v5

```console
$ docker pull matomo@sha256:fae00247d6082776d9488e96c1e032a9bde6922508c0c494ba219370b073b7da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139507176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1dceeaf363c2dd12760c755188738a53d74350de8dea4869533973dfbf2adc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:16:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 00:16:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 00:16:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:16:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 00:16:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 00:27:07 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 00:27:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:27:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:27:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 00:43:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 00:43:20 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 00:43:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 00:43:23 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 00:43:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 00:43:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:47:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 00:47:29 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:47:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 00:47:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 00:47:35 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 00:47:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 00:47:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 00:47:41 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 00:47:42 GMT
CMD ["php-fpm"]
# Wed, 31 Mar 2021 12:22:44 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 31 Mar 2021 12:25:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 12:25:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 31 Mar 2021 12:25:06 GMT
ENV MATOMO_VERSION=4.2.1
# Wed, 31 Mar 2021 12:25:37 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 12:25:40 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 31 Mar 2021 12:25:41 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 31 Mar 2021 12:25:41 GMT
VOLUME [/var/www/html]
# Wed, 31 Mar 2021 12:25:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 12:25:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61257e71ed1fe36dd059766677f4a537b356c6fc540a3ca4ba7402f6f3d590`  
		Last Modified: Wed, 31 Mar 2021 01:29:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe994f5a2a99df2b5e9f78688bf4a0a7da6f65bbcc6a46c31e2b096ce25c012f`  
		Last Modified: Wed, 31 Mar 2021 01:29:35 GMT  
		Size: 58.8 MB (58815883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eca09f3156e497ec384a401521d8dc49d572b779a60298cad4e6929d8f38aa`  
		Last Modified: Wed, 31 Mar 2021 01:29:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14a1275893a59e7c939e187ba5251a2f645c52fc63074a2ef486002c8c736c`  
		Last Modified: Wed, 31 Mar 2021 01:32:51 GMT  
		Size: 10.7 MB (10654223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d334dd8c3e1c92dcf4198b6570cf0ddaea7eaf51f2ea32a10a7dbb2d3f5f05`  
		Last Modified: Wed, 31 Mar 2021 01:32:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21302b092336380600c583be699fc5a9dc1e2394996c4f8b686da98e45b8641d`  
		Last Modified: Wed, 31 Mar 2021 01:32:53 GMT  
		Size: 27.2 MB (27187426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e21d115b26c09e8a8782dee678ac97cef1711ae2156ec32ad3b5a158d576fa`  
		Last Modified: Wed, 31 Mar 2021 01:32:51 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e559a0ab2f5c4cec184d81595e369c8b46da69d13f16b36d11c4cff4a3e6128f`  
		Last Modified: Wed, 31 Mar 2021 01:32:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8f566e5a87f2b0a9b54c103b867f3b1af600e741414b5448505e6a17d56c7`  
		Last Modified: Wed, 31 Mar 2021 01:32:51 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c75ac5a5a6276a7f6af51cda492fbb99af263854b29c9d5ea0761ecfd53c468`  
		Last Modified: Wed, 31 Mar 2021 12:26:25 GMT  
		Size: 3.0 MB (2960133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff445fd0388523dd43902450a09b0d02077fc2e1e57891f58f742c8891caf3b`  
		Last Modified: Wed, 31 Mar 2021 12:26:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794c0169ffdf7ddc95c3ef36f4b51df6f919fc50bcc7c618c54372b6ece2e31`  
		Last Modified: Wed, 31 Mar 2021 12:26:31 GMT  
		Size: 15.0 MB (15003485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71aff4d3ef6b78e46671d3590d066b9f37ba860343d40c984a55d4326f32942`  
		Last Modified: Wed, 31 Mar 2021 12:26:24 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5147cc058c8a6b3d6e089f61d4b9c96b835913f37c4e906ceb1c38a25d5ba2`  
		Last Modified: Wed, 31 Mar 2021 12:26:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; arm variant v7

```console
$ docker pull matomo@sha256:9ef65570848533bf61a3a66fb3e55da5012a043a83f66dd7699a79e1c6fac577
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136954856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7794927bf054ef18d0f3937f4264bd7e280758b33d59be55574f5b653c52a388`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:38 GMT
ADD file:c1eeb99fc8ec483e175d4948a58d7f7b246b0d6b887f435a5fef07ef43699f76 in / 
# Tue, 30 Mar 2021 23:08:41 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 07:22:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 07:22:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 07:22:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 07:22:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 07:22:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 07:32:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 07:32:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 07:32:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 07:32:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 07:48:40 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 07:48:41 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 07:48:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 07:48:44 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 07:49:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 07:49:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 07:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 07:52:09 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 07:52:12 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 07:52:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 07:52:14 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 07:52:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 07:52:17 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 07:52:20 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 07:52:21 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 01:49:56 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 01 Apr 2021 01:53:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 01:53:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 01:53:44 GMT
ENV MATOMO_VERSION=4.2.1
# Thu, 01 Apr 2021 01:54:13 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 01:54:16 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 01 Apr 2021 01:54:17 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 01 Apr 2021 01:54:18 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 01:54:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 01:54:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ee0a2cc24f2963b99b1d30dc2613f196b7c9e38337cf99332d6c4efe07f01ef2`  
		Last Modified: Tue, 30 Mar 2021 23:16:25 GMT  
		Size: 22.7 MB (22739814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6902379d71a94188d5c60681ae18bd9f9fa097906a99e027038263140fa89950`  
		Last Modified: Wed, 31 Mar 2021 08:31:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113a588066812e435718c64d9b2879309ea88c6fe5f5b398b8231cc96bd2611`  
		Last Modified: Wed, 31 Mar 2021 08:31:55 GMT  
		Size: 59.5 MB (59512371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d469e8c06518630db4bbc7bb2aeca23cd234ab4a06f2907ca2b721a2336f86`  
		Last Modified: Wed, 31 Mar 2021 08:31:32 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7e19bf54addb343fa2ba79bfa2555662f4fdf809770d8f7573b97fd3601f54`  
		Last Modified: Wed, 31 Mar 2021 08:35:06 GMT  
		Size: 10.7 MB (10654281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda17693662fcacee7caeaa999cb1cd78350a1d5a11c800ed265d1acb41f69b6`  
		Last Modified: Wed, 31 Mar 2021 08:35:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777eea881005d5ded6dcb3e9fcbdd24b7e05e1bff209c3db2216d5ea74c21aac`  
		Last Modified: Wed, 31 Mar 2021 08:35:12 GMT  
		Size: 26.2 MB (26200688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e336485d3c190e697f2cf90ec08887782cfd576cb3a5f2ae67fca58e7b2198`  
		Last Modified: Wed, 31 Mar 2021 08:35:03 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b89842c784ec5ce9eb39f17a0f15f5dedd7e40f400f74a25ab145c6eda2afd9`  
		Last Modified: Wed, 31 Mar 2021 08:35:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec1292d352b2e322ae0b0bd64ae6901e909809d4e327253dffb0bc3979b760`  
		Last Modified: Wed, 31 Mar 2021 08:35:06 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7ae7c228b6f5a46786aa5ca76de38486b71c0b3567a245b767848b0c4e3d8e`  
		Last Modified: Thu, 01 Apr 2021 01:55:25 GMT  
		Size: 2.8 MB (2831352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357f30f35c6fec86bca9379563fdb04d55fe213ee84bd1420e28b98552afe9b7`  
		Last Modified: Thu, 01 Apr 2021 01:55:25 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae32874e27acb9ee817dd55194c7eccc50732a6022da4ac55bbc47f15357d230`  
		Last Modified: Thu, 01 Apr 2021 01:55:32 GMT  
		Size: 15.0 MB (15003537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef733171e7900467f17090409ee2b21137da306ddd359cdfbfb418414c607be`  
		Last Modified: Thu, 01 Apr 2021 01:55:24 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3528680e5b8bb107bd955af87ccbbab9fe616d67a017ade9451389156351381b`  
		Last Modified: Thu, 01 Apr 2021 01:55:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:07fbfadf677f11ba6f5a21bb80cc71c89935e590b41fcbb4dd32a286c462f501
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153367336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effc2857aaede31a6786c4ab07c68df3de6ac32584908d054a7362fc848b3750`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 06:00:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 06:00:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 06:01:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 06:01:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 06:01:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 06:10:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 06:10:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 06:10:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 06:10:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 06:25:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 06:25:25 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 06:25:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 06:25:26 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 06:25:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 06:25:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:29:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 06:29:02 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:29:05 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 06:29:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 06:29:07 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 06:29:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 06:29:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 06:29:12 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 06:29:13 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 06:45:08 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 01 Apr 2021 06:47:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 06:47:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 06:47:36 GMT
ENV MATOMO_VERSION=4.2.1
# Thu, 01 Apr 2021 06:48:06 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 06:48:09 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 01 Apr 2021 06:48:11 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 01 Apr 2021 06:48:13 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 06:48:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 06:48:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1d497f4e5ea580a3a4b8a826f8c71379d6e7a76bd10d45f32adbac91f61cb2`  
		Last Modified: Wed, 31 Mar 2021 07:09:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b603f7372a2390997a547c017682bbccabf5f4ff2e17c5a7ad87a6ece073a18`  
		Last Modified: Wed, 31 Mar 2021 07:10:00 GMT  
		Size: 70.4 MB (70355229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0372695364ccf5f16a3ecfb0185b21a24a456e1867b911685b0a4288ad4b313`  
		Last Modified: Wed, 31 Mar 2021 07:09:33 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6102fb158490ba1c6742944504a179df99068d74a0834a4fcb60b2cb06a4070`  
		Last Modified: Wed, 31 Mar 2021 07:13:06 GMT  
		Size: 10.7 MB (10655139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36bdb0bbdcbbf5cbfb2008f47034c81f0a3976b4e31c0ebeb60bc9ea88bed04`  
		Last Modified: Wed, 31 Mar 2021 07:13:03 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0e6ff5b63c805b42755f36262309e873aebd4bf5df2733c9d1401cbc3757d0`  
		Last Modified: Wed, 31 Mar 2021 07:13:12 GMT  
		Size: 28.3 MB (28334435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82b3dfaa5654b6c88b4c3b50a315248699063f78176d3262d60b856395faf24`  
		Last Modified: Wed, 31 Mar 2021 07:13:03 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f05ad8490526e74f3f5d03c95ae786282c6a0de4f57b8fad2088459c7b5a92f`  
		Last Modified: Wed, 31 Mar 2021 07:13:03 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ceea2e2edbba463b34b11daa2639178a11bd541e761d683ad165464daa2063f`  
		Last Modified: Wed, 31 Mar 2021 07:13:03 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29efd18aa6e5510d6e4325b02e90927649c1a7bec03479e9ece9ed58b83d39e`  
		Last Modified: Thu, 01 Apr 2021 06:49:13 GMT  
		Size: 3.1 MB (3100961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf301d4c8a02c436372dc2250bc8651bc5b4caba8bca810f3836cac67046421`  
		Last Modified: Thu, 01 Apr 2021 06:49:12 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdcb818914dbfe932d3fa3b6fb2250e9a2fb4692416ba15bbffe3c148e0d106`  
		Last Modified: Thu, 01 Apr 2021 06:49:17 GMT  
		Size: 15.0 MB (15004239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b98c675715d7def7c14dc3658069c024c5f87a543c31b9e139791fca29727ac`  
		Last Modified: Thu, 01 Apr 2021 06:49:12 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1869b0831cfc91b5e47e281f538cde89b4bf7eed8899961ad548f45f2695e9d`  
		Last Modified: Thu, 01 Apr 2021 06:49:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; 386

```console
$ docker pull matomo@sha256:11d06a1bd3564dd8b16f4e050a453e907dc0f1f6f5590b8a7126093f0d2d787d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (167011258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f042794e6e93148bdb2b2d25e16f34c676f7ff6191c67e38d45dc1fa3083a30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:38:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 05:38:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 05:39:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:39:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 05:39:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 05:50:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 05:50:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 05:50:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 05:50:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 06:10:51 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 06:10:51 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 06:10:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 06:10:52 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 06:11:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 06:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:17:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 06:17:46 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:17:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 06:17:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 06:17:47 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 06:17:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 06:17:48 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 06:17:48 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 06:17:49 GMT
CMD ["php-fpm"]
# Wed, 31 Mar 2021 16:08:27 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 31 Mar 2021 16:09:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:09:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 31 Mar 2021 16:09:53 GMT
ENV MATOMO_VERSION=4.2.1
# Wed, 31 Mar 2021 16:10:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:10:11 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 31 Mar 2021 16:10:11 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 31 Mar 2021 16:10:11 GMT
VOLUME [/var/www/html]
# Wed, 31 Mar 2021 16:10:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 16:10:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98b67b2c4467eacf10bfe3c2eef4cb9d9dc040023f3562413a987120aa2b38c`  
		Last Modified: Wed, 31 Mar 2021 07:32:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398a2808bbaf89e86620a60aae2b88361cd9f03abd0f3e9b04b43ddf645bbc2e`  
		Last Modified: Wed, 31 Mar 2021 07:32:39 GMT  
		Size: 81.2 MB (81230040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fe28765e314abeb61d6d24aeacc128e934cb1bea417f77e92842b06f368ca`  
		Last Modified: Wed, 31 Mar 2021 07:32:03 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1321d1e543a95f500c10fd2d962b71bdbeb025bae6cedd4d31be6d7e43b4f14`  
		Last Modified: Wed, 31 Mar 2021 07:39:16 GMT  
		Size: 10.7 MB (10655557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9645d4e10b074ec4b9844c76680070dc0dee2987c61b33bdc5c318ba081db91a`  
		Last Modified: Wed, 31 Mar 2021 07:39:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e861be914a6b052c85867cd7f9e31f0a394ad36d5ea02fc5a88e6dfeb78d23`  
		Last Modified: Wed, 31 Mar 2021 07:39:22 GMT  
		Size: 29.2 MB (29153434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e1aeab3afb9c0a7d850247ca3b592eb09769ff8a5e4e1a0070c48849022400`  
		Last Modified: Wed, 31 Mar 2021 07:39:11 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c4769162336a241ef03ce19a0e035bad04a12e9dec4ed10a7339f7620cf20`  
		Last Modified: Wed, 31 Mar 2021 07:39:13 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da6dc26d71175a03303b1657bd85562afaa23041d6dc6584fcb701bec920952`  
		Last Modified: Wed, 31 Mar 2021 07:39:11 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62f1a616b2fd786c11e94da437b5a9fcfca39dd15f6ad9e1e79c928a8ce68a8`  
		Last Modified: Wed, 31 Mar 2021 16:12:24 GMT  
		Size: 3.2 MB (3165966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4767ffaf65bfb63431afd1083e6bf2e4ba482969889f10e43c61eb5eb143f72`  
		Last Modified: Wed, 31 Mar 2021 16:12:24 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f718be26f589cbc92359bbccdbb3e1c22faddf741a97dad485781b74f778224`  
		Last Modified: Wed, 31 Mar 2021 16:12:27 GMT  
		Size: 15.0 MB (15004448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3096d9a184c8688025c285718c4773851cfa4b79b553bd2137f1374ea6e94ce`  
		Last Modified: Wed, 31 Mar 2021 16:12:23 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d46233ab6ed9214fe000fff12f9d3a343113f1f6009ca4cb42108631d1d3b24`  
		Last Modified: Wed, 31 Mar 2021 16:12:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; mips64le

```console
$ docker pull matomo@sha256:0f13622ebb2266ec647c024a665559c25ffe84272b2793792aa8976577349498
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143927386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04331cbe46f4c98e26d902e14a034495fb0c8290c0efa5073a93ec5bbced7ba7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:47 GMT
ADD file:b5b2f1fc18276a3928a2d904fedc2991239e065051f16680662a22627d15e809 in / 
# Tue, 30 Mar 2021 22:09:48 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 00:27:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 00:28:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:28:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 00:28:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 00:54:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 00:54:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:54:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:54:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 01:38:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 01:38:06 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 01:38:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 01:38:07 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 01:38:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 01:38:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:51:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 01:51:10 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:51:12 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 01:51:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 01:51:13 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 01:51:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 01:51:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 01:51:15 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 01:51:16 GMT
CMD ["php-fpm"]
# Wed, 31 Mar 2021 15:24:08 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 31 Mar 2021 15:28:20 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 15:28:22 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 31 Mar 2021 15:28:22 GMT
ENV MATOMO_VERSION=4.2.1
# Wed, 31 Mar 2021 15:28:55 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 15:28:56 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 31 Mar 2021 15:28:56 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 31 Mar 2021 15:28:57 GMT
VOLUME [/var/www/html]
# Wed, 31 Mar 2021 15:28:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 15:28:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:17fa7bb8f5ce4138c383674409fef134204b2ae72f4a997a2cebccad07e8e32b`  
		Last Modified: Tue, 30 Mar 2021 22:16:21 GMT  
		Size: 25.8 MB (25806366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352cbf73d26a044699ae2f07261cb972fea9bcddf88ba2198123b5deda9e10f4`  
		Last Modified: Wed, 31 Mar 2021 02:51:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d1191368872841cbb21ecc69ac171357d4b1e986c7a460dcb0bc3d060f095`  
		Last Modified: Wed, 31 Mar 2021 02:52:26 GMT  
		Size: 61.4 MB (61403934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cc22997f22b69d3ca6ba56580b5d4484b5ce25878d6418a118d57ba4f3901`  
		Last Modified: Wed, 31 Mar 2021 02:51:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d8dadc848c5700ba333cbec67367c629aec69fad1c5b01e9e90eb0ee66295`  
		Last Modified: Wed, 31 Mar 2021 02:57:41 GMT  
		Size: 10.7 MB (10653547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62ca65b964ace7379c2f456310ea0c2cdc442e2ca5cde1fb518d83617b6cf5`  
		Last Modified: Wed, 31 Mar 2021 02:57:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4196270806704543539f9b562acdc331ae0296e2e15b8b04ac05af4a5c3905d3`  
		Last Modified: Wed, 31 Mar 2021 02:57:55 GMT  
		Size: 28.0 MB (27950685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f379443061bf3e47dc86549f33192e18245dd86df64d2ffbddd07bc8f54bcb89`  
		Last Modified: Wed, 31 Mar 2021 02:57:35 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e9b690e51359d8c3c48b92beb02c2680811256cb510f3330ed4bac535eb041`  
		Last Modified: Wed, 31 Mar 2021 02:57:35 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee649ce0aa8a119be500557d09960ee0272440539858cf02191ea9aa648f3fd7`  
		Last Modified: Wed, 31 Mar 2021 02:57:35 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb57ed5a32fe7d16b651577ae3109ee8607ca750a08c95b2d274cee99dcf87f`  
		Last Modified: Wed, 31 Mar 2021 15:30:14 GMT  
		Size: 3.1 MB (3097111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fa66c8ae704dd18b76417cec0b0bfc7792594a5bbd6ed11044b90407fc09a4`  
		Last Modified: Wed, 31 Mar 2021 15:30:12 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbd6240e83593c63c2ef4642884f83355663c062c5921df31dad19c9b50a923`  
		Last Modified: Wed, 31 Mar 2021 15:30:24 GMT  
		Size: 15.0 MB (15002975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce19c77d4b234c01b60338a7289de9139b7549d8e92d072aad6ce9b43188f32`  
		Last Modified: Wed, 31 Mar 2021 15:30:11 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b327f4e7288c5ab827a3436f9fa797ad6d5d4e0935c0f0661ccf7c4d5f235f`  
		Last Modified: Wed, 31 Mar 2021 15:30:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; ppc64le

```console
$ docker pull matomo@sha256:6280872209af8fcc064147f70c047f553a5210941b85307279392ee1e786dc2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.2 MB (172157341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33a8fea152e2a3fab62423b6f911edcbf09c72435105004dffc9b5e4b600afe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 22:36:03 GMT
ADD file:a544303d3ec263b38c231310d807e05249140188df5c5a5c785b2f176455ac39 in / 
# Tue, 30 Mar 2021 22:36:09 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 11:09:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 11:09:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 11:12:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 11:13:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 11:13:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 11:31:45 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 11:31:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 11:31:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 11:31:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 12:04:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 12:04:28 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 12:04:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 12:04:35 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 12:06:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 12:06:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 12:11:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 12:11:21 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 12:11:37 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 12:11:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 12:11:45 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 12:11:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 12:11:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 12:11:58 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 12:12:00 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 07:30:11 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 01 Apr 2021 07:32:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 07:32:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 07:32:45 GMT
ENV MATOMO_VERSION=4.2.1
# Thu, 01 Apr 2021 07:34:40 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 07:34:50 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 01 Apr 2021 07:34:56 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 01 Apr 2021 07:34:58 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 07:35:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 07:35:08 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c840eb5e9aed613b2af7557a4b5ad46898b8bc475a2d470c65ec7896b11282f1`  
		Last Modified: Tue, 30 Mar 2021 22:42:39 GMT  
		Size: 30.5 MB (30545907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609c2a62923b5b74c89e0e6a2975907d38aaa4e4c04d3a1c50454f163d588a55`  
		Last Modified: Wed, 31 Mar 2021 12:55:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5446013ea62187f1851814ee5a76ef3a061d2679ada7116792838147e136e`  
		Last Modified: Wed, 31 Mar 2021 12:56:12 GMT  
		Size: 82.3 MB (82290930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b7faded87e67bbc5dbb85edd1f7549536cb4ac88fed061610320ac232046ea`  
		Last Modified: Wed, 31 Mar 2021 12:55:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9120cd3194c261c8c8d41dca36e7bfc464e70b4825fc2bd36a31dc704bc107d9`  
		Last Modified: Wed, 31 Mar 2021 13:00:25 GMT  
		Size: 10.7 MB (10656267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d296600e09d03777ac8a19f06bb6e1f668ea3da7002270871be22334253f3c8f`  
		Last Modified: Wed, 31 Mar 2021 13:00:17 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365c50428f4e16ba237dfbe4933d0162e191564af9000a545378232dd4a238b`  
		Last Modified: Wed, 31 Mar 2021 13:00:24 GMT  
		Size: 30.3 MB (30258207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070aceba451b8fa2149b44cdf55a5e9c1827729d08e8582fe924796a9bc4a90e`  
		Last Modified: Wed, 31 Mar 2021 13:00:17 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a177f5261ae42b6f3af9affbbd793adf920649ea81cfd77a70cf2eafea3f1478`  
		Last Modified: Wed, 31 Mar 2021 13:00:17 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e5fff19229ac55b38f85bb403498abbee48cae5ebf0d32a3bf7b57ef3f9179`  
		Last Modified: Wed, 31 Mar 2021 13:00:18 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5df5ab906519a0f1281c6cdc0407d94c188b511619732769e90e5461ffc90e`  
		Last Modified: Thu, 01 Apr 2021 07:36:21 GMT  
		Size: 3.4 MB (3387472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7085137efc3a8502abce56b18bac5ba42f69ac6f62938e8d549f633c2194fb`  
		Last Modified: Thu, 01 Apr 2021 07:36:20 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b61d227e623c0769f2f7ca13d9187808fd6fe33e59e1347ba7410682077896`  
		Last Modified: Thu, 01 Apr 2021 07:36:25 GMT  
		Size: 15.0 MB (15005736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df27cad7328778f702ca48bf3110401bcf6696687d12d8b1696106a0060c7a18`  
		Last Modified: Thu, 01 Apr 2021 07:36:20 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9793fea02fb298d867cbdeb93e03c7e2d7ff90223c2d5a6720ba66a0b13faff6`  
		Last Modified: Thu, 01 Apr 2021 07:36:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm` - linux; s390x

```console
$ docker pull matomo@sha256:e53c8bf60d3d5fcbeb05329e67f8af0773296840f8d783984aec8139f1a9c0e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146914763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7cc570d3eed5a0dfc6d4039fff1ec89361d63241ae92b4ba4aa260eb593ddbf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:59:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 30 Mar 2021 23:59:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 30 Mar 2021 23:59:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:59:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Mar 2021 23:59:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 00:09:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 00:09:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:09:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:09:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 00:21:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 00:21:21 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 00:21:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 00:21:22 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 00:21:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 00:21:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:25:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 00:25:08 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:25:08 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 00:25:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 00:25:09 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 00:25:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 00:25:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 00:25:11 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 00:25:11 GMT
CMD ["php-fpm"]
# Wed, 31 Mar 2021 08:59:28 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 31 Mar 2021 09:02:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:02:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 31 Mar 2021 09:02:19 GMT
ENV MATOMO_VERSION=4.2.1
# Wed, 31 Mar 2021 09:02:48 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:02:55 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 31 Mar 2021 09:02:55 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 31 Mar 2021 09:02:56 GMT
VOLUME [/var/www/html]
# Wed, 31 Mar 2021 09:02:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 09:02:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371213f07fea0a0f872bf0d091f7465c36fa7dda5dd5954941ab4416869b7059`  
		Last Modified: Wed, 31 Mar 2021 00:43:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938cc915f5117d6a5b05f98b4d0e1f7f16367df8d2bdb348a42a011d67843718`  
		Last Modified: Wed, 31 Mar 2021 00:44:02 GMT  
		Size: 64.7 MB (64709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02470c7dad2d8dd8f8186e20fe6e989a534273373e80b8c45eb2afc1cd562287`  
		Last Modified: Wed, 31 Mar 2021 00:43:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c154eb1630eabecb460fc8372090099af3a08d4d9205c0480b650bf20c56de`  
		Last Modified: Wed, 31 Mar 2021 00:48:03 GMT  
		Size: 10.7 MB (10654498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2295b91965b29324ea4a0f61aed9bb67b4490343bfeab0b2ba04acb59330f28`  
		Last Modified: Wed, 31 Mar 2021 00:48:00 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec7b35a44ecbf9bbd49f746c4be1f8172a8d0e65f1207e91300d90fd33b2f6d`  
		Last Modified: Wed, 31 Mar 2021 00:48:04 GMT  
		Size: 27.7 MB (27686441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2726db42a024f0426abcd9519e41e7657a8f47f6036ff94019c15028b01da6b3`  
		Last Modified: Wed, 31 Mar 2021 00:48:00 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bcf9c94af738669aecd4be2d4127c2ca208ea2367266d375145f0804244fb2`  
		Last Modified: Wed, 31 Mar 2021 00:48:00 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51002783a640b7f8a9656724e3cdf4b5a4d5e8dd7e93c42db28ac63729774044`  
		Last Modified: Wed, 31 Mar 2021 00:48:00 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4419ba835a9378562ff129ec5e64c6e522fb30414e857bedbbf3c3baea64e7a`  
		Last Modified: Wed, 31 Mar 2021 09:03:55 GMT  
		Size: 3.1 MB (3093918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4918a9297801a9365f54b2370e43ad5b2d4c85be9e291e846ed06e4d37b14f64`  
		Last Modified: Wed, 31 Mar 2021 09:03:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480a849945458a810f03c6e0269ba72621460ed6b0e750fa86688a97efc7f7aa`  
		Last Modified: Wed, 31 Mar 2021 09:03:58 GMT  
		Size: 15.0 MB (15003839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edcb286e8650cee88480fda87d9bc4a63c658a7168c09c267112026dc2386de`  
		Last Modified: Wed, 31 Mar 2021 09:03:54 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ca9f280f0129cf7da10f72d8547ccdcda3c8b0daf7305368258539c70b561`  
		Last Modified: Wed, 31 Mar 2021 09:03:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
