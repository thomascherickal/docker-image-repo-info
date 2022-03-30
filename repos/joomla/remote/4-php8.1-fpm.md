## `joomla:4-php8.1-fpm`

```console
$ docker pull joomla@sha256:96821790ef91b20f407181f1b27e8397bdac98c06dcd0750de2162b2a8af7b6a
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

### `joomla:4-php8.1-fpm` - linux; amd64

```console
$ docker pull joomla@sha256:0e960c0d2075a237e618c57bacb957dd5a398162851cb070f36d90465db2d6d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186613567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9f4cd0c7cca63db0c6f22a206d0d3175c9440a82ee3f9c0616b9a7921423a5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:43:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 18:43:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 18:44:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:44:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 18:44:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 18:44:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 18:44:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 18:44:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 18:44:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 18:04:30 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 18:04:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 18:04:31 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 18:06:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 18:06:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:27:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 18:27:42 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:27:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 18:27:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 18:27:42 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 18:27:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 18:27:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 18:27:43 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 18:27:43 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 20:48:55 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 19 Mar 2022 20:48:55 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 19 Mar 2022 20:50:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:50:30 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 20:50:30 GMT
ENV JOOMLA_VERSION=4.1.0
# Sat, 19 Mar 2022 20:50:30 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sat, 19 Mar 2022 20:50:36 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 19 Mar 2022 20:50:36 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sat, 19 Mar 2022 20:50:37 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 19 Mar 2022 20:50:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 20:50:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15d475049bf47b33a15371e40ba8b1a4535451220b68578292b23738335498b`  
		Last Modified: Fri, 18 Mar 2022 04:51:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886e5161983fb82d6cbd0a8f7f8d0ebb90c72e349afbc290428b81bb572f0868`  
		Last Modified: Fri, 18 Mar 2022 04:52:08 GMT  
		Size: 91.6 MB (91604498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7666573a253171fcc168c406273e5843ae8aae6f251f8690878edfd3ec1b59`  
		Last Modified: Fri, 18 Mar 2022 04:51:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6aac8da418b607f749c51204330f4acfe721c3a4baac384681ca2d75c6fc45`  
		Last Modified: Fri, 18 Mar 2022 21:26:41 GMT  
		Size: 12.0 MB (12018669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b13992bc13bfb00101ff2a20bd91440a5304bef972c6150869327f2ed49c178`  
		Last Modified: Fri, 18 Mar 2022 21:26:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a732d119857825f9a2ad8037f9375808f034174647a551fc8daef4bf73046a13`  
		Last Modified: Fri, 18 Mar 2022 21:28:14 GMT  
		Size: 26.2 MB (26209119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589dc6ee39fef95efa4a9f588feaf72b6fcc0c54c9e9c38fc5d953fa482afb65`  
		Last Modified: Fri, 18 Mar 2022 21:28:09 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3ee85017e16012674a11ad277bf817153f00bbf2b293cd820bff559b57b6`  
		Last Modified: Fri, 18 Mar 2022 21:28:10 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fdd815d801fcc818e2584b40fe4f3d7f8c15a0e36d7ba8ba4da2c679114f47`  
		Last Modified: Fri, 18 Mar 2022 21:28:09 GMT  
		Size: 8.6 KB (8625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6e886a7597b9866566b1692f46dfa99b7c27fe1698cc04afcf5021e40987d`  
		Last Modified: Sat, 19 Mar 2022 21:05:44 GMT  
		Size: 3.1 MB (3104883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323aaf956e6a05b5364f1fd012c949e3d8832cfc71e212eac82a20ef96ad7890`  
		Last Modified: Sat, 19 Mar 2022 21:05:47 GMT  
		Size: 22.3 MB (22285219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c969c00bff3f48a7a5e16258318dfc14da702fe7108cbbaa8f661064f3e4f2a8`  
		Last Modified: Sat, 19 Mar 2022 21:05:43 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b9d1d0f5dc92fbb1fe1ec6e83ed86b145714a7c0497013c3b1a522c8c4c925`  
		Last Modified: Sat, 19 Mar 2022 21:05:43 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; arm variant v5

```console
$ docker pull joomla@sha256:db8ca5e59207143a8c444c3b18095c5cba25d78cfc54f5237f4d35a4cdd86ebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164613261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af92ef115f3f9895e168511fa0763558514f6bffddf7478bfa87d7fcdedb89e5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 19:50:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 19:50:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 19:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 19:51:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 19:51:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 19:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 19:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 19:52:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 19:52:02 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 17:16:09 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 17:16:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 17:16:10 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 17:17:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 17:17:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 17:33:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 17:33:23 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 17:33:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 17:33:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 17:33:25 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 17:33:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 17:33:27 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 17:33:28 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 17:33:28 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 03:45:14 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 19 Mar 2022 03:45:14 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 19 Mar 2022 03:50:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:50:10 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 03:50:10 GMT
ENV JOOMLA_VERSION=4.1.0
# Sat, 19 Mar 2022 03:50:10 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sat, 19 Mar 2022 03:50:28 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 19 Mar 2022 03:50:29 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sat, 19 Mar 2022 03:50:30 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 19 Mar 2022 03:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 03:50:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c11af9c0ad8de6675e4e7394b0f55d41135c1abfe801e8225a40b0ecc113be`  
		Last Modified: Fri, 18 Mar 2022 00:37:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5094249591f9019cf91d56b0a5b8378065e6c7b234d1ffa32516f92868978b1b`  
		Last Modified: Fri, 18 Mar 2022 00:38:25 GMT  
		Size: 73.7 MB (73684130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1181a1bb705d6f2d393bba06268fd7290eb1fb4d1f832b0f243ed30e57c842af`  
		Last Modified: Fri, 18 Mar 2022 00:37:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f963a3733c0918a5436c16d3d9c4f4433160f890fd3bd0d1cf945557f3240d4d`  
		Last Modified: Fri, 18 Mar 2022 19:20:58 GMT  
		Size: 12.0 MB (12017261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01de9786057f210d0058e21f18f896413988f071d98ec80f229dbc92c74b7ce6`  
		Last Modified: Fri, 18 Mar 2022 19:20:55 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f66ab101f6a79a424671a7014a2a6dafa8e024227354e5ea820cc248396db7`  
		Last Modified: Fri, 18 Mar 2022 19:23:22 GMT  
		Size: 24.8 MB (24795649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65010ad2f25c0c99953f5a30a796489b0844dbbb75918971536ec291765e424d`  
		Last Modified: Fri, 18 Mar 2022 19:23:12 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78aa4956971914ef454f43f9b4e144f394cb52ab2f5c096cd0e5323aaafeae2`  
		Last Modified: Fri, 18 Mar 2022 19:23:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737ae91c07eff41a0e83551af2d585435124c3f56cd300cff4242cb460a772b1`  
		Last Modified: Fri, 18 Mar 2022 19:23:12 GMT  
		Size: 8.6 KB (8625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff75de026fb06dae59fa4f8aaa83de08a4e59bf92d23b705735ef4ec97458c5`  
		Last Modified: Sat, 19 Mar 2022 03:58:41 GMT  
		Size: 2.9 MB (2896680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815075f622bfb0b427b4e2a47462f3155eb4cced9480867796f481bef75ec1ad`  
		Last Modified: Sat, 19 Mar 2022 03:58:59 GMT  
		Size: 22.3 MB (22285229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02b3961cc8367822637e5e627d0ae6e5cf39030a8be5599b32aae0a97c86a4`  
		Last Modified: Sat, 19 Mar 2022 03:58:39 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17800f0d3ea28e69f34e5a2a0e1270c3255872a828671bffd20f55de42737781`  
		Last Modified: Sat, 19 Mar 2022 03:58:40 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; arm variant v7

```console
$ docker pull joomla@sha256:5edcc746e6e8e26882f6abac0bca5309584316f4f9ca4836168146e6ee0b17ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (156968320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56cf5aa13b51900cfb0d02423087facdb281f1fd307e566c9ac38f2d1e5126e0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 06:49:01 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 06:49:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 06:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 06:49:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 06:49:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 06:49:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:49:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:49:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 06:49:51 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 06:49:51 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 06:49:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 06:49:52 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 06:50:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 06:50:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:05:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 07:05:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:05:10 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 07:05:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 07:05:11 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 07:05:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 07:05:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 07:05:14 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 07:05:14 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 15:58:18 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 29 Mar 2022 15:58:19 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 29 Mar 2022 16:02:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 16:02:55 GMT
VOLUME [/var/www/html]
# Tue, 29 Mar 2022 16:02:55 GMT
ENV JOOMLA_VERSION=4.1.0
# Tue, 29 Mar 2022 16:02:56 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Tue, 29 Mar 2022 16:03:14 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 29 Mar 2022 16:03:15 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 29 Mar 2022 16:03:16 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 29 Mar 2022 16:03:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 16:03:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf6ea3410c58e5dfb18a8d11ed37871fc3403ec1f9d63969c1410dc411fc9e`  
		Last Modified: Tue, 29 Mar 2022 10:29:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd96359d7acc6ffe17c6e8a0a4de1c02c133875cb011c7a24fe9ad218b54a4`  
		Last Modified: Tue, 29 Mar 2022 10:29:38 GMT  
		Size: 69.3 MB (69315695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627cc4eef368ed04b244a169bebdfcf487fab6d4e2eac809d7afb34311391e`  
		Last Modified: Tue, 29 Mar 2022 10:29:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf9d25a616dfb5938b4217af347215ecfaf820f2c0b2e7fefee97e553ed94df`  
		Last Modified: Tue, 29 Mar 2022 10:29:11 GMT  
		Size: 12.0 MB (12017311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638340666488e0d7e59016650d0e865095a091012bb2f0eeb91507451e567d31`  
		Last Modified: Tue, 29 Mar 2022 10:29:08 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f39ea1f7cf7e7b9e4705ad6a133384403376f9b20a5b7b38097aaac3724c60d`  
		Last Modified: Tue, 29 Mar 2022 10:31:55 GMT  
		Size: 24.0 MB (23971155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e7d67a2951ebe846271e4d180849c45e26baea6d431608026653b521e993cd`  
		Last Modified: Tue, 29 Mar 2022 10:31:46 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2267b7813e8d3f2f8317c3bb11c21665cec2ed1efe43828c44ac155a0a40e70e`  
		Last Modified: Tue, 29 Mar 2022 10:31:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb14e6288418e8d13cbd0428cf172e065077284a00716fd129315d282eb7eda`  
		Last Modified: Tue, 29 Mar 2022 10:31:46 GMT  
		Size: 8.6 KB (8622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646bf2426019b3c69c422145d22fa6bd25f8b453039c0c3479749ece1383c6e`  
		Last Modified: Tue, 29 Mar 2022 16:30:06 GMT  
		Size: 2.8 MB (2788825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e1ba6cbd229b739018842beb0abb93d382b38ccb30dcb6577eeed804afa3f2`  
		Last Modified: Tue, 29 Mar 2022 16:30:24 GMT  
		Size: 22.3 MB (22285215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7300916ae7195a4278ec59925eb24b4fd603675d493a084c9a6e2c6e8050319`  
		Last Modified: Tue, 29 Mar 2022 16:30:04 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1446b0ccd1508a4e0c42cf55de2735a1aa61ac744deb532845921952f0d5eaba`  
		Last Modified: Tue, 29 Mar 2022 16:30:04 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:a972f838aa1236c34d22a0ab362109616198540903419456623f53fdf9c9f19d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.8 MB (179750929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8eef6fc13a5cdb9303c649de20a204b4570ea3444eca9344d6e6973fb5c2daf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:04:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 14:04:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 14:04:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:04:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 14:04:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 14:04:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:04:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:04:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 14:04:45 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 18:09:49 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 18:09:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 18:09:51 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 18:11:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 18:11:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:24:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 18:24:24 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:24:24 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 18:24:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 18:24:26 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 18:24:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 18:24:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 18:24:29 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 18:24:30 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 20:04:40 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 19 Mar 2022 20:04:41 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 19 Mar 2022 20:06:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:06:24 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 20:06:25 GMT
ENV JOOMLA_VERSION=4.1.0
# Sat, 19 Mar 2022 20:06:26 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sat, 19 Mar 2022 20:06:33 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 19 Mar 2022 20:06:35 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sat, 19 Mar 2022 20:06:36 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 19 Mar 2022 20:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 20:06:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d64b996e3c6964119d9bc453f2742cab32b669682d1b31d83869f5bc77a1ee`  
		Last Modified: Thu, 17 Mar 2022 18:13:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e8603cc40c823959e187209a2b13be43a13f53851c445c5abc3b2ea00dfd37`  
		Last Modified: Thu, 17 Mar 2022 18:13:50 GMT  
		Size: 86.7 MB (86717067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48bd64469431f94558573227bbc1cb74193277b2fb5c35d1e1122590466b94`  
		Last Modified: Thu, 17 Mar 2022 18:13:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad3ec980781aea7d8aabb53f2db5e172dca38f1b8256fc5ab95452fe37157b`  
		Last Modified: Fri, 18 Mar 2022 20:28:47 GMT  
		Size: 11.8 MB (11803111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62c65179f67e5d63e69e1e688b0fce29df928b9710d00f1551f04d5800aecd5`  
		Last Modified: Fri, 18 Mar 2022 20:28:46 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187ee02c31a7218b2776f476380d9cbb9350b04bd670a816746fb4eb9161721a`  
		Last Modified: Fri, 18 Mar 2022 20:30:33 GMT  
		Size: 26.0 MB (26034018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4de152608ac57f15b68d071dc9f04fe4a579041a97a5c278a3d04c77f94db4`  
		Last Modified: Fri, 18 Mar 2022 20:30:29 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce66f1114cdbdebcd65a35e6d84dc4f4d5ceb7ffacc72d4735b1041a11364d47`  
		Last Modified: Fri, 18 Mar 2022 20:30:29 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd34caa6608c99b6387158eb2640226b68339c783cd82c37e2beec12cdb02e`  
		Last Modified: Fri, 18 Mar 2022 20:30:28 GMT  
		Size: 8.6 KB (8625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbaaa2277f7796a21acd96e08c73ddaa75450c203390557b03484885c5e695`  
		Last Modified: Sat, 19 Mar 2022 20:12:21 GMT  
		Size: 2.8 MB (2836802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcea4448bcaa945d53c7ed5a45da38c5834419429f17c453f868b13fee502ed`  
		Last Modified: Sat, 19 Mar 2022 20:12:24 GMT  
		Size: 22.3 MB (22282361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e814f3c8d0c321f39d9a6fa85985ec8ae35e48d75aa30a51cec2197148d3acd`  
		Last Modified: Sat, 19 Mar 2022 20:12:20 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1a6acf8d663cce3a17cde5a94b5ace12abebbe592ef3ec319bb231204402c`  
		Last Modified: Sat, 19 Mar 2022 20:12:20 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; 386

```console
$ docker pull joomla@sha256:b1d9d0d09b3b71ff0c987ed0cc005b66683e409fe9691f851b15dff526b3adc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.4 MB (188375338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e739b3a2af8c27b9fd33f3bb0e11f25095b02efbe574bc44bd8d5ece37e963f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:13:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:13:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:14:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:14:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:14:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:14:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:14:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 01:14:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 01:14:11 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 01:14:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 01:14:13 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 01:14:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 01:14:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:23:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 01:23:48 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:23:48 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 01:23:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 01:23:50 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 01:23:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 01:23:52 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 01:23:53 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 01:23:54 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 21:10:19 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 29 Mar 2022 21:10:19 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 29 Mar 2022 21:11:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 21:11:44 GMT
VOLUME [/var/www/html]
# Tue, 29 Mar 2022 21:11:45 GMT
ENV JOOMLA_VERSION=4.1.0
# Tue, 29 Mar 2022 21:11:46 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Tue, 29 Mar 2022 21:11:55 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 29 Mar 2022 21:11:56 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 29 Mar 2022 21:11:57 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 29 Mar 2022 21:11:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 21:11:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5eef24434e26d7c7efe110e0a514725a245f4a80feef19fde4adf2881c842c6`  
		Last Modified: Tue, 29 Mar 2022 03:19:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce29d62a2961a018f305c25e5e41d731c9c0f7ef22ee18a11b27b83c635fd5e`  
		Last Modified: Tue, 29 Mar 2022 03:19:36 GMT  
		Size: 92.5 MB (92510998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a5747ae4f3b12af8c59a4f80eab5e5e8dfd15b8f67d7364e1c226edd82eef1`  
		Last Modified: Tue, 29 Mar 2022 03:19:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712503f5bb243556eeceae55cf0a269d03f4f67ca2afe81a0347015db0ec5a1d`  
		Last Modified: Tue, 29 Mar 2022 03:19:21 GMT  
		Size: 11.8 MB (11803041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f46b3cd6be93c30f4113b7130515ea808c712aadfad907335e5024ca6f55215`  
		Last Modified: Tue, 29 Mar 2022 03:19:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbc89ae17ada18ff5aacbe6b24fd945cd1f593e71137447ee1e9b2fa68fe7fc`  
		Last Modified: Tue, 29 Mar 2022 03:21:20 GMT  
		Size: 26.5 MB (26467279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d851f5ea906c324facc745901e6797c79b1802c5151a98c734f385ef1ad3dd1`  
		Last Modified: Tue, 29 Mar 2022 03:21:15 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca10fb8af7cd9c52b701a8b984cc2ef1e3c0c151281337b27d6bd438acdb15b`  
		Last Modified: Tue, 29 Mar 2022 03:21:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a509bfc38089080c45bf703e53641523c100a1b0b806e13a874d7060bb484`  
		Last Modified: Tue, 29 Mar 2022 03:21:15 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c509409a44724852f910f95ad59c1b4e885477bc54978432e91512fd9e35787`  
		Last Modified: Tue, 29 Mar 2022 21:26:19 GMT  
		Size: 2.9 MB (2907448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9507250c667d705ed5d8fd312e288a7b89f043690241ebea774d62403fdd5b5`  
		Last Modified: Tue, 29 Mar 2022 21:26:21 GMT  
		Size: 22.3 MB (22282355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd608889e9a01d7b4cd25b01dcc331041bf0af913e743dbd7c778ef5a3f2550`  
		Last Modified: Tue, 29 Mar 2022 21:26:18 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe130bb5e0578e5585c519410ffe1ac9df925b01cced95b9173aecf05134b89`  
		Last Modified: Tue, 29 Mar 2022 21:26:18 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; mips64le

```console
$ docker pull joomla@sha256:9e61a5137fb00a509acb5ed0a98b6f8e497691bd5ab46d2c1745d6f43240d1e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163561497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a865867f3df8f2b3bcb6c7a84af098369cbab7fd7a33cd5780dc30553a379cdf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:16:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 18 Mar 2022 06:17:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 18 Mar 2022 06:18:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:18:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 18 Mar 2022 06:18:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 18 Mar 2022 06:18:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 06:18:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 06:18:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 06:19:00 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 06:19:03 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 06:19:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 06:19:10 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 06:20:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 06:20:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 07:02:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 00:16:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:16:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 00:16:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 00:16:22 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 00:16:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 00:16:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 00:16:35 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 00:16:39 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 04:05:39 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 29 Mar 2022 04:05:43 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 29 Mar 2022 04:11:58 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 04:12:01 GMT
VOLUME [/var/www/html]
# Tue, 29 Mar 2022 04:12:05 GMT
ENV JOOMLA_VERSION=4.1.0
# Tue, 29 Mar 2022 04:12:09 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Tue, 29 Mar 2022 04:12:43 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 29 Mar 2022 04:12:50 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 29 Mar 2022 04:12:55 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 29 Mar 2022 04:13:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 04:13:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc1457b77be2adf18a1b54e0a14aca031d2ca8f67f12b5a5f621a691bd28a48`  
		Last Modified: Fri, 18 Mar 2022 13:01:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439a25f7277d525bf09c81bf79c6230e999388eb18ee325f13ec03e912e33789`  
		Last Modified: Fri, 18 Mar 2022 13:02:07 GMT  
		Size: 71.8 MB (71809995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e4e0d8140ff896ecf0e5ad80965738e6651592aacddfc506e8aa8ecdb80db`  
		Last Modified: Fri, 18 Mar 2022 13:01:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232c96810755fc6d4ef5a043e40542fff4fbd73ce5566a140191b6c39f0f2c88`  
		Last Modified: Fri, 18 Mar 2022 13:01:16 GMT  
		Size: 11.8 MB (11801928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b814a977c6e7da947bb51456d5f6c7bfa009aedab5777bc6f631eb44e88111b`  
		Last Modified: Fri, 18 Mar 2022 13:01:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0871c2127eda6eca23303e59f6fd9fc9130c126f5b93888591b87ca0c7b8395d`  
		Last Modified: Fri, 18 Mar 2022 13:03:59 GMT  
		Size: 25.2 MB (25209719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a3bb283703b2b0392b8b9688550b34d5e577dde20afcc21380276906c9b15e`  
		Last Modified: Tue, 29 Mar 2022 00:30:13 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecff04ac9a8e384c4a3c5b767a8ce4b90d5ab6b18e525edff1fcd87a9b9751`  
		Last Modified: Tue, 29 Mar 2022 00:30:13 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcaff4954792c38000d9aa21ccc124c06cb02f339dea7e2286be0d1ae6e980c`  
		Last Modified: Tue, 29 Mar 2022 00:30:13 GMT  
		Size: 8.6 KB (8629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf544b206d0d9dc66e3d8b5765665fc77a3662c4cfc2c316cde448d29861d9c4`  
		Last Modified: Tue, 29 Mar 2022 04:30:47 GMT  
		Size: 2.8 MB (2802964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3767130cc883be28488c4659e8808c46d7f4dfb06eea6f600209399606f21ec`  
		Last Modified: Tue, 29 Mar 2022 04:31:01 GMT  
		Size: 22.3 MB (22282361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db4c19f1354d0ac16d4ff7d7221016be89dd8e21f814a65b29aa426dcd0665b`  
		Last Modified: Tue, 29 Mar 2022 04:30:44 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d944f3717019b45a3eaefe8fff0e61ec299048bb367587539ef476afff194ab1`  
		Last Modified: Tue, 29 Mar 2022 04:30:44 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; ppc64le

```console
$ docker pull joomla@sha256:423019bdf31e177df57e138ebec1911c3f3f2235777a8ea6cff0fb04f42c0697
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.8 MB (186767489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5045b2d89a53fb601fbecc24630796f599bc8f086120cc951cc1e189b6f57b3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 12:18:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 18 Mar 2022 12:18:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 18 Mar 2022 12:22:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 12:22:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 18 Mar 2022 12:23:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 18 Mar 2022 12:23:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 12:23:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 12:23:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 12:23:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 12:23:19 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 12:23:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 12:23:30 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 12:27:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 12:27:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:54:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 12:54:32 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:54:57 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 12:55:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 12:55:22 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 12:55:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 12:55:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 12:55:48 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 12:55:53 GMT
CMD ["php-fpm"]
# Sun, 20 Mar 2022 06:42:08 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sun, 20 Mar 2022 06:42:12 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sun, 20 Mar 2022 06:45:19 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:45:22 GMT
VOLUME [/var/www/html]
# Sun, 20 Mar 2022 06:45:27 GMT
ENV JOOMLA_VERSION=4.1.0
# Sun, 20 Mar 2022 06:45:31 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sun, 20 Mar 2022 06:45:54 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sun, 20 Mar 2022 06:45:58 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sun, 20 Mar 2022 06:46:01 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sun, 20 Mar 2022 06:46:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 06:46:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6484537d5ef744c30a9a64b7d2e56c6987ee873a38ba58f4e3f0949ddc170c2`  
		Last Modified: Fri, 18 Mar 2022 19:03:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac141ab24880de35152b298b83829f9359dfd5800a7b6bc7cb8933d21604700`  
		Last Modified: Fri, 18 Mar 2022 19:04:28 GMT  
		Size: 86.6 MB (86625475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8daf14d12dc3fc9b0e0c873d5d85da826a3b0278600f5f2d702a6208d715d6`  
		Last Modified: Fri, 18 Mar 2022 19:03:30 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588e134d013f15a93f8d505cd0c60460c9479fa93ce8e085f5f8076592d449b`  
		Last Modified: Fri, 18 Mar 2022 19:03:29 GMT  
		Size: 12.0 MB (12019110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bd3f243440959e5d4ef73867b2d6ead3d4f7ee061ba0e3663564a669d84e9`  
		Last Modified: Fri, 18 Mar 2022 19:03:27 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ca177e6a810f06aaf2da6ecd5fd5bdbe808fe34e64ed652d127fb6c009a28d`  
		Last Modified: Fri, 18 Mar 2022 19:07:08 GMT  
		Size: 27.2 MB (27231853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7d04377f39c812b64aee64cee0527764733bdf6041c2a43a09e03923e30b8`  
		Last Modified: Fri, 18 Mar 2022 19:06:46 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c5a90b8471da19c77f2be331c2b60cc2e039d2d413b85b73ba4621bb99426c`  
		Last Modified: Fri, 18 Mar 2022 19:06:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61941c89d1e780c23b8e48276d242334ee13a706712006a0042b1239ea29211`  
		Last Modified: Fri, 18 Mar 2022 19:06:46 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd2f0fc78e78d3dcb8a15a6e932cbfd349b6b4b66ce2afcd2fd001bee432879`  
		Last Modified: Sun, 20 Mar 2022 09:00:11 GMT  
		Size: 3.3 MB (3311479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c091758ac06b072550d166304bf4c831aa2bf50e6d969b2c3faf913a6182a87d`  
		Last Modified: Sun, 20 Mar 2022 09:00:14 GMT  
		Size: 22.3 MB (22285204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8beef2d4e2b3278ff7ce898aaa8cd7aa761538274b2be9532b14b13edd9d68fe`  
		Last Modified: Sun, 20 Mar 2022 09:00:10 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a695077a8e98fddd80e67fc75002c516a8ba560b6b7088c62870b370df46405`  
		Last Modified: Sun, 20 Mar 2022 09:00:10 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; s390x

```console
$ docker pull joomla@sha256:6cf127a6ecf0c9df271643b9ae701b52c2a09046ebfe1d49741af4a9f321fab8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.9 MB (163912339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5649aad42a268b34be54473e097364a48d4e7f16cba9937bb93c8ba3e939dff0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:57:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 08:57:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 08:57:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 08:57:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 08:57:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 08:57:28 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 05:44:19 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 05:44:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 05:44:19 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 05:46:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 05:46:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 05:54:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 05:54:17 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 05:54:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 05:54:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 05:54:18 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 05:54:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 05:54:19 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 05:54:19 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 05:54:20 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 01:15:23 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 19 Mar 2022 01:15:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 19 Mar 2022 01:16:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 01:16:25 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 01:16:25 GMT
ENV JOOMLA_VERSION=4.1.0
# Sat, 19 Mar 2022 01:16:26 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sat, 19 Mar 2022 01:16:34 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 19 Mar 2022 01:16:37 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sat, 19 Mar 2022 01:16:37 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 19 Mar 2022 01:16:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 01:16:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a168516a7b34ac78c5562407bc73cdbb0b67b5411f6cb3fde601c7d8859b891c`  
		Last Modified: Thu, 17 Mar 2022 11:54:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863e90272897da73827b4ced7f99c3ebee930f3316ca88d0c8e1b0ad60132cd0`  
		Last Modified: Thu, 17 Mar 2022 11:54:55 GMT  
		Size: 71.6 MB (71617741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ac7f51cfa884bfe88ce25e7756dd4c49de4125cad58ced6332dc8a5690707`  
		Last Modified: Thu, 17 Mar 2022 11:54:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54fa669140fef898758e2fd54be815bcaadf6eb1239b30cf4a853b9e2b37cd3`  
		Last Modified: Fri, 18 Mar 2022 07:28:12 GMT  
		Size: 12.0 MB (12017525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e039646f8841f710e9097da7f7d2ad511e389736020c3b06b7ba0b7beb344a`  
		Last Modified: Fri, 18 Mar 2022 07:28:11 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80157286b843658866c276c3abd4a2d08e5f21cd1b03afb821b474a71cee6d96`  
		Last Modified: Fri, 18 Mar 2022 07:29:11 GMT  
		Size: 25.3 MB (25267453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08768888b411753a350e4a317544679c9790d5b7f2d3d801a85d6376a42449e`  
		Last Modified: Fri, 18 Mar 2022 07:29:07 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f69955448211234eb3df4f17a381a651e575fbbf90ba2e4ca43041b28d0c0f`  
		Last Modified: Fri, 18 Mar 2022 07:29:07 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a366ed0cc65a8b96f4bdda44656e9bb84a91ec8b7eea33bb3db7bcd30e72ca53`  
		Last Modified: Fri, 18 Mar 2022 07:29:07 GMT  
		Size: 8.6 KB (8625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fc5acd29a45f1e4fc72a5c36ca90f24665736656fb716939817bc9009ea698`  
		Last Modified: Sat, 19 Mar 2022 01:22:18 GMT  
		Size: 3.1 MB (3054021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319bf00dae911e247260f66f78140468f3f3e1c4665e6fbb8a07866cffaddaf`  
		Last Modified: Sat, 19 Mar 2022 01:22:21 GMT  
		Size: 22.3 MB (22285197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e59ecb899aa6add0ca9add37338ec2a6111576e1ab854460378a436ec0edfe6`  
		Last Modified: Sat, 19 Mar 2022 01:22:17 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307c8ac688cd811d72d3608f5467aa0d834a60e9a2c5b97939e26dfebb72e2a5`  
		Last Modified: Sat, 19 Mar 2022 01:22:17 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
