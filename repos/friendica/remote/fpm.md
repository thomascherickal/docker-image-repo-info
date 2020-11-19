## `friendica:fpm`

```console
$ docker pull friendica@sha256:5ca1609bf64ab9fd891a74c219b99543d84f9bed73c4da1b1356c79bcb386b7d
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

### `friendica:fpm` - linux; amd64

```console
$ docker pull friendica@sha256:b01a4a14e05a9799b540c26c5697f93752947d15eafc85301633f37281ab2158
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227045888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10eda1c8ea871358e022a4c077f512dedeb5151a6eea1ebe25b84580b56dbb26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 08:44:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 08:44:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 08:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 08:44:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 08:44:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 09:02:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 09:02:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 09:02:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 09:02:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 10:07:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 18 Nov 2020 10:07:33 GMT
ENV PHP_VERSION=7.3.24
# Wed, 18 Nov 2020 10:07:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Wed, 18 Nov 2020 10:07:34 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Wed, 18 Nov 2020 10:07:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 10:07:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 10:15:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 10:15:44 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 10:15:46 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 10:15:48 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 18 Nov 2020 10:15:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 10:15:48 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 10:15:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 10:15:50 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 10:15:51 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 10:15:51 GMT
CMD ["php-fpm"]
# Thu, 19 Nov 2020 04:09:01 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Thu, 19 Nov 2020 04:09:01 GMT
ENV TINI_VERSION=v0.19.0
# Thu, 19 Nov 2020 04:09:02 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Thu, 19 Nov 2020 04:11:10 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 04:11:11 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 19 Nov 2020 04:11:11 GMT
VOLUME [/var/www/html]
# Thu, 19 Nov 2020 04:11:12 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Thu, 19 Nov 2020 04:11:12 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Thu, 19 Nov 2020 04:11:20 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 19 Nov 2020 04:11:21 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Thu, 19 Nov 2020 04:11:22 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Thu, 19 Nov 2020 04:11:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 04:11:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266fc315b0155934606f2688364a42d4233b2a7605f51f06d6aced8c88fe2e6`  
		Last Modified: Wed, 18 Nov 2020 12:03:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8a5fa787a1ee6c4cb42f9b382aacfeb33d97504cbd3d35e23727bab752e5cd`  
		Last Modified: Wed, 18 Nov 2020 12:04:07 GMT  
		Size: 76.7 MB (76652404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc127c18841756f8fef538b2136f8b2c1c90b972c621e0f7885f7fbc7a15cb`  
		Last Modified: Wed, 18 Nov 2020 12:03:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550f3756f9dd967296322022bbc87f938f3ce28df5bec4d7cb3a70f5199b87`  
		Last Modified: Wed, 18 Nov 2020 12:07:51 GMT  
		Size: 12.5 MB (12459899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ef67933ae1388e6c51f495e46278dec6fb7e1e96e265f39761fad293c1fc4e`  
		Last Modified: Wed, 18 Nov 2020 12:07:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb2ed47d336c8f58445e68a646bc723a4f66e762d06576122e77fda47622f6d`  
		Last Modified: Wed, 18 Nov 2020 12:07:54 GMT  
		Size: 28.8 MB (28767218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9676ab4ad6f0aaa2ca0d808d54d45cc65ddfa2da76e030727f912a1e70102730`  
		Last Modified: Wed, 18 Nov 2020 12:07:49 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d17455cee2ea0f01a124b36d37db438545ee0678be512860b6fb362e2a1d8e4`  
		Last Modified: Wed, 18 Nov 2020 12:07:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12355146902bd3190b4bef14aa0b479a874c026be0895f2a36afbd7ca11729ed`  
		Last Modified: Wed, 18 Nov 2020 12:07:49 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e74987d1e0293f2ae6892c4574ee8616809a8a6a0c7a911b13267c0d0c7fc4`  
		Last Modified: Wed, 18 Nov 2020 12:07:49 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaf63c554482294443cf083770872fb5504ce3e8b56093cfcaf4306f063b48a`  
		Last Modified: Thu, 19 Nov 2020 04:12:31 GMT  
		Size: 19.1 MB (19101203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60f6e49c899313de5dd3d5aa85c661d08c38d9c2c2d0cc7b4e08953b93d4243`  
		Last Modified: Thu, 19 Nov 2020 04:12:27 GMT  
		Size: 16.1 KB (16095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0838be56b1a5b656aeb59483f5b008e572f2f14359a5867a6227c436c33aae3`  
		Last Modified: Thu, 19 Nov 2020 04:12:30 GMT  
		Size: 15.2 MB (15241092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7520fa9acd522f64f5f07e2e9e1401162ff923c5bd7ef15e0ea9bb482e8e3a8c`  
		Last Modified: Thu, 19 Nov 2020 04:12:25 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364ab105f82c2036b891ee157eb74540b400cc7318dcb3517bc9aa2925b3710e`  
		Last Modified: Thu, 19 Nov 2020 04:12:34 GMT  
		Size: 47.7 MB (47686181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a10ec83f6cff9e5441221674168a41fd8c72055a1bd3036f907e8eed9ba53`  
		Last Modified: Thu, 19 Nov 2020 04:12:26 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb240b29c13dc85b958eed5de67a5ad2f009296d75bf309ad25d1c3fc17ed74`  
		Last Modified: Thu, 19 Nov 2020 04:12:26 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm variant v5

```console
$ docker pull friendica@sha256:504e2ed8122f9b125fcee77876ee0e387c67a765c2618de025c2045dc75b2c5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.9 MB (202945042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:619dc6f7fcd279b15726643ae008e804288e018aa9bb99b15bf0b845da66151e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:21:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 04:21:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 04:21:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 04:21:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 04:21:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 04:30:49 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 04:30:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:30:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:30:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 05:03:57 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 29 Oct 2020 22:34:03 GMT
ENV PHP_VERSION=7.3.24
# Thu, 29 Oct 2020 22:34:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Thu, 05 Nov 2020 19:51:32 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Thu, 05 Nov 2020 19:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 19:51:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:56:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 19:56:04 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:56:08 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 19:56:11 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 05 Nov 2020 19:56:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 19:56:13 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 19:56:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 19:56:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 19:56:18 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 19:56:19 GMT
CMD ["php-fpm"]
# Thu, 05 Nov 2020 21:35:52 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Thu, 05 Nov 2020 21:35:53 GMT
ENV TINI_VERSION=v0.19.0
# Thu, 05 Nov 2020 21:35:57 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Thu, 05 Nov 2020 21:41:12 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 05 Nov 2020 21:41:20 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 05 Nov 2020 21:41:23 GMT
VOLUME [/var/www/html]
# Thu, 05 Nov 2020 21:41:26 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Thu, 05 Nov 2020 21:41:30 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Thu, 05 Nov 2020 21:41:56 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 05 Nov 2020 21:41:59 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Thu, 05 Nov 2020 21:42:00 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Thu, 05 Nov 2020 21:42:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 05 Nov 2020 21:42:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5544e1e4c59070ffab6bb67438e06cb51e70ef8edc65047cea48fd2ab8bdb0ea`  
		Last Modified: Tue, 13 Oct 2020 06:07:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca39c077cee68edc8bd24950274f31e7e0e35f4f1d4189e1bf2ef8ec7e3d9edd`  
		Last Modified: Tue, 13 Oct 2020 06:07:28 GMT  
		Size: 58.8 MB (58801053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b23e07d9f8d59f1c6d41ceb0c2708766c400c69bde2c74dc2877152fd7f045`  
		Last Modified: Tue, 13 Oct 2020 06:07:07 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239cd43c4a7a2474285169ebb16e2f2077c0728fc243ed6c6d79987cbf93ea2`  
		Last Modified: Thu, 05 Nov 2020 21:02:55 GMT  
		Size: 12.5 MB (12458122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91e2dc0810024b5f20bc20eb936a1e36cd95b3201a144bb701da48ca3dd65f0`  
		Last Modified: Thu, 05 Nov 2020 21:02:53 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa45bacbe963734038dc5d1695f5c8bb7f6217569a355e10573a8a671e6aafb`  
		Last Modified: Thu, 05 Nov 2020 21:03:00 GMT  
		Size: 27.3 MB (27317401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b28bd7889c464449afe456216e76c1710095aa6a2f3b22da35337b6a26f23a`  
		Last Modified: Thu, 05 Nov 2020 21:02:51 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e364c6b16a6ad9efefff674882faf3364cc249e5c8b330ace51208fa086d682`  
		Last Modified: Thu, 05 Nov 2020 21:02:52 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce584c4d2d7fbd798c99ebfadd2206c5ffa3cdfd122abe552acd3e6f66d4a3`  
		Last Modified: Thu, 05 Nov 2020 21:02:52 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979eb99834c1b76ac0daf30be9564bc32e5c96e89782e21afd8a4790cbb42c60`  
		Last Modified: Thu, 05 Nov 2020 21:02:52 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef56b8477de29763b8eb6476ca85a4013081d734822314084a561beb24ecf428`  
		Last Modified: Thu, 05 Nov 2020 21:43:52 GMT  
		Size: 17.8 MB (17789437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63c13919ad875120e842bf427f0599dbb6f849b45d56c383f45732f1b6c3a12`  
		Last Modified: Thu, 05 Nov 2020 21:43:47 GMT  
		Size: 15.5 KB (15521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0cb2775e0d171d86bdc42f9d007e9c10784f051892ac3983e0fa28bd341fda`  
		Last Modified: Thu, 05 Nov 2020 21:43:49 GMT  
		Size: 14.0 MB (14024940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d7bf3abfa03bdff542f2608c8c62f142c9f0c43a6b882547b2719b69be7a75`  
		Last Modified: Thu, 05 Nov 2020 21:43:45 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c251f9490ca00a600b61f96b28dfe2615a49ae9317b3fc425de3099a7a48ada4`  
		Last Modified: Thu, 05 Nov 2020 21:43:59 GMT  
		Size: 47.7 MB (47686177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a02d435a903524256bdac06a1497f3f29b166a89dab086afdc955ca524464b`  
		Last Modified: Thu, 05 Nov 2020 21:43:45 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6338e5abc3ff3dbba61437f7266544b5e802784d25cd1715dfba32b0fdb2302`  
		Last Modified: Thu, 05 Nov 2020 21:43:45 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm variant v7

```console
$ docker pull friendica@sha256:54a6e74629dc5ee818a6b612bd55ab32ec018d36009c0d47942fc480ff7efefc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197626447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4760cc0b009de97dc2572f458024548fe70d4682d2cc5b7dd9122f03f57650`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:47:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Nov 2020 23:47:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Nov 2020 23:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 23:48:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Nov 2020 23:48:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Nov 2020 23:56:13 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 17 Nov 2020 23:56:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 23:56:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 23:56:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 00:26:34 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 18 Nov 2020 00:26:35 GMT
ENV PHP_VERSION=7.3.24
# Wed, 18 Nov 2020 00:26:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Wed, 18 Nov 2020 00:26:38 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Wed, 18 Nov 2020 00:27:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 00:27:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 00:30:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 00:30:04 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 00:30:07 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 00:30:09 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 18 Nov 2020 00:30:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 00:30:11 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 00:30:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 00:30:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 00:30:17 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 00:30:18 GMT
CMD ["php-fpm"]
# Wed, 18 Nov 2020 20:16:48 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Wed, 18 Nov 2020 20:16:49 GMT
ENV TINI_VERSION=v0.19.0
# Wed, 18 Nov 2020 20:16:51 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Wed, 18 Nov 2020 20:21:10 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 20:21:13 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 18 Nov 2020 20:21:14 GMT
VOLUME [/var/www/html]
# Wed, 18 Nov 2020 20:21:15 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Wed, 18 Nov 2020 20:21:16 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Wed, 18 Nov 2020 20:22:56 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Wed, 18 Nov 2020 20:23:01 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Wed, 18 Nov 2020 20:23:03 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Wed, 18 Nov 2020 20:23:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 20:23:05 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531bbb917fccba63f54fa698cfc54068c09767ead93fc6e6644347dd27b257a3`  
		Last Modified: Wed, 18 Nov 2020 01:34:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5e8740a1696bf1e23f4e8db4ddeeefdc469ea5cbc5030b4b966a023c71c05`  
		Last Modified: Wed, 18 Nov 2020 01:34:34 GMT  
		Size: 59.5 MB (59507784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea34a36e19ecf6fc3c24c0040632cc43cf946a21a2874da82d860ca8b00de30`  
		Last Modified: Wed, 18 Nov 2020 01:34:15 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f326437ca16afa0d6cf34f03c89ad56d7e340c7fcd8bb2a0c4fbd9e954a8cf60`  
		Last Modified: Wed, 18 Nov 2020 01:38:55 GMT  
		Size: 12.5 MB (12458092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8094582527b08b710edd8c7a47dac939cedeac437cbf258e2b55483d5e38a4`  
		Last Modified: Wed, 18 Nov 2020 01:38:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0406c39180ae7065dcd5c5fc62d474869d71e2453f7be3833d9c484b25bb69`  
		Last Modified: Wed, 18 Nov 2020 01:38:58 GMT  
		Size: 26.3 MB (26319556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf061f8e9d7c6498fd4104927ff1c56e428176e8544cabbed28fb9be2b3352`  
		Last Modified: Wed, 18 Nov 2020 01:38:50 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12e3c3a3093f9c06ec159fadfe8de8a3d8b2ad2d0a0f527e35dfc4d569a5bfd`  
		Last Modified: Wed, 18 Nov 2020 01:38:51 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce428cb9cd56b228dba9bf85c0be1714308af4687b95d4639180140a013a84a8`  
		Last Modified: Wed, 18 Nov 2020 01:38:51 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f970ad59eb112f729a79dcadc95585ed63ff6e4b3db3370f861d595eb93ae08`  
		Last Modified: Wed, 18 Nov 2020 01:38:50 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8367a8d3c5ade9fd336a9c184af2e0612ee15b9ff91be1ddddcd1443871ac537`  
		Last Modified: Wed, 18 Nov 2020 20:25:04 GMT  
		Size: 16.1 MB (16061266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78aed123b6f1fbe3a0d83167d67fa96d62e968708ae39f8f0562c80e75d84e1`  
		Last Modified: Wed, 18 Nov 2020 20:25:01 GMT  
		Size: 14.8 KB (14754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e237d6ddcebfae481ec055b61becbeab6a8af78c1bda4377039f45b77aaba2`  
		Last Modified: Wed, 18 Nov 2020 20:25:01 GMT  
		Size: 12.8 MB (12848264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5216c100ed607f05b0bbeaf5750fe63b8dd3db22181de77c3449bcf1882d6d`  
		Last Modified: Wed, 18 Nov 2020 20:24:58 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8a41b0604972bfebbbe77427ef87fba50bad90cce2b01996a357d200bd6d41`  
		Last Modified: Wed, 18 Nov 2020 20:25:12 GMT  
		Size: 47.7 MB (47686151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14acafbecc6542bbd142969265af9e06fc8e6729d14c4359f8aa6a8d1354714`  
		Last Modified: Wed, 18 Nov 2020 20:24:58 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0ee005b104d6cc55d9ba39e53e83705effcbe58e860e9172085f703446993b`  
		Last Modified: Wed, 18 Nov 2020 20:24:58 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:a4829a2c28913f9938655d41bb048228642326169aeb63df67f39610d4ec2ac0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217810461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6831cb7f9072916f36dbfc5ab860c747d65ee25ea2b36f5590ca386df762e914`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:54:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 02:54:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 02:54:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:54:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 02:54:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 03:04:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 03:04:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:04:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 03:04:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 03:36:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 18 Nov 2020 03:36:13 GMT
ENV PHP_VERSION=7.3.24
# Wed, 18 Nov 2020 03:36:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Wed, 18 Nov 2020 03:36:15 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Wed, 18 Nov 2020 03:36:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 03:36:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 03:39:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 03:39:41 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 03:39:43 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 03:39:45 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 18 Nov 2020 03:39:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 03:39:47 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 03:39:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 03:39:50 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 03:39:50 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 03:39:51 GMT
CMD ["php-fpm"]
# Wed, 18 Nov 2020 23:46:25 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Wed, 18 Nov 2020 23:46:26 GMT
ENV TINI_VERSION=v0.19.0
# Wed, 18 Nov 2020 23:46:29 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Wed, 18 Nov 2020 23:50:44 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:50:47 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 18 Nov 2020 23:50:48 GMT
VOLUME [/var/www/html]
# Wed, 18 Nov 2020 23:50:49 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Wed, 18 Nov 2020 23:50:50 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Wed, 18 Nov 2020 23:51:11 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Wed, 18 Nov 2020 23:51:17 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Wed, 18 Nov 2020 23:51:19 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Wed, 18 Nov 2020 23:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 23:51:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfe6c188ae8daf1a09a047918e301010eaa2f14f98648e742a0beb8cc525ad7`  
		Last Modified: Wed, 18 Nov 2020 04:37:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7496e2962f6d5953bde1d172cf95cf12b1d8a90c07354c68de7ccd67923764`  
		Last Modified: Wed, 18 Nov 2020 04:37:40 GMT  
		Size: 70.3 MB (70337639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0299a101fd6922debd223a74c36a8a9c1d2503a553b2aadc7bb529d39bcdfe95`  
		Last Modified: Wed, 18 Nov 2020 04:37:21 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef05d4ae150836ccaa9a85a803017e63fcabbb77a309851a1fbce1e0522acc5b`  
		Last Modified: Wed, 18 Nov 2020 04:41:55 GMT  
		Size: 12.5 MB (12458903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6f497f37827e91c09db876393ad2dc1ae072cf102454de1b4e56f12cbb66ca`  
		Last Modified: Wed, 18 Nov 2020 04:41:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ade8a3c71a97a84251640ce974acc159a5b8ec7218f0ae94191dd71eb8ad902`  
		Last Modified: Wed, 18 Nov 2020 04:41:59 GMT  
		Size: 28.4 MB (28437845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72b702288165bcb1423a0616930048861a041052ca0388457d1584882a505c`  
		Last Modified: Wed, 18 Nov 2020 04:41:52 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7033492ebe48b527fbada975184ce4a652feaf0c886bb5685ab52130b393ad0c`  
		Last Modified: Wed, 18 Nov 2020 04:41:52 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152a293b46d3763a1cb7db3ff5f24420566932db31cda5f54e2b6e0fa00e0a17`  
		Last Modified: Wed, 18 Nov 2020 04:41:52 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e64de93965fdb6baa3572fe2438c94ed80b79d6c0ecbe81a3e7264c9a5d940`  
		Last Modified: Wed, 18 Nov 2020 04:41:52 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca536db33fd6f51b87d4f50066186de2f089fa3126225c062bc0280f26ce21f1`  
		Last Modified: Wed, 18 Nov 2020 23:53:05 GMT  
		Size: 19.4 MB (19405824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd915e4e8f87af8834d6be5df48e64d7c51f8e56f869958c98bb6b8f46652d89`  
		Last Modified: Wed, 18 Nov 2020 23:53:00 GMT  
		Size: 15.7 KB (15700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e089386a412f9da1cfdaee1d303cfff05e6992aae075ef5469d261e76738ed6`  
		Last Modified: Wed, 18 Nov 2020 23:53:01 GMT  
		Size: 13.6 MB (13589450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e330da0ab7979ff02e02e8dd2157e84f70da6152e271f9e8812302e6907e8ba`  
		Last Modified: Wed, 18 Nov 2020 23:52:57 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c557f5f67a0974b153fd02e3c68c78e3e936a52b2788cb936b8d724e50e63fb5`  
		Last Modified: Wed, 18 Nov 2020 23:53:11 GMT  
		Size: 47.7 MB (47686191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7371993804f174ee410ef0935cd1c707a30d6f3cf928ff87d2bb018d00e8f871`  
		Last Modified: Wed, 18 Nov 2020 23:52:58 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c5a134c41633cb55fd4010291d73bec759f2f002b206d6955b97b2faacfbbc`  
		Last Modified: Wed, 18 Nov 2020 23:52:57 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; 386

```console
$ docker pull friendica@sha256:bd2844122e4b593565cc359a8c26d6568900c6f87a3c43aaf94b5ad75f35d4cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234293560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee8a1d0a61dabc17c3cf06346c347708346f335ffea30cca334cfb9b4cebad4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:47:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 07:47:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 07:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:47:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 07:47:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 08:46:56 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 30 Oct 2020 00:21:38 GMT
ENV PHP_VERSION=7.3.24
# Fri, 30 Oct 2020 00:21:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Thu, 05 Nov 2020 22:21:50 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Thu, 05 Nov 2020 22:22:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Nov 2020 22:22:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 22:30:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 22:30:31 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 05 Nov 2020 22:30:33 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 22:30:34 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 05 Nov 2020 22:30:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 22:30:35 GMT
WORKDIR /var/www/html
# Thu, 05 Nov 2020 22:30:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 05 Nov 2020 22:30:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Nov 2020 22:30:37 GMT
EXPOSE 9000
# Thu, 05 Nov 2020 22:30:37 GMT
CMD ["php-fpm"]
# Fri, 06 Nov 2020 03:13:26 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 06 Nov 2020 03:13:26 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 06 Nov 2020 03:13:27 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 06 Nov 2020 03:16:05 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Nov 2020 03:16:06 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 06 Nov 2020 03:16:06 GMT
VOLUME [/var/www/html]
# Fri, 06 Nov 2020 03:16:06 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Fri, 06 Nov 2020 03:16:06 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Fri, 06 Nov 2020 03:16:20 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 06 Nov 2020 03:16:21 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Fri, 06 Nov 2020 03:16:21 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 06 Nov 2020 03:16:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Nov 2020 03:16:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c025d092578150306e736243d79877f016e308c259079f3050040068805ec2`  
		Last Modified: Tue, 13 Oct 2020 10:37:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af847e2bbb92ee205de4388ed3631534643337cd4c5487a4c0158092a75fba69`  
		Last Modified: Tue, 13 Oct 2020 10:38:32 GMT  
		Size: 81.2 MB (81196048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d53973650961722caa47d6c81a99b797341d74d6986661b78f0f5979b6197`  
		Last Modified: Tue, 13 Oct 2020 10:37:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbd832cf34fd26fb06bcd41f0093a44b0e18a4e48bc0f81fd4a24ed9c3b31a`  
		Last Modified: Fri, 06 Nov 2020 02:16:14 GMT  
		Size: 12.5 MB (12459377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2254e97ef939a238a5f9ec4e9227db81ff8eccd4c4a784aacba2c10dea63916b`  
		Last Modified: Fri, 06 Nov 2020 02:16:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0ef9f39b5c13e1c495718d6c6ac9230c57d560774ef15c2e452d26a93cdcb`  
		Last Modified: Fri, 06 Nov 2020 02:16:19 GMT  
		Size: 29.3 MB (29308240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91c73f1545f2561e6c3b280d7f4e168db73302bf126e660e26368b91e05207d`  
		Last Modified: Fri, 06 Nov 2020 02:16:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c270d53bb7b5e7632d318e70484a76ffb15422c8ba10d2314b2fb6b34e7fa79`  
		Last Modified: Fri, 06 Nov 2020 02:16:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a435aaf1f31dd8a9395628b76b3485d1a60e6fd68426beafdc1c5b4f448efeb`  
		Last Modified: Fri, 06 Nov 2020 02:16:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b4ae8f72bf123c94a13f20d5dbd63fd5af27c36be983834a5727a651dc704b`  
		Last Modified: Fri, 06 Nov 2020 02:16:10 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06ee9b3bda45e870e7149e632ef3c4441436f10c0a6c00cfc46d39fe3380aa1`  
		Last Modified: Fri, 06 Nov 2020 03:20:10 GMT  
		Size: 21.1 MB (21089588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55d80105ac2c34b6740969234ef9c31da4592de95a5356001639dfbb378d382`  
		Last Modified: Fri, 06 Nov 2020 03:20:00 GMT  
		Size: 16.1 KB (16115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2571cd05e5a089cbac5f440bbdccf048a055285f73ddd7e44255d671d8510f`  
		Last Modified: Fri, 06 Nov 2020 03:20:07 GMT  
		Size: 14.8 MB (14771436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00586f47bffad32a06b0e1cacd6fe6e060b4cad9f163a18a813bb060cb0b001`  
		Last Modified: Fri, 06 Nov 2020 03:19:58 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed51c5ae1d2f7f192f479f3e28e8f5eb434c142947da4ba2e581e5221f915ce0`  
		Last Modified: Fri, 06 Nov 2020 03:20:16 GMT  
		Size: 47.7 MB (47686189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d1bb15d6ac198e5ac63dfdd25b7d7eaf6a0a12de8d95d48e97a99c1b80c9a6`  
		Last Modified: Fri, 06 Nov 2020 03:19:59 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3a3b4091e6155f00dca365c6a3efec07e6cf840c4b1d7c8b70998152583f1b`  
		Last Modified: Fri, 06 Nov 2020 03:19:58 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; mips64le

```console
$ docker pull friendica@sha256:47293a11a48d86b028dc2f34112f9da76c671f437b7cbb48c94a386ef83ffee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208572998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9f6715f15a82eac85429e74b34e1a078b8aab4944d81bd1d7dd75557f019a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:15:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 07:15:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 07:16:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:16:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 07:16:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 07:42:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 07:42:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 07:42:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 07:42:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 09:20:06 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 18 Nov 2020 09:20:06 GMT
ENV PHP_VERSION=7.3.24
# Wed, 18 Nov 2020 09:20:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Wed, 18 Nov 2020 09:20:06 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Wed, 18 Nov 2020 09:20:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 09:20:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 09:33:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 09:33:25 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 09:33:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 09:33:29 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 18 Nov 2020 09:33:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 09:33:30 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 09:33:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 09:33:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 09:33:32 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 09:33:32 GMT
CMD ["php-fpm"]
# Wed, 18 Nov 2020 12:02:17 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Wed, 18 Nov 2020 12:02:18 GMT
ENV TINI_VERSION=v0.19.0
# Wed, 18 Nov 2020 12:02:21 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Wed, 18 Nov 2020 12:08:48 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:08:50 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 18 Nov 2020 12:08:51 GMT
VOLUME [/var/www/html]
# Wed, 18 Nov 2020 12:08:51 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Wed, 18 Nov 2020 12:08:51 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Wed, 18 Nov 2020 12:09:16 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Wed, 18 Nov 2020 12:09:18 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Wed, 18 Nov 2020 12:09:19 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Wed, 18 Nov 2020 12:09:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 12:09:20 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8a605388fd73fc0a30049e1816ed2373347cbf1ca6d77be293fa8862d2b3f5`  
		Last Modified: Wed, 18 Nov 2020 09:48:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4e3df7e0f49e71f681e38aaf78e338a20a808236b450b995a1cdc14a23984e`  
		Last Modified: Wed, 18 Nov 2020 09:49:47 GMT  
		Size: 61.4 MB (61388764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6316538eedb24d61e8570cb82fdf616a81fec0940e867631bf9386a7492f304b`  
		Last Modified: Wed, 18 Nov 2020 09:48:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e557b9f23345490999328df2fdd49e29c9b21b4b846feda2070997fab6fc1c0`  
		Last Modified: Wed, 18 Nov 2020 09:57:55 GMT  
		Size: 12.5 MB (12457368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605075d9839e3f5d55cf36c3e58de9350c2114e86f26162397634124241484cc`  
		Last Modified: Wed, 18 Nov 2020 09:57:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872538ca454ba432e7360a4189f9a87da21ad7242d07eb9789c1d9990d4bf05e`  
		Last Modified: Wed, 18 Nov 2020 09:58:09 GMT  
		Size: 28.1 MB (28106875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9f9bf926bcf7c5bdce9ccbe72af8962b0b505c300d3854e120fd7de3398567`  
		Last Modified: Wed, 18 Nov 2020 09:57:49 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689835116bc0ef5ee09b70964840cb73f5b7333d6f691dce27c59e8636fb350e`  
		Last Modified: Wed, 18 Nov 2020 09:57:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5bc768c463641f865af9fd5b0d25df68f48c604095775e4fe40665dacf1ce5`  
		Last Modified: Wed, 18 Nov 2020 09:57:49 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29858a9788bfcfe1cbe60fa644be2f31b7fe14e141d63e0ff66336bf1aaee9a1`  
		Last Modified: Wed, 18 Nov 2020 09:57:49 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2474fbfdd13b1c80d1129ea4ae2ebc95da22df539ab7c04b816e4780a8742c6`  
		Last Modified: Wed, 18 Nov 2020 12:11:28 GMT  
		Size: 19.4 MB (19449824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248863ed3d7c226b52680a3a503b33e0f945fb2695e69197ab04990933f87b72`  
		Last Modified: Wed, 18 Nov 2020 12:11:00 GMT  
		Size: 15.9 KB (15896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd76729a1f19735cd45edba8316caf5b7650dd34fd8c54a8b85bddf6dfa6b9e`  
		Last Modified: Wed, 18 Nov 2020 12:11:24 GMT  
		Size: 13.7 MB (13674318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80df921503f05caf6e681e3f345267790ee5d341dfe2d3ec2fdf298d041c13dd`  
		Last Modified: Wed, 18 Nov 2020 12:10:57 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee64e5559c0a6b9bfa43efb08fc4ebb172c6739adc03255268f96ff08462663`  
		Last Modified: Wed, 18 Nov 2020 12:11:44 GMT  
		Size: 47.7 MB (47686168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cec32376fb1483daeb78810e0d2da755bb095fcb3fd477c3f44b966521fa01`  
		Last Modified: Wed, 18 Nov 2020 12:10:57 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b438742a137ed71002fe055616c991972c902435c27eed5bc40e24dc845a02b`  
		Last Modified: Wed, 18 Nov 2020 12:10:57 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; ppc64le

```console
$ docker pull friendica@sha256:9b3f6e8183d214204bf47e10b0c98716729aadbbe923c88f51c3baf1ad9d0181
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242712138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424388ed74b1e2c8d185aee2f8a1f19ac6cd7fb60ca02be468895206c2750667`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 13:25:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Nov 2020 13:26:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Nov 2020 13:29:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 13:29:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Nov 2020 13:29:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Nov 2020 13:49:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 18 Nov 2020 13:49:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 13:49:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Nov 2020 13:49:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Nov 2020 14:54:26 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 18 Nov 2020 14:54:30 GMT
ENV PHP_VERSION=7.3.24
# Wed, 18 Nov 2020 14:54:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Wed, 18 Nov 2020 14:54:41 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Wed, 18 Nov 2020 14:56:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 14:56:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Nov 2020 15:02:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Nov 2020 15:02:34 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Wed, 18 Nov 2020 15:02:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Nov 2020 15:02:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 18 Nov 2020 15:03:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Nov 2020 15:03:03 GMT
WORKDIR /var/www/html
# Wed, 18 Nov 2020 15:03:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 18 Nov 2020 15:03:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 18 Nov 2020 15:03:28 GMT
EXPOSE 9000
# Wed, 18 Nov 2020 15:03:33 GMT
CMD ["php-fpm"]
# Thu, 19 Nov 2020 00:55:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Thu, 19 Nov 2020 00:55:38 GMT
ENV TINI_VERSION=v0.19.0
# Thu, 19 Nov 2020 00:55:54 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Thu, 19 Nov 2020 01:20:06 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 01:20:31 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 19 Nov 2020 01:20:43 GMT
VOLUME [/var/www/html]
# Thu, 19 Nov 2020 01:20:51 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Thu, 19 Nov 2020 01:20:57 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Thu, 19 Nov 2020 01:21:31 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 19 Nov 2020 01:21:39 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Thu, 19 Nov 2020 01:21:41 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Thu, 19 Nov 2020 01:21:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 01:21:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7345157b43f0655c8ac09a2a234d8a2f94542bb32ab16cf4880d4b09722e59`  
		Last Modified: Wed, 18 Nov 2020 15:46:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449b8a70df5c7fde5f5f4a781a4c6b695e0a940f7b4e10d3dcd0774e1efcc891`  
		Last Modified: Wed, 18 Nov 2020 15:47:05 GMT  
		Size: 82.3 MB (82259488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5babd79ef916acbafae12a90aa7e8b4ffa775d7104905dca61473f86a20263`  
		Last Modified: Wed, 18 Nov 2020 15:46:32 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a298e0a6a4b1699ec98098769394b1961259b27a9a88cd422db78988727b1302`  
		Last Modified: Wed, 18 Nov 2020 15:53:48 GMT  
		Size: 12.5 MB (12459931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e904764915c5512cd8007522b94bbe7f390d91bb4f298039d44935637377a7d`  
		Last Modified: Wed, 18 Nov 2020 15:53:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f15df1d9570759ae61da2f214450265981ba99644245d6cc6e628220f05bd79`  
		Last Modified: Wed, 18 Nov 2020 15:53:48 GMT  
		Size: 30.5 MB (30465226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377926854cace61ddecabbfb7909763f66e0d03d745d4452be5514163e84319f`  
		Last Modified: Wed, 18 Nov 2020 15:53:42 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9058e8f8ff77fdd71b84f24f926b894e2c3070f9a2c1f54ff8a50e287f7b2953`  
		Last Modified: Wed, 18 Nov 2020 15:53:42 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ff947068b2378884a5ba16491f939942280952ed93956facb8684f4b0a2f4e`  
		Last Modified: Wed, 18 Nov 2020 15:53:42 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6c66c42999be8d56a9e8f34cd928ee2e8c21419fd9bda8a2c89e68877a13c`  
		Last Modified: Wed, 18 Nov 2020 15:53:42 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3c2f91110053b2a48c628563c3615ceff29057f9e7fbb4fad34a87c829392`  
		Last Modified: Thu, 19 Nov 2020 01:25:19 GMT  
		Size: 23.9 MB (23888400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768d8e5278ef4c52868579f908b50ad7f1abacda7f799fcb00d17d19d7a26ebe`  
		Last Modified: Thu, 19 Nov 2020 01:25:14 GMT  
		Size: 16.3 KB (16322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e178c7a5ad30c40b131859bf97b1f32583042866cd04e45967d70de28e2e16f`  
		Last Modified: Thu, 19 Nov 2020 01:25:15 GMT  
		Size: 15.4 MB (15388501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a6b75725aa31dc1d6f871a798be255db43551f9ca4aeb9c1a4c662213c1dbd`  
		Last Modified: Thu, 19 Nov 2020 01:25:10 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84941d74eb4141c6e48d7708cf0c03a599c7bd2a01f1a15d4451c36ce9d9f87b`  
		Last Modified: Thu, 19 Nov 2020 01:25:20 GMT  
		Size: 47.7 MB (47686170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0964cfc8be4a61c826be7691d296dd991fcc6e2a4b619620ae6c23745a536a47`  
		Last Modified: Thu, 19 Nov 2020 01:25:10 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838143575948dec8dca43d5e82f8cbd188d1cbc98ecc8b1841de2326209174a3`  
		Last Modified: Thu, 19 Nov 2020 01:25:10 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; s390x

```console
$ docker pull friendica@sha256:f8c24824df700527b1c4ba09de11b3a5f02d9d7fad0e608bacdb4a1791d81135
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210615523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40da688a05626626e2d5307aad93d3264e68fb5ab1044fbe5470aab230111807`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:05:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Nov 2020 22:05:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Nov 2020 22:06:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:06:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Nov 2020 22:06:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Nov 2020 22:20:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 17 Nov 2020 22:20:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 22:20:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Nov 2020 22:20:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Nov 2020 23:19:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 17 Nov 2020 23:19:31 GMT
ENV PHP_VERSION=7.3.24
# Tue, 17 Nov 2020 23:19:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.24.tar.xz.asc
# Tue, 17 Nov 2020 23:19:33 GMT
ENV PHP_SHA256=78b0b417a147ab7572c874334d11654e3c61ec5b3f2170098e5db02fb0c89888
# Tue, 17 Nov 2020 23:19:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Nov 2020 23:19:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:27:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Nov 2020 23:27:36 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:27:38 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Nov 2020 23:27:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 17 Nov 2020 23:27:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Nov 2020 23:27:41 GMT
WORKDIR /var/www/html
# Tue, 17 Nov 2020 23:27:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 17 Nov 2020 23:27:44 GMT
STOPSIGNAL SIGQUIT
# Tue, 17 Nov 2020 23:27:45 GMT
EXPOSE 9000
# Tue, 17 Nov 2020 23:27:45 GMT
CMD ["php-fpm"]
# Wed, 18 Nov 2020 18:17:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Wed, 18 Nov 2020 18:17:58 GMT
ENV TINI_VERSION=v0.19.0
# Wed, 18 Nov 2020 18:18:01 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Wed, 18 Nov 2020 18:22:36 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 18:22:39 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 18 Nov 2020 18:22:40 GMT
VOLUME [/var/www/html]
# Wed, 18 Nov 2020 18:22:40 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Wed, 18 Nov 2020 18:22:41 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Wed, 18 Nov 2020 18:23:08 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Wed, 18 Nov 2020 18:23:14 GMT
COPY multi:fe4e917e01c1623d9fbcef6e6d61848ea22a09e81fdabad357a3be58b2c814b7 in / 
# Wed, 18 Nov 2020 18:23:15 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Wed, 18 Nov 2020 18:23:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 18:23:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee323c0bdcb822c2cb3d1bd93141d6d29b8940a6180a88839cd68c80fbd106c2`  
		Last Modified: Wed, 18 Nov 2020 00:07:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec8f1576a5517595c8a7a530526f62d922496f66584f9dbd8e4d72690c136ad`  
		Last Modified: Wed, 18 Nov 2020 00:07:28 GMT  
		Size: 64.7 MB (64706676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9ccf205c352e00231140d9f5c3f826695eb3a553ccbd4ffd9cfbee2b8411f`  
		Last Modified: Wed, 18 Nov 2020 00:07:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca39d7161c099196aced576076ad6dfc0c2cc8c2827ff821b20987534aad404`  
		Last Modified: Wed, 18 Nov 2020 00:11:41 GMT  
		Size: 12.5 MB (12458456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850f42b5c39945f7bb439435dbcc4ca53cbec70908194dc2210822e05ef85ed`  
		Last Modified: Wed, 18 Nov 2020 00:11:41 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797a8e2949a0554956454f5687c1a5129d5809ee4f3e4682bfed03f325a11349`  
		Last Modified: Wed, 18 Nov 2020 00:11:42 GMT  
		Size: 27.9 MB (27900346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cb07c8ea94322efa6570df9c186d0c8be87078340b14d09300bfa8c06be3a2`  
		Last Modified: Wed, 18 Nov 2020 00:11:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0656e3910b760d29f08eeef2cb887b192b98ddf685704b7d907d3011baddee8`  
		Last Modified: Wed, 18 Nov 2020 00:11:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858526c6cefafcdad0950e4a05369e614eb44017b3ac32361513e5180b7fdad`  
		Last Modified: Wed, 18 Nov 2020 00:11:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f5940743bcd7bd2dfaf19adf7f37ccad712d90f407254f9cf5369bfc34133d`  
		Last Modified: Wed, 18 Nov 2020 00:11:37 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b27a47982f8d364407d40fb192f0f4d4a9d487d0d12e5b72650814930eac14`  
		Last Modified: Wed, 18 Nov 2020 18:25:03 GMT  
		Size: 18.4 MB (18374927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6863096020a23e25dcc59ac628123f05c0f623c9bdae26854f459b4ee49cf3ff`  
		Last Modified: Wed, 18 Nov 2020 18:24:59 GMT  
		Size: 16.4 KB (16427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c18d5f009e2d49e07e87d3668b3a2f72ddefde1ec8305c45119b7f385d0ebc`  
		Last Modified: Wed, 18 Nov 2020 18:24:58 GMT  
		Size: 13.7 MB (13734989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edbd31563169d35e16d5b1e93839d5d78f07473ea52b837374c260a25b3cd0f`  
		Last Modified: Wed, 18 Nov 2020 18:24:56 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba504fe41f5ecb42193860303e11e6a20fc8d36268c1f8e04dcc8e4764c6fc`  
		Last Modified: Wed, 18 Nov 2020 18:25:04 GMT  
		Size: 47.7 MB (47686168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd569ed54e6e447578b6fc9191c724bbc82c5b4a0c827b8a9237e3eea9845df`  
		Last Modified: Wed, 18 Nov 2020 18:24:56 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996269054d2967c372e065ba8f92c0d074bec39fac48eb5f8cc16e2b8231d65`  
		Last Modified: Wed, 18 Nov 2020 18:24:55 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
