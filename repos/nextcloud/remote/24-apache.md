## `nextcloud:24-apache`

```console
$ docker pull nextcloud@sha256:cc9309e393c1362173bc763c2f033f804588658f329cf05672eceb28d8341f04
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

### `nextcloud:24-apache` - linux; amd64

```console
$ docker pull nextcloud@sha256:865daf7ddd5cd13762518b3b4c2589d18e361836119a7a58dfc235ae1a3b37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317598837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b770dbdebc5f6d31f9e86f3b9a7da7133d2f1d8b33ebd05b90eb3defeca14c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:39:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 00:50:28 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 00:50:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 00:50:29 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 00:50:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 00:50:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 00:53:34 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:53:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 00:53:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 00:53:35 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 00:53:35 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:53:35 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 00:53:35 GMT
EXPOSE 80
# Fri, 10 Jun 2022 00:53:35 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 03:28:33 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 10 Jun 2022 03:28:34 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 10 Jun 2022 03:28:34 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 10 Jun 2022 03:31:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 03:31:18 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 10 Jun 2022 03:31:18 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 03:31:19 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 21 Jun 2022 23:48:00 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Tue, 21 Jun 2022 23:48:42 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Jun 2022 23:48:44 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Tue, 21 Jun 2022 23:48:45 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 21 Jun 2022 23:48:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Jun 2022 23:48:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8da7928e6794c3678151992e658fc20885b6d267319d4cdcefa1cf36d61f121`  
		Last Modified: Fri, 10 Jun 2022 01:42:54 GMT  
		Size: 11.2 MB (11218836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa0c876b41f525bfd65d8aa2bd90f2a21e4646fefa346f40b4c96ca4f095c05`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf79d622325039c1d301c7152e7e9a8583852e18d82b5dbaf8e54c07b3120a52`  
		Last Modified: Fri, 10 Jun 2022 01:42:53 GMT  
		Size: 10.8 MB (10774751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff0e31f4907cc931e04204514f6ddc7dde3a008847646a34a6578f618426ae6`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97ccd5e9d41a7718d888fc5f36bb6ae9f445ae909838a18beece388ffe13ace`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd678d497712d7c9e108a6af8ae2158a6de7e4e39a8c24661855231097d05d7`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21128a5b47b9d33dfd217bfd81dce8f7387eabaf91375baf89db0f6f702315d7`  
		Last Modified: Fri, 10 Jun 2022 03:40:56 GMT  
		Size: 1.7 MB (1700920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af3245d4c4b048c721fec320664ae8b9a8c44f8edad1d4e702b1a74fb31780d`  
		Last Modified: Fri, 10 Jun 2022 03:40:58 GMT  
		Size: 17.5 MB (17487591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a17bb72e04d513016b9d63c89fb354cd61d0b1c6bd914b4df714af168de0d4`  
		Last Modified: Fri, 10 Jun 2022 03:40:53 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1f987da77cb372e128e4e6b0ad996b36de38a4a4d84d565c611b869d5ca7fb`  
		Last Modified: Fri, 10 Jun 2022 03:40:56 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba66568e4e9cb8867120686a726b1413fbc2a031956692a46e4805896347cb90`  
		Last Modified: Tue, 21 Jun 2022 23:55:32 GMT  
		Size: 134.2 MB (134173818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5a8c5fc6c40f8d9ee9cf83ec5c084d4b0a5871dbddfdf9ab8ca6a750eba7f4`  
		Last Modified: Tue, 21 Jun 2022 23:55:16 GMT  
		Size: 3.0 KB (3013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c5ea3edb86044e7da0f39951834a7b6b13ccedc1eb5349c65caa4194823b87`  
		Last Modified: Tue, 21 Jun 2022 23:55:16 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:e3efbcdeab747e9c73b633573951062aff9e75870de8545236be9e99ffe39db5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.2 MB (293184873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162390b41cb1338af0d7b531a7315a7049d7ad9573f92735558abacda55b1323`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 23:35:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 23:35:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 23:36:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 23:36:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 23:36:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 23:41:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 23:41:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 23:42:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 23:42:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 23:42:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 23:42:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 23:42:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 23:42:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Jun 2022 01:59:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 24 Jun 2022 02:44:06 GMT
ENV PHP_VERSION=8.0.20
# Fri, 24 Jun 2022 02:44:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 24 Jun 2022 02:44:07 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 24 Jun 2022 02:44:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jun 2022 02:44:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jun 2022 02:49:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 24 Jun 2022 02:49:32 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 24 Jun 2022 02:49:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jun 2022 02:49:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jun 2022 02:49:35 GMT
STOPSIGNAL SIGWINCH
# Fri, 24 Jun 2022 02:49:35 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 24 Jun 2022 02:49:36 GMT
WORKDIR /var/www/html
# Fri, 24 Jun 2022 02:49:36 GMT
EXPOSE 80
# Fri, 24 Jun 2022 02:49:36 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jun 2022 15:40:46 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 24 Jun 2022 15:40:47 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 24 Jun 2022 15:40:47 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 24 Jun 2022 15:47:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 15:47:39 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 24 Jun 2022 15:47:40 GMT
VOLUME [/var/www/html]
# Fri, 24 Jun 2022 15:47:41 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 24 Jun 2022 16:04:29 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Fri, 24 Jun 2022 16:05:59 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 16:06:01 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Fri, 24 Jun 2022 16:06:04 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Fri, 24 Jun 2022 16:06:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jun 2022 16:06:04 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e09f88f3062c4ac137aceba98450d079bdce7152b5329623464a6542325584`  
		Last Modified: Fri, 24 Jun 2022 04:17:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe814f0e772803c6ff5bfa73308b751c597dd457ec3c64cd244b3ae64d384ce`  
		Last Modified: Fri, 24 Jun 2022 04:18:27 GMT  
		Size: 73.7 MB (73685507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b36f773d9748a4a3dd653209f9309cf65790c131a8f74000a5c238b404656fc`  
		Last Modified: Fri, 24 Jun 2022 04:17:37 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd91b55f976c2d294b7fb809a76fef4bf5b9d27f037261fdcb314cf4836a583`  
		Last Modified: Fri, 24 Jun 2022 04:19:17 GMT  
		Size: 18.5 MB (18545718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e33fcf758cd2eeca055274206601c964d56363b50ae31db3484bfdb4b58572c`  
		Last Modified: Fri, 24 Jun 2022 04:19:06 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba5a8d9530d18c8db8d0d095d695edcf7cdb36e54aa2f5f370047aa8ffec6c`  
		Last Modified: Fri, 24 Jun 2022 04:19:06 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33080ac20ac80fb914921d55ff227657c68bf1ae789dfe7b155e7e62080a7ded`  
		Last Modified: Fri, 24 Jun 2022 04:39:45 GMT  
		Size: 11.2 MB (11217610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4db983d6bb5151046c6f39e5cbae29d997fab182366972b44ab7601f8f0e5c0`  
		Last Modified: Fri, 24 Jun 2022 04:39:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69284bdd72d4ac54bbc9c6d929d4387ee3e2cd220bf72aa7d8eb16ad70f900e8`  
		Last Modified: Fri, 24 Jun 2022 04:39:48 GMT  
		Size: 9.8 MB (9790407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512b711164cd58543f5910fc88122143532a7a2558d82442a352062adc0cd82e`  
		Last Modified: Fri, 24 Jun 2022 04:39:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc31d38aa5816dd8376d77603bfdde496a0b492657a5ad351392e53441b0e00b`  
		Last Modified: Fri, 24 Jun 2022 04:39:40 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc61980674ad98882c4bcb3cd1e9c82b072dd14d717c96bc85445a855305dd64`  
		Last Modified: Fri, 24 Jun 2022 04:39:40 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a2bdbb3f5d9ab678633a1891595bb1acde8f9310249911cf2dfb0ad8ac5a78`  
		Last Modified: Fri, 24 Jun 2022 16:10:46 GMT  
		Size: 1.7 MB (1656679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6529743af6608fb24f9096717734fe5826f97375ddd360606d2e07ede7d7b4f7`  
		Last Modified: Fri, 24 Jun 2022 16:10:55 GMT  
		Size: 15.2 MB (15183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f357b0f53bb6892a01f02c25143be67da5df9794ab6de80eafebbf623b19d9cd`  
		Last Modified: Fri, 24 Jun 2022 16:10:44 GMT  
		Size: 599.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70c632b1f9b838ac992ace460bc0c05a4487a9220d4ae82fb3667b8e032eab1`  
		Last Modified: Fri, 24 Jun 2022 16:10:44 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d27cbb8eb53c03e369f26e7eecf612a8973059feea0340818a5153d9eef554d`  
		Last Modified: Fri, 24 Jun 2022 16:19:47 GMT  
		Size: 134.2 MB (134171974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e800f147ebeeed230283bbe4d4324262b7a402ca4922c572b2acd2eed40a4d8`  
		Last Modified: Fri, 24 Jun 2022 16:18:22 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2300d1928eddd6f6a12a531271c6f7bba2b99fc0e1918910d8df1903fe55eaef`  
		Last Modified: Fri, 24 Jun 2022 16:18:22 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:7c65677deaa08a3604b26932e206c6eb96561e7d1533b27657e33997bf0f97c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.2 MB (284154504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11598345e8eade6975004e9dd3b56eb4be0929304b3179848ce707fec4a9295e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 07:20:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 29 May 2022 07:20:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 29 May 2022 07:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 07:21:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 29 May 2022 07:21:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 29 May 2022 07:26:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sun, 29 May 2022 07:26:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sun, 29 May 2022 07:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sun, 29 May 2022 07:27:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sun, 29 May 2022 07:27:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sun, 29 May 2022 07:27:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:27:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:27:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sun, 29 May 2022 08:12:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 03:15:27 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 03:15:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 03:15:27 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 03:15:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 03:15:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:20:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 03:20:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:20:26 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 03:20:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 03:20:27 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 03:20:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:20:28 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 03:20:28 GMT
EXPOSE 80
# Fri, 10 Jun 2022 03:20:29 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 10:51:16 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 10 Jun 2022 10:51:17 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 10 Jun 2022 10:51:17 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 10 Jun 2022 10:58:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 10:58:05 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 10 Jun 2022 10:58:05 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 10:58:07 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 21 Jun 2022 23:10:18 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Tue, 21 Jun 2022 23:11:45 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Jun 2022 23:11:48 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Tue, 21 Jun 2022 23:11:50 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 21 Jun 2022 23:11:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Jun 2022 23:11:51 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d3aba112689c02d6b26a241e0065c97e4d937ec22a83ec2611313d531e8b0a`  
		Last Modified: Sun, 29 May 2022 10:31:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c1acd8b719bd38a8741d6d093c916a6a558e402efb4f9e8a9c0d8331959d0d`  
		Last Modified: Sun, 29 May 2022 10:31:44 GMT  
		Size: 69.3 MB (69318858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669dd875526c016d77dc484bfa38a4f856de0994a919ad17c67ba551ea39613a`  
		Last Modified: Sun, 29 May 2022 10:31:01 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b62250e8ba44edd5728ef78550f4413110a8e30299f9759013a4a2cc1895e2`  
		Last Modified: Sun, 29 May 2022 10:33:02 GMT  
		Size: 18.0 MB (17993441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ada171d9ed11a53015749eebc93e05f658d1b63f4b62423ef83f2886cb2611`  
		Last Modified: Sun, 29 May 2022 10:32:52 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f5395bf69c3010288a162f6244f829e5cff002fa2f6e52ca8ed267c3f27b64`  
		Last Modified: Sun, 29 May 2022 10:32:52 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0810a76231e24ecfdb4fd8691e8d8711ce8d8eb05b6b4d4ed35e92108ac037`  
		Last Modified: Fri, 10 Jun 2022 04:46:45 GMT  
		Size: 11.2 MB (11217645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78439a09f93def0b2bcccfabddd807a1a450154598df011ac38968167c90b666`  
		Last Modified: Fri, 10 Jun 2022 04:46:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67aa67e30060e970fad11dd6d9ce0d1092358f7b8f1917a36b206c10cf13d63`  
		Last Modified: Fri, 10 Jun 2022 04:46:47 GMT  
		Size: 9.3 MB (9305929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72bffa9cf9c2ace904c27a07724c8c56d7a422b9a5dc3cf067c5c2839bffece`  
		Last Modified: Fri, 10 Jun 2022 04:46:40 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e67ae5da713049b8fa577296b5b6baf2f5437e4252c0d10c3b848bd88a6a2a`  
		Last Modified: Fri, 10 Jun 2022 04:46:41 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ffeb74aca3c1bee0ec90466e3b864fa19668389aefbaeede12432487239d02`  
		Last Modified: Fri, 10 Jun 2022 04:46:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce69f844d89c039bba39101a7e1cd7a7962d57790e7253696afab178e66efd`  
		Last Modified: Fri, 10 Jun 2022 11:20:32 GMT  
		Size: 1.5 MB (1510705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69d58ba24ed1ea8d2206895068f22e98298e730b714482ca61580c5b783960a`  
		Last Modified: Fri, 10 Jun 2022 11:20:39 GMT  
		Size: 14.0 MB (14047605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247fa981a24d519cef08285a22f66b05a3168c0243fce708e2fbff993a92178c`  
		Last Modified: Fri, 10 Jun 2022 11:20:30 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3670d804b1b4c98505f95c96eaaf7737744a4cf912a7b7b73f4f7aa1f8c06d`  
		Last Modified: Fri, 10 Jun 2022 11:20:30 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223af9071840a4b1729e8e299cdac629a0c5096406a4e82d65feca22ba55c638`  
		Last Modified: Tue, 21 Jun 2022 23:33:27 GMT  
		Size: 134.2 MB (134172094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534599d921fd24afb5bc54fcc782efc191bdb457de2f6eb2c6b1a7c140f151f7`  
		Last Modified: Tue, 21 Jun 2022 23:32:00 GMT  
		Size: 3.0 KB (3013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628916aa7ad17d022645642c8183bbc57bcdaa0a5409f9bd544983af5c70df3f`  
		Last Modified: Tue, 21 Jun 2022 23:31:59 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:0d6823c324ca534d800f8643edaa6e7c42c83509f83ebf9b08a4f26a255f41cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.4 MB (307409862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c54644adecaa7e768fb4f9a2035658b1f166df9a3866fa610ef3d29bfc2c3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 07:41:36 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jun 2022 07:41:37 GMT
ENV PHP_VERSION=8.0.20
# Thu, 23 Jun 2022 07:41:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Thu, 23 Jun 2022 07:41:39 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Thu, 23 Jun 2022 07:41:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 07:41:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 07:44:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 07:44:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 07:44:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 07:44:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 07:44:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 07:44:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 07:44:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 07:44:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 07:44:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:28:48 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 23 Jun 2022 21:28:49 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 23 Jun 2022 21:28:50 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 24 Jun 2022 09:26:29 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 09:26:30 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 24 Jun 2022 09:26:31 GMT
VOLUME [/var/www/html]
# Fri, 24 Jun 2022 09:26:32 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 24 Jun 2022 09:26:33 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Fri, 24 Jun 2022 09:27:12 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 09:27:14 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Fri, 24 Jun 2022 09:27:16 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Fri, 24 Jun 2022 09:27:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jun 2022 09:27:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348c58c704b0fc585d43b532cb116da9c992f6d4f486787159e9b244ba0f5664`  
		Last Modified: Thu, 23 Jun 2022 08:40:30 GMT  
		Size: 11.0 MB (11003340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc7bb918d7cba47e93727f2f8d91b52c18f54e3aa4739a28e4a23fdcaf480fb`  
		Last Modified: Thu, 23 Jun 2022 08:40:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e0b6d994663cb0734ced6392d0ffaa09c5c47c799025cfee2387705fbe0909`  
		Last Modified: Thu, 23 Jun 2022 08:40:28 GMT  
		Size: 10.2 MB (10231573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddda15445007d351408b7946df6fae07e307f8d9a93b2979c2ceec280c9b845`  
		Last Modified: Thu, 23 Jun 2022 08:40:26 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995bfe8a33b18666856f338926587e2cda7e0d6694eaae18724f476cb46debff`  
		Last Modified: Thu, 23 Jun 2022 08:40:26 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd306e6ddec24282a5fede5b8ad9c2d86d1fc4f2aaaaec950958e8bdcfb02b`  
		Last Modified: Thu, 23 Jun 2022 08:40:26 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c994555b9a99042fc97e3b355ff6e3b3e1b028d323e07749d5f1b352641b7e70`  
		Last Modified: Fri, 24 Jun 2022 09:32:06 GMT  
		Size: 1.4 MB (1432169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7da03b75cb3568d88fad72dec30f421b794eeccd2d0dd6e51b7ee734dd789d`  
		Last Modified: Fri, 24 Jun 2022 09:32:07 GMT  
		Size: 15.1 MB (15069456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc447c4e97bb1a4fc5e61d50b3188d3e58948c658fe01f0e12b7a362e205d317`  
		Last Modified: Fri, 24 Jun 2022 09:32:03 GMT  
		Size: 565.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc592139aa1c0f40e10891c4b58cdc499a9da726cd33b0bde533cbb00b3ae40f`  
		Last Modified: Fri, 24 Jun 2022 09:32:03 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b4af6194646a7c1dc2100e2d50df3ab2bde935a1499b853cb572c83bec2709`  
		Last Modified: Fri, 24 Jun 2022 09:32:21 GMT  
		Size: 133.9 MB (133933420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d224f14b4b2b180ca2ba03b7a7b84cdc06044667db1e06416d57b296e422a0e1`  
		Last Modified: Fri, 24 Jun 2022 09:32:03 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7081020a6c1aae28a9191fec8558a8320b508b4d80abee30a7ea2e3144bbc16c`  
		Last Modified: Fri, 24 Jun 2022 09:32:03 GMT  
		Size: 2.2 KB (2201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; 386

```console
$ docker pull nextcloud@sha256:89c877534354b7cd02be7e32a979e85a108475d31b799beafae4b0f1f4c73ade
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.6 MB (318621085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7d619de237083fe2dec2ed9450fddc7d987a2038de475e70d8a23ef46e495`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 11:41:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 11:41:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 11:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 11:42:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 11:42:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 11:45:22 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 11:45:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 11:45:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 11:45:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 11:45:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 11:45:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 11:45:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 11:45:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 12:37:42 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jun 2022 12:37:43 GMT
ENV PHP_VERSION=8.0.20
# Thu, 23 Jun 2022 12:37:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Thu, 23 Jun 2022 12:37:45 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Thu, 23 Jun 2022 12:38:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 12:38:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 12:40:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 12:40:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 12:40:42 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 12:40:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 12:40:44 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 12:40:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 12:40:46 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 12:40:47 GMT
EXPOSE 80
# Thu, 23 Jun 2022 12:40:48 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 18:02:06 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 23 Jun 2022 18:02:06 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 23 Jun 2022 18:02:07 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 23 Jun 2022 18:04:45 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 18:04:46 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 23 Jun 2022 18:04:47 GMT
VOLUME [/var/www/html]
# Thu, 23 Jun 2022 18:04:48 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 23 Jun 2022 18:11:20 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Thu, 23 Jun 2022 18:12:04 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 18:12:06 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Thu, 23 Jun 2022 18:12:07 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Thu, 23 Jun 2022 18:12:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 18:12:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1090d3a60d1d6fdda24dfc39bebc748986624eb6704d50fec74f24f9d02bd359`  
		Last Modified: Thu, 23 Jun 2022 13:26:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42ca7953461e2d2ec71f3f7b3be3185bbef10580cc04d8b2dd05333e08ae016`  
		Last Modified: Thu, 23 Jun 2022 13:26:59 GMT  
		Size: 92.5 MB (92512688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26af2ccf84cef54d7640e15316beaa5cd504fe5d633458a7c2abbc8339c8279e`  
		Last Modified: Thu, 23 Jun 2022 13:26:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57286f1780cb4cf221e413558d2a6eedd0c265fcb2c17c71e8dde3eb874fa5e`  
		Last Modified: Thu, 23 Jun 2022 13:27:43 GMT  
		Size: 19.5 MB (19501632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957814d66da2e21922c95f2b31959035f5cf2cdb0c6c4415a7a0deff05faca43`  
		Last Modified: Thu, 23 Jun 2022 13:27:38 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4787d42868be303dfaed01875bfbb22fc8f9d97d02609ec7bf66eaa3b6364dc6`  
		Last Modified: Thu, 23 Jun 2022 13:27:38 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6246530bab10372574270ac2a80406ba9a3e23406b6f9aa475cfb814c907ad88`  
		Last Modified: Thu, 23 Jun 2022 13:36:39 GMT  
		Size: 11.0 MB (11003350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86fa8634c824bbb2916b5c253e9c48bb8a9195ad8d4a6af40cf1b3cbe86212e`  
		Last Modified: Thu, 23 Jun 2022 13:36:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a7ba1e39d0d2b9b724d0fa88b87b9a7246f7de659e9600c205001d400fd6f7`  
		Last Modified: Thu, 23 Jun 2022 13:36:37 GMT  
		Size: 11.0 MB (10978563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5f4c88fcefbdf4ee9608726a6720e7de67ee7049b4665ff731dbf716d04cc`  
		Last Modified: Thu, 23 Jun 2022 13:36:36 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff4f87489d89fe403c291ae3eb7fb87238a6804e16529646e797295712cc267`  
		Last Modified: Thu, 23 Jun 2022 13:36:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0b090c1c8f3b5297511c1287b53adfc9e044e67346d8787c1a114e98c1a440`  
		Last Modified: Thu, 23 Jun 2022 13:36:36 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cacd8b9f19968b3b9b9b4146207af5385b88cc2925fb33e0c799602bf18a17`  
		Last Modified: Thu, 23 Jun 2022 18:14:51 GMT  
		Size: 1.5 MB (1516410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cb0d104ab66706f9be23d09e0121e9aa2abd50ad4cb9b31373d55ce09afbc7`  
		Last Modified: Thu, 23 Jun 2022 18:14:53 GMT  
		Size: 16.8 MB (16773045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9932a18ae70679574e70858a8fdb960ab4a0058e4a7afed6286ae46ddd6dbeb`  
		Last Modified: Thu, 23 Jun 2022 18:14:48 GMT  
		Size: 565.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f94a5d9d564d540412c5ef538b090ee2e294f4e3a6e9b231e57aa0245e31582`  
		Last Modified: Thu, 23 Jun 2022 18:14:48 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5719f32c7da61e0f1043e26dc613873473a291e263dcf5a16ba152e5ae85571c`  
		Last Modified: Thu, 23 Jun 2022 18:17:51 GMT  
		Size: 133.9 MB (133933392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b5a3035328dcc7a7e785e3a72c779fbadf099b1a29bef27e35bf38e6e5140a`  
		Last Modified: Thu, 23 Jun 2022 18:17:32 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8344ce041362cd1007b2c7aa2b8d0b0cbc93d33ce8aa1d84c4728df31885cb59`  
		Last Modified: Thu, 23 Jun 2022 18:17:32 GMT  
		Size: 2.2 KB (2198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; mips64le

```console
$ docker pull nextcloud@sha256:6711516b09f06ff5a8ae7de461b98e50f60667a0435ff0d7c26f2c2146719911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291833132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccae89f27328500126dbf0858cbdddf7faaef4d3dadf3da18eb45af25bbd604`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:30:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 03:30:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:32:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 03:32:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 03:46:37 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 03:46:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 03:47:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 03:47:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 03:47:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 03:47:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 03:47:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 03:48:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 05:44:55 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 02:55:44 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 02:55:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 02:55:52 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 02:56:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 02:56:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:10:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 03:10:07 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:10:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 03:10:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 03:10:21 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 03:10:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:10:27 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 03:10:31 GMT
EXPOSE 80
# Fri, 10 Jun 2022 03:10:35 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 09:13:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 10 Jun 2022 09:13:58 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 10 Jun 2022 09:14:02 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 10 Jun 2022 09:26:35 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 09:26:43 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 10 Jun 2022 09:26:47 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 09:26:55 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 21 Jun 2022 23:21:09 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Tue, 21 Jun 2022 23:23:42 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Jun 2022 23:23:52 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Tue, 21 Jun 2022 23:24:01 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 21 Jun 2022 23:24:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Jun 2022 23:24:17 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48ffa812cba4145b49cbbc61824a577807dfbea2e248d5216b5b1fa5d6d81b5`  
		Last Modified: Sat, 28 May 2022 10:42:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ee5523dfa904c61988aab187090bf4bdb8ce8a4c4b8fa903a0ae6bc67d00cc`  
		Last Modified: Sat, 28 May 2022 10:43:14 GMT  
		Size: 71.8 MB (71812105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85368acf1e84d74f279250b786757fc0fad630ccedb2cf42c99422aee2bd1097`  
		Last Modified: Sat, 28 May 2022 10:42:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3d2a738e63dfed168edc3c29258832be93684258d02b06a2b24e4e6aa434`  
		Last Modified: Sat, 28 May 2022 10:44:17 GMT  
		Size: 18.9 MB (18933116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66edaf522933dedc6d868e8f08ca79a936b873e00d232920dc4c3401c31eb0b`  
		Last Modified: Sat, 28 May 2022 10:44:04 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbae8f5d7ec49c8d7b9e972935e1d7dce5fddc80dc90a2cc4852c0f4ef42974`  
		Last Modified: Sat, 28 May 2022 10:44:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555c0b1d77d4e9fcab24e98ef6726127ecc0213bc6cf2787a67a930e950e59a5`  
		Last Modified: Fri, 10 Jun 2022 06:11:14 GMT  
		Size: 11.0 MB (11002170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8800f1d624a7aa13a796bfdf11abb7d2f88cc759d6f095d12573a7b5b428cca`  
		Last Modified: Fri, 10 Jun 2022 06:11:09 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bc3c1c129b47b8ba088e2723b4d6a29de5f2e3c31a62020d83fa59a511e8ed`  
		Last Modified: Fri, 10 Jun 2022 06:11:16 GMT  
		Size: 9.9 MB (9917719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a27d7308d0fdae16db5d11d26e7543e8d88cde1318cc1bc6bd08b198dbbb90`  
		Last Modified: Fri, 10 Jun 2022 06:11:08 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c031687977a5322d1732f9749286880f5fdbed2fd96582548b30694ef2455da4`  
		Last Modified: Fri, 10 Jun 2022 06:11:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c5d53a5588c59e90faf9a23e6bd2c75225d27053a0aa2fedd5f3cb961bae46`  
		Last Modified: Fri, 10 Jun 2022 06:11:08 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a927aaeab6467ade5d99f134409e729c51366da5cc79225fba309841bbcbb929`  
		Last Modified: Fri, 10 Jun 2022 10:01:50 GMT  
		Size: 1.6 MB (1568632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af507461cb2ed4ccf30d31c7ee5831350a1447117852b02ee0c8beb83da7ad9`  
		Last Modified: Fri, 10 Jun 2022 10:02:02 GMT  
		Size: 15.0 MB (15011608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54207a3656efcd281dbaa38701e7b9157f0292636fb04896d3312f822e3ea414`  
		Last Modified: Fri, 10 Jun 2022 10:01:47 GMT  
		Size: 570.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529abdfd475cf1493c5eb90dcef1764f4c7549e9cf71cd5f1b52a411e0164a63`  
		Last Modified: Fri, 10 Jun 2022 10:01:46 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e3e3941132c6fe61429e78a3e26df4d163c035b40140b0a010dfddb323c9b7`  
		Last Modified: Tue, 21 Jun 2022 23:37:41 GMT  
		Size: 133.9 MB (133934695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e541009516ada43ba64f79b9a1d3ac8c1f90bcfc928832a287b8f0ece2dc2ab`  
		Last Modified: Tue, 21 Jun 2022 23:36:19 GMT  
		Size: 3.0 KB (3012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f3ed915e9355770c6a641ec7882a20c0f5fcfafb35753957aa0dba4bbec742`  
		Last Modified: Tue, 21 Jun 2022 23:36:19 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:2d0fb0d3c533b7145d755930618bf2de0b5a8e31dd7fcbcc3ad8f950d06c9e7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.8 MB (317789767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3d5aeccfc1a4e69ed7d913ffb31e427890dfc5fda6a276a2570f83ea3b2265`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:19:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 13:19:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 13:21:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:21:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 13:21:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 13:30:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 13:30:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 13:31:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 13:32:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 13:32:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 13:32:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:32:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 13:32:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 15:45:50 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jun 2022 15:46:00 GMT
ENV PHP_VERSION=8.0.20
# Thu, 23 Jun 2022 15:46:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Thu, 23 Jun 2022 15:46:27 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Thu, 23 Jun 2022 15:50:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 15:50:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:58:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 15:58:58 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:59:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 15:59:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 15:59:32 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 15:59:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:59:39 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 15:59:48 GMT
EXPOSE 80
# Thu, 23 Jun 2022 15:59:55 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jun 2022 16:01:36 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 24 Jun 2022 16:01:42 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 24 Jun 2022 16:01:46 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 24 Jun 2022 16:12:15 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 16:12:23 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 24 Jun 2022 16:12:28 GMT
VOLUME [/var/www/html]
# Fri, 24 Jun 2022 16:12:35 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 24 Jun 2022 16:34:10 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Fri, 24 Jun 2022 16:35:56 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 16:36:02 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Fri, 24 Jun 2022 16:36:05 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Fri, 24 Jun 2022 16:36:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jun 2022 16:36:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618065a0bfa6328b4fa8bfa229184683290183358ab149e3cef6f7df5bd46640`  
		Last Modified: Thu, 23 Jun 2022 17:34:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653612b565ca7461d374ea3a3a41e762b8a5cb9feb9a82568ac1630fb1fd7a93`  
		Last Modified: Thu, 23 Jun 2022 17:35:14 GMT  
		Size: 86.6 MB (86628379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1e1e66d25ba24674f96f2e04415857aac883817afbcf72ae287832b06683a7`  
		Last Modified: Thu, 23 Jun 2022 17:34:36 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc202bcdf402267f23756b080fd5cc6e078589a8b1294cc846ec639869e39f1`  
		Last Modified: Thu, 23 Jun 2022 17:36:03 GMT  
		Size: 20.5 MB (20453759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c44daf1952ff503c2962078c3daec863935d86b9e263096d7cc79688d2e2888`  
		Last Modified: Thu, 23 Jun 2022 17:35:53 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ba6bd1c324b429743a954b6c0038ec40197bf41698336fe1a15a627fb1410`  
		Last Modified: Thu, 23 Jun 2022 17:35:52 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1cade60dbeba310860c5f2ae30932c098816d1868240418a5fb54851baab3f`  
		Last Modified: Thu, 23 Jun 2022 17:45:58 GMT  
		Size: 11.2 MB (11219322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72961a2ded5785b4282a711ee3d204caf0b22ce7047a928ac8492efd6c6e2ce7`  
		Last Modified: Thu, 23 Jun 2022 17:45:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36a12f8a6cd7f498a5e495250847cb822785ed448f27c4daa131ef41f78061`  
		Last Modified: Thu, 23 Jun 2022 17:45:57 GMT  
		Size: 11.1 MB (11138121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88a834b0ffd945330665156c2f6ba436654dbfba5091cd7da0e89c5873ff03`  
		Last Modified: Thu, 23 Jun 2022 17:45:54 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df673f646f8e1141125dae68face5933b87fd9c25478330906f8b4ddb20535ad`  
		Last Modified: Thu, 23 Jun 2022 17:45:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d87656bcfa51726864e4b687f8e6d85c55782ada9869181f0fb1717ad636ab`  
		Last Modified: Thu, 23 Jun 2022 17:45:54 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b7ed09c265d00beec7f090d9c8a7d8e3b8def0dbab566101d9825147de570d`  
		Last Modified: Fri, 24 Jun 2022 16:40:02 GMT  
		Size: 1.9 MB (1871682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce6952687372e83b73ef791e0dafbd408672f78314b56e80d36144be1d535df`  
		Last Modified: Fri, 24 Jun 2022 16:40:10 GMT  
		Size: 17.0 MB (17002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981f19a05b22d3d88d3b7ef439e91ee9cb69aa8d42f6b4b7057df238e86d3c0e`  
		Last Modified: Fri, 24 Jun 2022 16:39:56 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c945eb11423924cc912f96c9c4a1f2c120bda713adbb191891cffae1100715`  
		Last Modified: Fri, 24 Jun 2022 16:39:56 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18d0a5014b00eb36279f155a2eea05a941d0c701628a031712be15eaf2538e`  
		Last Modified: Fri, 24 Jun 2022 16:51:58 GMT  
		Size: 134.2 MB (134176738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95915009f4d98a61cbd8d694d3764ea8aebefb78cd1fb1225329e6f43b864f3f`  
		Last Modified: Fri, 24 Jun 2022 16:50:19 GMT  
		Size: 3.0 KB (3013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850414523c22f431df947fc99cceb8d01b8ad1742ebeae2d544bcddaee673292`  
		Last Modified: Fri, 24 Jun 2022 16:50:19 GMT  
		Size: 2.2 KB (2200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-apache` - linux; s390x

```console
$ docker pull nextcloud@sha256:578d5b7bc13f7f002534cf5f4c1a4f4336983f28ad6b8899c8434f06b04bf2e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292370285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5db097063032f858e703a0f085301ccd4ee04608a6961775eda14f1551d5fc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:23:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:23:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:23:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:24:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:24:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:26:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:26:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:26:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:26:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:26:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:26:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:26:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:26:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 07:10:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jun 2022 07:10:48 GMT
ENV PHP_VERSION=8.0.20
# Thu, 23 Jun 2022 07:10:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Thu, 23 Jun 2022 07:10:48 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Thu, 23 Jun 2022 07:10:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 07:10:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 07:13:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 07:13:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 07:13:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 07:13:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 07:13:38 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 07:13:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 07:13:38 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 07:13:39 GMT
EXPOSE 80
# Thu, 23 Jun 2022 07:13:39 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:08:17 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 23 Jun 2022 21:08:17 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 23 Jun 2022 21:08:18 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 23 Jun 2022 21:12:21 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:12:23 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 23 Jun 2022 21:12:24 GMT
VOLUME [/var/www/html]
# Thu, 23 Jun 2022 21:12:24 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 23 Jun 2022 21:21:34 GMT
ENV NEXTCLOUD_VERSION=24.0.2
# Thu, 23 Jun 2022 21:22:15 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:22:26 GMT
COPY multi:8757660dcec88b1946ba094c23fe14a1eb69054b1f7ddde5e16899421f67e84a in / 
# Thu, 23 Jun 2022 21:22:26 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Thu, 23 Jun 2022 21:22:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:22:27 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac3dc014d550bf03a1729b039a5f18fc36ee17be3dd0416bb30c3b4a7535c1`  
		Last Modified: Thu, 23 Jun 2022 07:57:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4014f31e7ed528e757a0a6304c23851740d7fc224ebc60a432fe29fcfe7d22d9`  
		Last Modified: Thu, 23 Jun 2022 07:57:10 GMT  
		Size: 71.6 MB (71623880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69abfac73dadc0771e03f979a0317fbbd77e330ec2249b29ff7fe9b1847a7c6`  
		Last Modified: Thu, 23 Jun 2022 07:57:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014e9e897ad90a6f2cbecd243c6e018071cc9a78e69f67c9e892838bbef15a81`  
		Last Modified: Thu, 23 Jun 2022 07:57:32 GMT  
		Size: 19.1 MB (19054112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4492c9a8a2c77ca48c14e62987ec0fc0b3573579e7d455dc858cb5ad2d5169`  
		Last Modified: Thu, 23 Jun 2022 07:57:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4ba43a64c6ee653983ae6f12df6c17d00ed6166714e72d992b4dbfe171291a`  
		Last Modified: Thu, 23 Jun 2022 07:57:30 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4201b04cd204488a63d4449e9234c6243f0ebc837a17c3e0b87c6f189e5502a7`  
		Last Modified: Thu, 23 Jun 2022 08:03:32 GMT  
		Size: 11.2 MB (11217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c37df5ef66cd1f8f79dbf5708c6076a44058619fde299d9237043e12f08fc1`  
		Last Modified: Thu, 23 Jun 2022 08:03:30 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f0126f6efc9de21ef63bf414daaf1b1d9e3ffa3b4953d16678c3081f2385df`  
		Last Modified: Thu, 23 Jun 2022 08:03:31 GMT  
		Size: 9.9 MB (9922672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b77afd4cd7710152e804fed993f8159208ca2fb447d5ce0b8d8538fb210bf3`  
		Last Modified: Thu, 23 Jun 2022 08:03:30 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bfc6eb20a5e4634b7d53b33c22a3b4f83f0645851f7f92c9461b3d04163113`  
		Last Modified: Thu, 23 Jun 2022 08:03:30 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2150d45fd5c49ef1bb2e72c0235bc3934d3b49709d5c37dc64da9b479d6c1b78`  
		Last Modified: Thu, 23 Jun 2022 08:03:30 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48de01ad8fbb90a7a091441f72f462652e0d77a06f442916014a980c3cd4f555`  
		Last Modified: Thu, 23 Jun 2022 21:26:04 GMT  
		Size: 1.7 MB (1659563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505074395f62bb4019c2a709fc367cd60ee756322f4d48a78bc44b14b9f57740`  
		Last Modified: Thu, 23 Jun 2022 21:26:06 GMT  
		Size: 15.1 MB (15052676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b92b18b15dea6d46209fe2a81f898c602e45f0bc78a47d081b73c390272cf1`  
		Last Modified: Thu, 23 Jun 2022 21:26:02 GMT  
		Size: 599.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1461643ccd272f9f07ced7ff4b94832b10c69152fca56aa8b10a5fca0654142`  
		Last Modified: Thu, 23 Jun 2022 21:26:02 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6795769dd18f6d059c4e835b39d4b71f5a066f51b19811e5173b945121f4f1bf`  
		Last Modified: Thu, 23 Jun 2022 21:28:46 GMT  
		Size: 134.2 MB (134172268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ad1af90dcef47c9fed284a5daff904ee996324a960f03d389cd458383a2dc`  
		Last Modified: Thu, 23 Jun 2022 21:28:32 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ea51dda0efac31afe5ea73d14e6bc94f28cb3887e24c56ea13a14211efa2bc`  
		Last Modified: Thu, 23 Jun 2022 21:28:32 GMT  
		Size: 2.2 KB (2199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
