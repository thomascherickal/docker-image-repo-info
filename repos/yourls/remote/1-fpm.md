## `yourls:1-fpm`

```console
$ docker pull yourls@sha256:f3428e4bd35948d2c916b6ad08d36851eac94a993e10512bd18ca13d1b966672
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

### `yourls:1-fpm` - linux; amd64

```console
$ docker pull yourls@sha256:19b64ba4d698f40a077daa4937b4b2ccec4894f92be3c0104e11f3da2feb0cd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167151998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab54d91e7a63437f7a401b3af33be26741147eb5fae508ad2d3740b183327f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:30:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 19:30:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 19:30:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:30:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 19:30:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 19:30:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 19:30:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 19:30:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 20:28:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 21 Dec 2021 20:28:49 GMT
ENV PHP_VERSION=8.0.14
# Tue, 21 Dec 2021 20:28:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Tue, 21 Dec 2021 20:28:49 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Tue, 21 Dec 2021 20:29:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 20:29:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 20:52:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 20:52:22 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 21 Dec 2021 20:52:23 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 20:52:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 20:52:24 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 20:52:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 21 Dec 2021 20:52:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Dec 2021 20:52:26 GMT
EXPOSE 9000
# Tue, 21 Dec 2021 20:52:27 GMT
CMD ["php-fpm"]
# Wed, 22 Dec 2021 12:53:06 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 22 Dec 2021 12:53:06 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 22 Dec 2021 12:53:06 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 22 Dec 2021 12:53:06 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 22 Dec 2021 12:53:07 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 22 Dec 2021 12:53:07 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 22 Dec 2021 12:53:07 GMT
LABEL org.opencontainers.image.version=1.8.2
# Wed, 22 Dec 2021 12:53:53 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 22 Dec 2021 12:53:53 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Dec 2021 12:53:55 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 22 Dec 2021 12:53:55 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Wed, 22 Dec 2021 12:53:56 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Wed, 22 Dec 2021 12:53:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 12:53:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5608244554dec85339ec1c4946f2ed8998a1d9e8592283a13dd7a6169919656`  
		Last Modified: Tue, 21 Dec 2021 22:41:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d07066487a0cbf4adc6fef4372421dfd28c101b62eb404118e440133b65d422`  
		Last Modified: Tue, 21 Dec 2021 22:42:04 GMT  
		Size: 91.6 MB (91604190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6dfaf1958c6d3e5fad6e48d4e8a6df231e94d65bde1c3df6a971203da8a1d5`  
		Last Modified: Tue, 21 Dec 2021 22:41:47 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355a67f4a30887dfd487604787f9a016ed56e2cc26421fae0f8097a45ddc521e`  
		Last Modified: Tue, 21 Dec 2021 22:46:47 GMT  
		Size: 11.2 MB (11178073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b540e144b47fd901031c68e3f9567ab9061de6af2a5eff329672042294e2638d`  
		Last Modified: Tue, 21 Dec 2021 22:46:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f147acc1d50d28cbb0c11dd78e46092b5b7d74d591e0a8cc2a1229bbb0e459d5`  
		Last Modified: Tue, 21 Dec 2021 22:47:46 GMT  
		Size: 29.8 MB (29754941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88e574d983facf02d18d332cbe5d9f2836cf0b089bcdc168bc584633fd335e5`  
		Last Modified: Tue, 21 Dec 2021 22:47:41 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c8268e38be8026d3fcf2306d4ca67d2f8e4eea85755e5199a210f06039de68`  
		Last Modified: Tue, 21 Dec 2021 22:47:41 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38cd1d70246e6f0745b79df52553722b15dd66d98a2ed9e811cd4c4c0a6fd2d`  
		Last Modified: Tue, 21 Dec 2021 22:47:41 GMT  
		Size: 8.6 KB (8575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6b5032074f1618d9bd9bae7af5fb619e2a11dfd3a9973be8e6814784b468f7`  
		Last Modified: Wed, 22 Dec 2021 12:55:02 GMT  
		Size: 666.7 KB (666689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5dd271a89e876f198f05b8b0ab3ce1cb634141155a0482e30a9746e5d2df05`  
		Last Modified: Wed, 22 Dec 2021 12:55:02 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ac3f1b66da86eeabc64808870b42a61db17476d3ab21737448001139a4bd9e`  
		Last Modified: Wed, 22 Dec 2021 12:55:02 GMT  
		Size: 2.6 MB (2574445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8973a517cc9b4a1fb0a8cb5fe34265c7f5d85276dfb293da215c29807bcc3d`  
		Last Modified: Wed, 22 Dec 2021 12:55:02 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09541d1b7503a22daf3d51c3778edc06e0cbfea90372594038ee8967927d659b`  
		Last Modified: Wed, 22 Dec 2021 12:55:02 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:f723041adfa973bff752e8feec58faaa7a5541a5effd0a095136d1460be48324
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144702517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:019314152d16ba41bdf013fef2978074f279629b91ef2da94c206596102eebd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:13:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:13:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:14:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:14:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:14:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 01:14:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:14:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:14:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 02:02:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 18 Dec 2021 01:35:58 GMT
ENV PHP_VERSION=8.0.14
# Sat, 18 Dec 2021 01:35:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Sat, 18 Dec 2021 01:35:59 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Sat, 18 Dec 2021 01:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 18 Dec 2021 01:36:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 18 Dec 2021 01:53:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 18 Dec 2021 01:53:52 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 18 Dec 2021 01:53:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 18 Dec 2021 01:53:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 18 Dec 2021 01:53:54 GMT
WORKDIR /var/www/html
# Sat, 18 Dec 2021 01:53:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 18 Dec 2021 01:53:56 GMT
STOPSIGNAL SIGQUIT
# Sat, 18 Dec 2021 01:53:57 GMT
EXPOSE 9000
# Sat, 18 Dec 2021 01:53:57 GMT
CMD ["php-fpm"]
# Sat, 18 Dec 2021 05:22:27 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 18 Dec 2021 05:22:28 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 18 Dec 2021 05:22:28 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 18 Dec 2021 05:22:29 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 18 Dec 2021 05:22:29 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 18 Dec 2021 05:22:29 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 18 Dec 2021 05:22:30 GMT
LABEL org.opencontainers.image.version=1.8.2
# Sat, 18 Dec 2021 05:23:44 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 18 Dec 2021 05:23:46 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Dec 2021 05:23:49 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 18 Dec 2021 05:23:50 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 18 Dec 2021 05:23:50 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Sat, 18 Dec 2021 05:23:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 05:23:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b027b55d12ad9ac869559247a51c3128131e902296b69d94ad0923affd65b49`  
		Last Modified: Fri, 03 Dec 2021 04:21:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f66ff2b781e02c0d613433e3c079cab11ef176f78cc3ef16fd441f40132e9f5`  
		Last Modified: Fri, 03 Dec 2021 04:22:42 GMT  
		Size: 73.7 MB (73684131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67de67500ee532057975d51ed0340f7d279a7a7cf82659d1b3965733f8b47937`  
		Last Modified: Fri, 03 Dec 2021 04:21:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0059198c803d536397578db3fdd5073d447341d616f49c0e994e4e166968efc`  
		Last Modified: Sat, 18 Dec 2021 02:43:46 GMT  
		Size: 11.2 MB (11176492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a3cf1371afa09e377e8489059c91e9acaa153ced441de0d815ec9ce88dac54`  
		Last Modified: Sat, 18 Dec 2021 02:43:42 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3aa136a594d0420ae93654cd7fbd32ba5973fd239ad58bf44f49fe33a222c6`  
		Last Modified: Sat, 18 Dec 2021 02:45:28 GMT  
		Size: 28.0 MB (28021079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5280859f535c5ef93b3004a602e1e4fcaa639e4038e96d5650ca26dc7d9e1fcb`  
		Last Modified: Sat, 18 Dec 2021 02:45:10 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0114a25589de4112cdba9cb1cfa09ae9ac2a8cc4e070d789230fae6af5f06d`  
		Last Modified: Sat, 18 Dec 2021 02:45:10 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603f24dcf3f9d7f2f0133e30d82a08a6e6cf8af9ce4e697d893b75c295bf243e`  
		Last Modified: Sat, 18 Dec 2021 02:45:10 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5667b0ff4956f8e6f20e3f02e8c7fbed1810692a4adbda822e2e7f6e8a512804`  
		Last Modified: Sat, 18 Dec 2021 05:25:40 GMT  
		Size: 319.5 KB (319501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a681f8175d64e87a5d796475c8dad281097d2594f9b6e91f34422c1a1f49bb55`  
		Last Modified: Sat, 18 Dec 2021 05:25:40 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b91134f24df32c9d9bd0c8b10a64cc32dc9b04ad39200a805bf3e6e3cdf823`  
		Last Modified: Sat, 18 Dec 2021 05:25:42 GMT  
		Size: 2.6 MB (2574446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de457e711f318af4a609e843b4d4dc50e723be92c327270cce31f38f77a91cfa`  
		Last Modified: Sat, 18 Dec 2021 05:25:40 GMT  
		Size: 2.0 KB (2044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7048f0d17105ea9a719ce0585c85b5109f6806aeb646d226f0f06e3a673d161f`  
		Last Modified: Sat, 18 Dec 2021 05:25:40 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:633cbdba5cee4ff34cc9c8fee54371adb2b497e359acc6beb132bd0209a2b856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136954230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97026ad79737afdeb303404c836e64c862c74abc325b95a93614e35b6289aca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 23:36:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 23:36:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 23:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 23:37:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 23:37:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 23:37:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 23:37:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 23:37:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 00:22:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 18 Dec 2021 01:28:28 GMT
ENV PHP_VERSION=8.0.14
# Sat, 18 Dec 2021 01:28:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Sat, 18 Dec 2021 01:28:29 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Sat, 18 Dec 2021 01:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 18 Dec 2021 01:28:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 18 Dec 2021 01:43:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 18 Dec 2021 01:43:13 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 18 Dec 2021 01:43:15 GMT
RUN docker-php-ext-enable sodium
# Sat, 18 Dec 2021 01:43:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 18 Dec 2021 01:43:16 GMT
WORKDIR /var/www/html
# Sat, 18 Dec 2021 01:43:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 18 Dec 2021 01:43:18 GMT
STOPSIGNAL SIGQUIT
# Sat, 18 Dec 2021 01:43:19 GMT
EXPOSE 9000
# Sat, 18 Dec 2021 01:43:19 GMT
CMD ["php-fpm"]
# Sat, 18 Dec 2021 09:12:31 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 18 Dec 2021 09:12:31 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 18 Dec 2021 09:12:32 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 18 Dec 2021 09:12:32 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 18 Dec 2021 09:12:33 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 18 Dec 2021 09:12:33 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 18 Dec 2021 09:12:34 GMT
LABEL org.opencontainers.image.version=1.8.2
# Sat, 18 Dec 2021 09:13:45 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 18 Dec 2021 09:13:47 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Dec 2021 09:13:50 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 18 Dec 2021 09:13:51 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 18 Dec 2021 09:13:51 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Sat, 18 Dec 2021 09:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 09:13:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50ffdc47d6f068811ac71535715f43a36fe261bbb0c3e31f43186a2282c558b`  
		Last Modified: Fri, 03 Dec 2021 02:41:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bef2d8d286eef83c2c19371d6f497a886c348995670857a897340992fbf33c`  
		Last Modified: Fri, 03 Dec 2021 02:42:37 GMT  
		Size: 69.3 MB (69315176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5d96c53a2bfbf975478318788fcea14a43e10e632584b962131667404f99ec`  
		Last Modified: Fri, 03 Dec 2021 02:41:55 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf51bcfe8d55a19078431fc83d3ca64f4c51a1574b396d9228b2c68c152733b`  
		Last Modified: Sat, 18 Dec 2021 03:03:36 GMT  
		Size: 11.2 MB (11176497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ed2278179c5e9c7581439fdeda1ca5d91550c64bd0de78cc816a9805527bd8`  
		Last Modified: Sat, 18 Dec 2021 03:03:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000c1d4c7875eea62b7f9e1705bbe24e5fde9f00b98698d91214b2b4034db678`  
		Last Modified: Sat, 18 Dec 2021 03:05:16 GMT  
		Size: 27.0 MB (27011165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2888023cd6bd394f0d7b5189e6579d6dafa693ef1ca5125ac47eca83fb90166c`  
		Last Modified: Sat, 18 Dec 2021 03:05:00 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e4f0dd6dd04ee04c968be98e801c4cf1b941dbdc633ed030b9a3402793bd1a`  
		Last Modified: Sat, 18 Dec 2021 03:05:00 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e6cf478d7811b3de5659eb6229475870017764fc1ac50f2482d1fa164b7fdb`  
		Last Modified: Sat, 18 Dec 2021 03:05:00 GMT  
		Size: 8.6 KB (8576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e769ef8f04da480cfd858d24af06308bd11f5d09bc893f31e3b45b948b20707`  
		Last Modified: Sat, 18 Dec 2021 09:17:39 GMT  
		Size: 287.7 KB (287716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec02969706ade2e7b28e7fa622c97a746ac521a273a29370afc5cc515bdfdc2e`  
		Last Modified: Sat, 18 Dec 2021 09:17:39 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e628b8fb2a52354404e855b6a43d0a35b4f840b4720943d17f6908a7b50cdd`  
		Last Modified: Sat, 18 Dec 2021 09:17:41 GMT  
		Size: 2.6 MB (2574445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa0181a1d49e27cc6e75d4b5d48e58e40009b02acde6bb85371d287ee18e87`  
		Last Modified: Sat, 18 Dec 2021 09:17:39 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04c4ad8cb916f3e02c26373ef0c1290830a5b8083d5fb515ac71d9509cee888`  
		Last Modified: Sat, 18 Dec 2021 09:17:39 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:245e59bdde560d28005cdb83d33e9d886fbe09090cbb9bd714bff92443ad31e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159739694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3c5a4a09d759cdaf5447f97fc06a5ad831ef1f98a5bd65f5649042352d3510`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 03:35:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 03:35:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:35:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 03:35:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 03:35:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:35:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:35:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 04:10:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 21 Dec 2021 04:10:27 GMT
ENV PHP_VERSION=8.0.14
# Tue, 21 Dec 2021 04:10:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Tue, 21 Dec 2021 04:10:29 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Tue, 21 Dec 2021 04:10:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 04:10:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:19:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 04:19:03 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:19:03 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 04:19:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 04:19:05 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 04:19:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 21 Dec 2021 04:19:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Dec 2021 04:19:08 GMT
EXPOSE 9000
# Tue, 21 Dec 2021 04:19:09 GMT
CMD ["php-fpm"]
# Wed, 22 Dec 2021 02:00:11 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 22 Dec 2021 02:00:12 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 22 Dec 2021 02:00:13 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 22 Dec 2021 02:00:14 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 22 Dec 2021 02:00:15 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 22 Dec 2021 02:00:16 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 22 Dec 2021 02:00:17 GMT
LABEL org.opencontainers.image.version=1.8.2
# Wed, 22 Dec 2021 02:00:41 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 22 Dec 2021 02:00:42 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Dec 2021 02:00:44 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 22 Dec 2021 02:00:45 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Wed, 22 Dec 2021 02:00:46 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Wed, 22 Dec 2021 02:00:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 02:00:47 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fabbcc6f532a6a8b531637691358450f915c31905ac07c8bafef41a6529224`  
		Last Modified: Tue, 21 Dec 2021 05:22:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e737003186221828fccfeddc973f0e3dc6c217db56d064ad52aff59977d933`  
		Last Modified: Tue, 21 Dec 2021 05:22:19 GMT  
		Size: 86.9 MB (86920347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7adcc66be5bd6c34225cc77d6a19284e8c323df6241875eb616acb8cddd9011`  
		Last Modified: Tue, 21 Dec 2021 05:22:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8045df9b04d8fcb21f6ebaf4d4aa9cdab57ddb17edba7ab9d08ddc5a7f975497`  
		Last Modified: Tue, 21 Dec 2021 05:27:24 GMT  
		Size: 11.0 MB (10961476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75696ae08de9c13c65be82fbf1cb3ee243b6f8c182bde15668128e6a533e520f`  
		Last Modified: Tue, 21 Dec 2021 05:27:23 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1441d6abd933018ad5be2283ff49db0aa9834a89e9438fd5ab83f25894dbdc6`  
		Last Modified: Tue, 21 Dec 2021 05:28:24 GMT  
		Size: 28.9 MB (28891561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23f13e5842de1a05ef2c3c63907eabc00b4fa3e90868d9193fef5022696b57`  
		Last Modified: Tue, 21 Dec 2021 05:28:20 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f3c133db6349743400fc4946b293734b8455bf40cb213a0fa56b528560e16`  
		Last Modified: Tue, 21 Dec 2021 05:28:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98baabe9b4355ff631502cabe86e55a9ea7f2228bf970d103d069c81aba8a392`  
		Last Modified: Tue, 21 Dec 2021 05:28:20 GMT  
		Size: 8.6 KB (8577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c9c0b024c11dd4b8495ab7a7266778951b1f891e53c465ddb08542a99fd3ea`  
		Last Modified: Wed, 22 Dec 2021 02:02:12 GMT  
		Size: 331.0 KB (331012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708f00ca31cc27199cd2816f65a56fa94c6c6a0a312cadb97548b196a4c3c57d`  
		Last Modified: Wed, 22 Dec 2021 02:02:12 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd425793f28dcf3bbae84ff8b1b11b597d033076a91f3abacf85d696b7fb2f3`  
		Last Modified: Wed, 22 Dec 2021 02:02:12 GMT  
		Size: 2.6 MB (2575512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7656a26ccd8bd1893dce106f6d3062145b627035e7c20ed4b3ed5f71942a4c`  
		Last Modified: Wed, 22 Dec 2021 02:02:12 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01889dbf65c345dd81cb9f03e3ef1ca00c572fcc102e4141c8bf4ee5a38589ae`  
		Last Modified: Wed, 22 Dec 2021 02:02:12 GMT  
		Size: 1.6 KB (1550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; 386

```console
$ docker pull yourls@sha256:2157fab4fdcc839fea5a303d8958cdf757e3023c0427b039d85f66d274844a9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169781414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4d2e21513a1155636e69966c82b11c78cad31e23f16254f2190b09198b032c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:55:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 12:55:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 12:55:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:55:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 12:55:46 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 12:55:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 12:55:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 12:55:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 13:51:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 21 Dec 2021 13:51:44 GMT
ENV PHP_VERSION=8.0.14
# Tue, 21 Dec 2021 13:51:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Tue, 21 Dec 2021 13:51:44 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Tue, 21 Dec 2021 13:52:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 13:52:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 14:16:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 14:16:11 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 21 Dec 2021 14:16:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 14:16:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 14:16:14 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 14:16:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 21 Dec 2021 14:16:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Dec 2021 14:16:16 GMT
EXPOSE 9000
# Tue, 21 Dec 2021 14:16:16 GMT
CMD ["php-fpm"]
# Wed, 22 Dec 2021 08:52:29 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 22 Dec 2021 08:52:29 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 22 Dec 2021 08:52:29 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 22 Dec 2021 08:52:30 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 22 Dec 2021 08:52:30 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 22 Dec 2021 08:52:30 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 22 Dec 2021 08:52:31 GMT
LABEL org.opencontainers.image.version=1.8.2
# Wed, 22 Dec 2021 08:53:39 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 22 Dec 2021 08:53:40 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Dec 2021 08:53:43 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 22 Dec 2021 08:53:43 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Wed, 22 Dec 2021 08:53:44 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Wed, 22 Dec 2021 08:53:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 08:53:44 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3024a970d01a7ef049e3539cd86216f2b9ba836cc7349134a8daac2cd7967a3`  
		Last Modified: Tue, 21 Dec 2021 17:08:50 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c53ffbaa8e42e904ade656bec770a649d2440f23381661e50812c484003c32`  
		Last Modified: Tue, 21 Dec 2021 17:09:29 GMT  
		Size: 92.7 MB (92715879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401ee648bb0837c49fd04dd8d305a1106b6d151227c0f56981dbb1efba74aa4`  
		Last Modified: Tue, 21 Dec 2021 17:08:50 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff3e79660606573b66a5d4f4dc5b58ab56088519ff60f701741d8effb83c985`  
		Last Modified: Tue, 21 Dec 2021 17:16:39 GMT  
		Size: 11.2 MB (11177251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4dece9aebec9625a5c560262d9b28ff394053877eded204bbba7612d12d54c`  
		Last Modified: Tue, 21 Dec 2021 17:16:38 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee40abf813c45667d1ce84aaf7c6f62aa0c6811ccad6665b826678b937249ff`  
		Last Modified: Tue, 21 Dec 2021 17:18:15 GMT  
		Size: 30.3 MB (30281052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca4eb461db2ef194fbc39ce99e61e7f27ac2c40662c7ef4ef8fe6d6154550db`  
		Last Modified: Tue, 21 Dec 2021 17:18:04 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ca29324739e07959569607304f3a37f12aa7a2bfdfb4d8832c0825c98bef4`  
		Last Modified: Tue, 21 Dec 2021 17:18:03 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857dfa8bbb9f4cfa87a1bd86048891d349165f4e9534fa7c23f32a5f84501a92`  
		Last Modified: Tue, 21 Dec 2021 17:18:03 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923f2d5f5c600ce3e470b5581dcc97c2bf9e01ca151971782a5836ef2c246dc`  
		Last Modified: Wed, 22 Dec 2021 08:55:20 GMT  
		Size: 645.9 KB (645896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b333e0c4a6288fe17487feafb8a970a7c3be123f3f5c7fd191867c746b9cc3da`  
		Last Modified: Wed, 22 Dec 2021 08:55:20 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eafc7d9484dbb06fb718074ebaf9e63276056b09a45e2513bcb31b3e95c469`  
		Last Modified: Wed, 22 Dec 2021 08:55:21 GMT  
		Size: 2.6 MB (2574445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f249d00784ac1c21605fddac0bf79b56619c01c0f4b90726e15e75c7dbc445`  
		Last Modified: Wed, 22 Dec 2021 08:55:20 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d58669ff513f8f7ac892b30efb8d193dcf0974581e759b08f991bcd39c1809`  
		Last Modified: Wed, 22 Dec 2021 08:55:20 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:85fe035d3bf4df30ec7f03c8de2c6b7cbf965102363bfb2d2613ddf3dfb738a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144490899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c3ecf881859f5feb1d803e6d439d4868274cd982c698d12eaa358116df3250`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:10 GMT
ADD file:419aff162077eb16923c3ede6455ca86756a929a5a837bc6ac6b8dc67913503a in / 
# Thu, 02 Dec 2021 03:09:10 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 12:32:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 12:32:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 12:33:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:33:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 12:33:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 12:33:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 12:34:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 12:34:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 14:21:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 18 Dec 2021 01:52:52 GMT
ENV PHP_VERSION=8.0.14
# Sat, 18 Dec 2021 01:52:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Sat, 18 Dec 2021 01:52:53 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Sat, 18 Dec 2021 01:53:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 18 Dec 2021 01:53:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 18 Dec 2021 02:32:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 18 Dec 2021 02:32:10 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 18 Dec 2021 02:32:12 GMT
RUN docker-php-ext-enable sodium
# Sat, 18 Dec 2021 02:32:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 18 Dec 2021 02:32:12 GMT
WORKDIR /var/www/html
# Sat, 18 Dec 2021 02:32:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 18 Dec 2021 02:32:15 GMT
STOPSIGNAL SIGQUIT
# Sat, 18 Dec 2021 02:32:15 GMT
EXPOSE 9000
# Sat, 18 Dec 2021 02:32:15 GMT
CMD ["php-fpm"]
# Sat, 18 Dec 2021 08:24:12 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 18 Dec 2021 08:24:13 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 18 Dec 2021 08:24:13 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 18 Dec 2021 08:24:13 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 18 Dec 2021 08:24:14 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 18 Dec 2021 08:24:14 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 18 Dec 2021 08:24:14 GMT
LABEL org.opencontainers.image.version=1.8.2
# Sat, 18 Dec 2021 08:25:46 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 18 Dec 2021 08:25:48 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Dec 2021 08:25:52 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 18 Dec 2021 08:25:52 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 18 Dec 2021 08:25:53 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Sat, 18 Dec 2021 08:25:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 08:25:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:df61fb15db6391af55d70bc3c0db3e9014438c81bf802619fb527221adf5e8a8`  
		Last Modified: Thu, 02 Dec 2021 03:17:58 GMT  
		Size: 29.6 MB (29630496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83c1e85b8a7d8f4eac1893af0c207b44ba6740c84b242afaf7d96af4a26120b`  
		Last Modified: Fri, 03 Dec 2021 18:41:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124389778aab42ee498bcb3c59b91b0d2d14f182fd993a4560f80bc5de07b749`  
		Last Modified: Fri, 03 Dec 2021 18:42:42 GMT  
		Size: 72.0 MB (72013733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf72b6001435333c90ef2102c1791b7223d8a3068ff8eaad536bd904a50a3fb5`  
		Last Modified: Fri, 03 Dec 2021 18:41:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730d8acb8a698088fdc085b5fd3fa32a371aab6fe6cf991532979830d185f92`  
		Last Modified: Sat, 18 Dec 2021 03:55:56 GMT  
		Size: 11.2 MB (11175844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c25d7c09274cea9245512cdab24def3b280829a12ed477cf26bf189f5682e6`  
		Last Modified: Sat, 18 Dec 2021 03:55:51 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618b95af4a310d27c79471eb862be147fd8041673a9ed078936d368ccb239620`  
		Last Modified: Sat, 18 Dec 2021 03:59:32 GMT  
		Size: 28.8 MB (28750527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14b0bef1c7107e6f5abe5f853cba600f48d23b8cd6c99784f5528e6d7fc88a8`  
		Last Modified: Sat, 18 Dec 2021 03:59:09 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04fb2f8df42ca7fec8d47bef1c9d3ec69d861046077585b4aa44acb11426630`  
		Last Modified: Sat, 18 Dec 2021 03:59:11 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a493579d708487c81c64ecc88163a92968c52e34cb46b4b9c5e3906c597005e`  
		Last Modified: Sat, 18 Dec 2021 03:59:10 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e88e496a00260131cdb824a7f92a3430b5983000a73d216a68cffefecb6e361`  
		Last Modified: Sat, 18 Dec 2021 08:27:09 GMT  
		Size: 329.9 KB (329904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c72e049498a5e55d0835f7bf654018402709e428f5d589be82b4148d568ab8`  
		Last Modified: Sat, 18 Dec 2021 08:27:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e289e0189382290ac9e2bdceab32f91b8ad6fd5d5517df2f84682155bed060`  
		Last Modified: Sat, 18 Dec 2021 08:27:11 GMT  
		Size: 2.6 MB (2574414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a5145f8fa52f821a283b800b7787d6d9506350eadf35d94c966376b2d099a7`  
		Last Modified: Sat, 18 Dec 2021 08:27:13 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff347db9f66ab8f5bfdad49f14fda64c1ff0d0cccddb6cf3a31c2e317dcedc`  
		Last Modified: Sat, 18 Dec 2021 08:27:08 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:4b0f3e546576dccc622c61cbff13915a0f3963b455389583f75b504f2561ffcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.1 MB (167104031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:611aa65b564ce57ee1958318729b469d4e9ec7341ad9a4e35fcf78ea301095e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 06:34:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 06:34:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 06:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 06:35:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 06:35:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 06:36:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 06:36:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 06:36:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 07:24:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 21 Dec 2021 07:24:55 GMT
ENV PHP_VERSION=8.0.14
# Tue, 21 Dec 2021 07:24:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Tue, 21 Dec 2021 07:24:57 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Tue, 21 Dec 2021 07:25:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 07:25:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 07:40:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 07:40:31 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 21 Dec 2021 07:40:35 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 07:40:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 07:40:38 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 07:40:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 21 Dec 2021 07:40:45 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Dec 2021 07:40:46 GMT
EXPOSE 9000
# Tue, 21 Dec 2021 07:40:47 GMT
CMD ["php-fpm"]
# Wed, 22 Dec 2021 08:24:41 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 22 Dec 2021 08:24:43 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 22 Dec 2021 08:24:46 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 22 Dec 2021 08:24:47 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 22 Dec 2021 08:24:48 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 22 Dec 2021 08:24:49 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 22 Dec 2021 08:24:52 GMT
LABEL org.opencontainers.image.version=1.8.2
# Wed, 22 Dec 2021 08:25:33 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 22 Dec 2021 08:25:40 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Dec 2021 08:25:48 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 22 Dec 2021 08:25:49 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Wed, 22 Dec 2021 08:25:50 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Wed, 22 Dec 2021 08:25:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 08:25:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2031a2d9a9486eb693888310bd7c404b858eab6e58b93f9a67b0fa0ba0a076d`  
		Last Modified: Tue, 21 Dec 2021 09:23:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfef6776fce19b49c4cf70c3d6d31adf3afee6e19352646f3bc27655b8af9072`  
		Last Modified: Tue, 21 Dec 2021 09:23:43 GMT  
		Size: 86.6 MB (86624501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368374be7cc559a071ecd39ce723f773680ae0523d3213e72fef1d724547a300`  
		Last Modified: Tue, 21 Dec 2021 09:23:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db354b3dee3ac337e784ef142994f03cdbc133f4dca67aa0a0a230a02dc2c449`  
		Last Modified: Tue, 21 Dec 2021 09:29:50 GMT  
		Size: 11.2 MB (11178318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18455b317531c14ffc53a8729101bfec8f56ab6bacce5dda0b3bd4189478065`  
		Last Modified: Tue, 21 Dec 2021 09:29:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5507f30ce593020659afb756ab071170883f38c9ee1a386c9d3f29b22eac6af3`  
		Last Modified: Tue, 21 Dec 2021 09:30:59 GMT  
		Size: 31.1 MB (31071246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3fb132fe86091e260252858f08990f45fc9166bb183cc6d93f1c4ebf4b43e5`  
		Last Modified: Tue, 21 Dec 2021 09:30:53 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213893b77c6453ad816d9070333345829f34c3dae59440721ff8d95ac5e14118`  
		Last Modified: Tue, 21 Dec 2021 09:30:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d451ca1873944b291f2e9d302a2b60d8abd428b7ccc1488bfa452d5a2dfdd2`  
		Last Modified: Tue, 21 Dec 2021 09:30:54 GMT  
		Size: 8.6 KB (8576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a7d5ff2bba3ef199031f645f19b3b0768802c71617545657aa13edf07cc86a`  
		Last Modified: Wed, 22 Dec 2021 08:27:29 GMT  
		Size: 380.5 KB (380491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6cd52b7c77cfbf8d758b7ac78fedc572e0329e4035ff573f64cc8a08d9ee4d`  
		Last Modified: Wed, 22 Dec 2021 08:27:29 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb371e3d7f0022894a80322f85e5237c2d3fa1e93112699931a8aa76c166619`  
		Last Modified: Wed, 22 Dec 2021 08:27:29 GMT  
		Size: 2.6 MB (2574443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3336d2e9ed145a8f33af2abb92421ce5a34ff61068b7a3653390971e55dbdea`  
		Last Modified: Wed, 22 Dec 2021 08:27:29 GMT  
		Size: 2.0 KB (2044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae94a91740bb19df225c7a991526488eca3b0d7d68b5f14e62762da7d70c4a`  
		Last Modified: Wed, 22 Dec 2021 08:27:29 GMT  
		Size: 1.5 KB (1549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm` - linux; s390x

```console
$ docker pull yourls@sha256:75ab4f12f06f822e10412193b221daad7321c2aecf133e3d6388b70c589d4f4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143926594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ef78531eebcb9a915e47ed31a9ec65a6919edb6ef74ecfe7f4139501975077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:47:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 05:47:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 05:47:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:48:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 05:48:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 05:48:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 05:48:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 05:48:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 06:08:56 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 21 Dec 2021 06:08:56 GMT
ENV PHP_VERSION=8.0.14
# Tue, 21 Dec 2021 06:08:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.14.tar.xz.asc
# Tue, 21 Dec 2021 06:08:56 GMT
ENV PHP_SHA256=fbde8247ac200e4de73449d9fefc8b495d323b5be9c10cdb645fb431c91156e3
# Tue, 21 Dec 2021 06:09:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 06:09:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:15:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 06:15:49 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:15:50 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 06:15:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 06:15:50 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 06:15:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 21 Dec 2021 06:15:51 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Dec 2021 06:15:51 GMT
EXPOSE 9000
# Tue, 21 Dec 2021 06:15:51 GMT
CMD ["php-fpm"]
# Tue, 21 Dec 2021 18:21:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 21 Dec 2021 18:21:56 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 21 Dec 2021 18:21:56 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 21 Dec 2021 18:21:56 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 21 Dec 2021 18:21:56 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 21 Dec 2021 18:21:57 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 21 Dec 2021 18:21:57 GMT
LABEL org.opencontainers.image.version=1.8.2
# Tue, 21 Dec 2021 18:22:13 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 21 Dec 2021 18:22:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 21 Dec 2021 18:22:15 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 21 Dec 2021 18:22:16 GMT
COPY --chown=www-data:www-datafile:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Tue, 21 Dec 2021 18:22:16 GMT
COPY file:a47a395071c52d8d08402c95253924b09809713039b46033d6f6f75603938896 in /usr/local/bin/ 
# Tue, 21 Dec 2021 18:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 18:22:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea9906d585cce4773a1c39d603e30320e2ad3203d009914355e8008e64cb015`  
		Last Modified: Tue, 21 Dec 2021 07:08:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b426503ba635c77e4325d59b53584acc86bd622ffff9a713e34fbf79bd5f97c`  
		Last Modified: Tue, 21 Dec 2021 07:08:20 GMT  
		Size: 71.6 MB (71618295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf31efb9d4476e50c136ee15b83416dca20a8e68481bdb51ae28766a87ff4ff`  
		Last Modified: Tue, 21 Dec 2021 07:08:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4af35afd24e9b092e3734b88e5d445309695ba5af9397d5b9deb83946fd7d1`  
		Last Modified: Tue, 21 Dec 2021 07:11:52 GMT  
		Size: 11.2 MB (11176801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8b38f0b7ebc104cf44bd46e641c0357f444cdee084e055e67e45b59d4cb927`  
		Last Modified: Tue, 21 Dec 2021 07:11:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f2e39d408834ed550b8d0cbc0574eb57c849cbedf0093614ac7f77c80dc2d`  
		Last Modified: Tue, 21 Dec 2021 07:12:30 GMT  
		Size: 28.6 MB (28564665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ceefb31398014d695c79bed9623638347ae0ecd2082e0f1abacd898c18a724`  
		Last Modified: Tue, 21 Dec 2021 07:12:26 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95454e6a0969f6809a9e6c0f19c80fc6519ea8633bc3d253abda808d8278344b`  
		Last Modified: Tue, 21 Dec 2021 07:12:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abc06efe1335d421606ab453518ce2a45152f3872525932fe8d4c70a00bed2`  
		Last Modified: Tue, 21 Dec 2021 07:12:26 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78afd4ba792eacc3138b8d0412b3c86ed54eac689569a8692c6fef3a38b65b7`  
		Last Modified: Tue, 21 Dec 2021 18:23:27 GMT  
		Size: 334.7 KB (334716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9641e50057ce035b073bbd059f0515c489fa1af60a2b15561523f282cd7f65b6`  
		Last Modified: Tue, 21 Dec 2021 18:23:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f921995e75d8df1ef3411930485f2b4165539cbeb5a40b8be234da017643442`  
		Last Modified: Tue, 21 Dec 2021 18:23:27 GMT  
		Size: 2.6 MB (2574445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328197bc04fa990815d4740354a47f8d56743f62e697d5e3874a3186a6feb79`  
		Last Modified: Tue, 21 Dec 2021 18:23:27 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ba0007722d1f6d00107b7028c20d98ca5e6831289d70e6258cfce8c26cd1d`  
		Last Modified: Tue, 21 Dec 2021 18:23:27 GMT  
		Size: 1.5 KB (1549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
