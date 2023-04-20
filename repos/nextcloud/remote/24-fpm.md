## `nextcloud:24-fpm`

```console
$ docker pull nextcloud@sha256:cf1010dd1ee30a85bbdcd89ce7acc4793a651e705fe54d863105cd3aa28de7ef
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

### `nextcloud:24-fpm` - linux; amd64

```console
$ docker pull nextcloud@sha256:323d02a6483c0b656d0b08d124a6e9c02cec8e4244b3a9eee660809a6b440638
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.1 MB (319135296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0e8a299000d75daf25776af10515d3ce0c8686dd90a6e2eb469469e8698180`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:30:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:30:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:31:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:31:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:31:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:31:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:31:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:31:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 05:16:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 05:16:51 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 05:16:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 05:16:51 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 05:17:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 05:17:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:25:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 05:25:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:25:55 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 05:25:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 05:25:55 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 05:25:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 05:25:55 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 05:25:55 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 05:25:55 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 13:17:06 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 12 Apr 2023 13:17:06 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 12 Apr 2023 13:17:06 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 12 Apr 2023 13:19:31 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 13:19:32 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 12 Apr 2023 13:19:32 GMT
VOLUME [/var/www/html]
# Thu, 20 Apr 2023 20:32:26 GMT
ENV NEXTCLOUD_VERSION=24.0.12
# Thu, 20 Apr 2023 20:33:09 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 20:33:11 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Thu, 20 Apr 2023 20:33:11 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Thu, 20 Apr 2023 20:33:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Apr 2023 20:33:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c8021d1258ac2078c39a88a97b3c834df2a1bf40f1b56f88bb237cc837c9cb`  
		Last Modified: Wed, 12 Apr 2023 05:43:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff43c2de6846ddda72bd88d8150e2bb08bca320f1f8ff895a2c09afae223ecb`  
		Last Modified: Wed, 12 Apr 2023 05:43:13 GMT  
		Size: 91.6 MB (91636376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383987c505e89f10b4ef0b1352d7b5e1337ed05746b6e846e0760340080ea1b3`  
		Last Modified: Wed, 12 Apr 2023 05:43:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406de4d879c89f29f320a5320a9cc8a227337ca7555fb2e311ee7ccd65fd3792`  
		Last Modified: Wed, 12 Apr 2023 05:53:08 GMT  
		Size: 11.1 MB (11120681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dcc67dfe07e8b1e767981726e7ac26a240ff3b8dc6d8da026c445f097f316b`  
		Last Modified: Wed, 12 Apr 2023 05:53:07 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e45d818b3faa70d0ed6a780db6743278e6fcc658ca9042b110ed122ddede7`  
		Last Modified: Wed, 12 Apr 2023 05:53:50 GMT  
		Size: 26.0 MB (25968957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d846857621ad0de7209be9a1521e28523765d86c256d8af9ee67ca18a2d05f`  
		Last Modified: Wed, 12 Apr 2023 05:53:46 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb7a9093340e7eaf2ea422463c33f12caa63dcc1fb44befe06b4f4d90da67aa`  
		Last Modified: Wed, 12 Apr 2023 05:53:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d27dd943da5b6964a9eaef40e8a0b81fa3848a427eb6ee27834e46b3f98cf0c`  
		Last Modified: Wed, 12 Apr 2023 05:53:46 GMT  
		Size: 8.7 KB (8716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e8293dbb1dfc65b1d7fe9b2872441e1619f997cf43e839d965a795e9537554`  
		Last Modified: Wed, 12 Apr 2023 13:36:08 GMT  
		Size: 19.5 MB (19482094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba70a296080be2bf7433f5c8c9ff04451c2ba8a0f127f8c267f9725fd35f0ca`  
		Last Modified: Wed, 12 Apr 2023 13:36:04 GMT  
		Size: 4.2 MB (4159017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e955fb4ce678d9a85761397f8d300b5ff771937599a6504dd0d6b9831213a3d`  
		Last Modified: Wed, 12 Apr 2023 13:36:03 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0afb75c847e2850b5710f59bc25ff32305138ec543a29446a389d640cf27ad`  
		Last Modified: Thu, 20 Apr 2023 20:41:05 GMT  
		Size: 135.3 MB (135331652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e5b693a324852f26bb8acdb4dc07037a182d744690a115e60fc6cb9a239b1a`  
		Last Modified: Thu, 20 Apr 2023 20:40:50 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8b277b3707dd8c7bddbc1830f7f1885878825ac5f87538e20214da87f3f75`  
		Last Modified: Thu, 20 Apr 2023 20:40:50 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:7925450622d42d92e695419a9217bebe1887584fd2f7d9fee6f0f07898b8e497
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.7 MB (294652656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91624aacbe2bd9bab40b130becbc3629e3f642f640bbe45a68a989b2f4a7251c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:41 GMT
ADD file:11004b5308adcb1c41526eac7071d373a5c42ca2e457a2e9e8b3a9d621c4e8e1 in / 
# Wed, 12 Apr 2023 00:48:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:14:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 04:14:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 04:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 04:14:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:58:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 04:58:23 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 04:58:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 04:58:24 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 04:58:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:58:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:05:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 05:05:57 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:05:57 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 05:05:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 05:05:57 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 05:05:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 05:05:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 05:05:58 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 05:05:58 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 11:30:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 12 Apr 2023 11:30:45 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 12 Apr 2023 11:30:46 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 12 Apr 2023 11:32:57 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 11:32:57 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 12 Apr 2023 11:32:57 GMT
VOLUME [/var/www/html]
# Thu, 20 Apr 2023 20:50:52 GMT
ENV NEXTCLOUD_VERSION=24.0.12
# Thu, 20 Apr 2023 20:51:43 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 20:51:50 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Thu, 20 Apr 2023 20:51:50 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Thu, 20 Apr 2023 20:51:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Apr 2023 20:51:50 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5303309ebdb5d711447ed8a4ea072653ca7445c193060ec0aea30a89e92cda7e`  
		Last Modified: Wed, 12 Apr 2023 00:51:08 GMT  
		Size: 28.9 MB (28919551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b601dbf5623210200f12d1f8e2e0552f6306d5639c93397539b152544aae65`  
		Last Modified: Wed, 12 Apr 2023 05:09:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7fb2dad31be9edbd83b355c9c7edbbf4f2f8b078a83439e616a55be13d231`  
		Last Modified: Wed, 12 Apr 2023 05:09:17 GMT  
		Size: 73.7 MB (73685610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885a71e0c8784871a05569a5c7ff2475817a34a695add893444c1a4256a277e6`  
		Last Modified: Wed, 12 Apr 2023 05:09:04 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ed2a41109f0da318b4307add20303559b2bd0e15b37bc7d434a85f87e75598`  
		Last Modified: Wed, 12 Apr 2023 05:14:47 GMT  
		Size: 11.1 MB (11118835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de111c73c4c70bb4645ac2f838828e25078db1f49cd9b4e55fefeb3b8a1b5805`  
		Last Modified: Wed, 12 Apr 2023 05:14:46 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9d853e00c33c3ae11d7fb5bd3ef6cac93a11e6261049d2ca09b257781aa601`  
		Last Modified: Wed, 12 Apr 2023 05:15:35 GMT  
		Size: 24.5 MB (24548505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10017170beac339d0c42e995c923de8c06863c13d4b61f44a1e64d5e3c467d8`  
		Last Modified: Wed, 12 Apr 2023 05:15:31 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df3eee10ecb83d022b1882dc5bd42709c416a19f8eb0106dea13a34c91c3f8b`  
		Last Modified: Wed, 12 Apr 2023 05:15:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f85ad547b7bc7af84b1a51a95e8aeacd12e9e7092c061b3a3e51db74c6b62a0`  
		Last Modified: Wed, 12 Apr 2023 05:15:31 GMT  
		Size: 8.7 KB (8716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2184ffd3715821756de8ecef0569b3d30564eecf8c7f7e78be567e48f220f946`  
		Last Modified: Wed, 12 Apr 2023 11:48:56 GMT  
		Size: 17.4 MB (17427044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a86a1ca5b86744c7501622fc7edbdfc1c6c5eb546c789d50807e46d41362cd`  
		Last Modified: Wed, 12 Apr 2023 11:48:53 GMT  
		Size: 3.6 MB (3604877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317172de58330e123752d8f04c48b6a860873cd3557e8c80e1f02faa29d91a3`  
		Last Modified: Wed, 12 Apr 2023 11:48:52 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d81e21334fb5db5399acd3716e8a833ba6b88e3fd0c7647f0ff7d68b7bc67e`  
		Last Modified: Thu, 20 Apr 2023 20:58:39 GMT  
		Size: 135.3 MB (135329933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2c8c162710ea05865a42af9b55c9a927f37d51c10f124744d6f40c18d2361d`  
		Last Modified: Thu, 20 Apr 2023 20:58:06 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8a373cdbde9049f753aae65df30f680c7dfd94e779acf73b0a8a784c90972f`  
		Last Modified: Thu, 20 Apr 2023 20:58:06 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:c9e2d4d48b1e8e869713a939bd7515a406d791f8b96cc5efcfcb96ebc8ffa05d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.4 MB (285448343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9bfcd81dc8d443a611277792e55541540244b5f9a93b39d5522b654d556ab0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:35:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:35:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:35:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:35:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 02:35:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:35:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:35:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:06:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 04:06:27 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 04:06:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 04:06:27 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 04:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:06:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:13:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 04:13:14 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:13:14 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 04:13:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 04:13:15 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 04:13:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 04:13:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 04:13:15 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 04:13:15 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 11:57:42 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 12 Apr 2023 11:57:43 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 12 Apr 2023 11:57:43 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 12 Apr 2023 11:59:45 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 11:59:45 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 12 Apr 2023 11:59:46 GMT
VOLUME [/var/www/html]
# Wed, 12 Apr 2023 11:59:46 GMT
ENV NEXTCLOUD_VERSION=24.0.11
# Wed, 12 Apr 2023 12:00:53 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 12:00:57 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Wed, 12 Apr 2023 12:00:57 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Wed, 12 Apr 2023 12:00:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 12:00:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4c3fcca6db962fb49617da5ac21af2abd9525daf0f8e86ce71084de6803ea`  
		Last Modified: Wed, 12 Apr 2023 04:28:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f5e561d5b9a35f200f2b1559ae811ad4ce71d740a69aea8c443d39a7fdba7`  
		Last Modified: Wed, 12 Apr 2023 04:28:17 GMT  
		Size: 69.3 MB (69321908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a726bf573f3daeb69abfd49bd12ad0bd1e6359d8f5cc041c41666d11884385`  
		Last Modified: Wed, 12 Apr 2023 04:28:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f103be272b0d1e21008dbc7649bb6e607d69a017f8978a5c8f445c7441504ba`  
		Last Modified: Wed, 12 Apr 2023 04:38:11 GMT  
		Size: 11.1 MB (11118868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0034ad8b60355db430dc9ce3621ebd9f468bb4dde54e6d6c9b227b62a39a5`  
		Last Modified: Wed, 12 Apr 2023 04:38:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91116fdd38dbf91516c08915a6f8a6ee6413b11c7486d9c09da06aca3945f35e`  
		Last Modified: Wed, 12 Apr 2023 04:38:54 GMT  
		Size: 23.8 MB (23754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4ac54b72fe29a98ba50b47e7252822e61ce2fb218bc5e42e3c6971c2d39747`  
		Last Modified: Wed, 12 Apr 2023 04:38:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98916418f0b0a8604b5c9a8a2ff047f41e0b9a4d0fd9c3f67ca27bf4c8010176`  
		Last Modified: Wed, 12 Apr 2023 04:38:50 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a195249043b27ab98f9e9ca24c0b62539dc93be3c56d37c76a25bccfeaf024f`  
		Last Modified: Wed, 12 Apr 2023 04:38:50 GMT  
		Size: 8.7 KB (8718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff4351b857d81b1d5ae7577d91b910a0a53a2e0103be12a3efd20836e71ecf`  
		Last Modified: Wed, 12 Apr 2023 12:15:15 GMT  
		Size: 15.9 MB (15869171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbceb4cb39c287fcb13fe2577416787b4bdae93db4d323637a2215f247c3867`  
		Last Modified: Wed, 12 Apr 2023 12:15:12 GMT  
		Size: 3.5 MB (3487435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9224471720b4150a69f52f2b73751d5dc40c7130a8f57074556986c6c0f748`  
		Last Modified: Wed, 12 Apr 2023 12:15:11 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff663a733d019bec0f9b4358c2918e7b5879b8af6b27e102e4bab0733944c1a`  
		Last Modified: Wed, 12 Apr 2023 12:15:35 GMT  
		Size: 135.3 MB (135298534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd06fc34d51cac7365cb614f901c878f2fa11c249c66d48361a6902c019d7e`  
		Last Modified: Wed, 12 Apr 2023 12:15:11 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292e36d019bce6f841d930f0b4bd7b884cd6e8f8961416bc6e3b4ad5d4f7fc50`  
		Last Modified: Wed, 12 Apr 2023 12:15:11 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:8e8b5978b78fd7ab05ac084338ea2a7156a7d60fb4189aa27780e120a233a7da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309774302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87342aabe4ea0f846b5c281d2248251323d0504d38258e65e4f46815d0ce048b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:57:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 07:57:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 07:57:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:57:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 07:57:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 07:58:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 07:58:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 07:58:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 09:35:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 09:35:07 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 09:35:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 09:35:07 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 09:35:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 09:35:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:41:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 09:41:30 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:41:31 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 09:41:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 09:41:31 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 09:41:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 09:41:31 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 09:41:31 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 09:41:31 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 16:50:09 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 12 Apr 2023 16:50:10 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 12 Apr 2023 16:50:10 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 12 Apr 2023 16:51:59 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 16:52:00 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 12 Apr 2023 16:52:00 GMT
VOLUME [/var/www/html]
# Wed, 12 Apr 2023 16:52:00 GMT
ENV NEXTCLOUD_VERSION=24.0.11
# Wed, 12 Apr 2023 16:52:39 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 16:52:42 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Wed, 12 Apr 2023 16:52:42 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Wed, 12 Apr 2023 16:52:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 16:52:42 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f2f210bdf0abad378762a728c4debd95e91b2c1b0972f1343a00fb2b4de7d5`  
		Last Modified: Wed, 12 Apr 2023 09:54:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94128402988c00cfbe7df969124206ced4768288b775ea18ecfe8d2fd9af8d6`  
		Last Modified: Wed, 12 Apr 2023 09:54:28 GMT  
		Size: 86.9 MB (86928989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c1987c00542c8d723ebae9238f853a76f0c093fe230959d6434d031917246c`  
		Last Modified: Wed, 12 Apr 2023 09:54:19 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d2328668db9ea0ea964a4665dde2303232a32be7739c3bd528769c47f7553b`  
		Last Modified: Wed, 12 Apr 2023 10:04:07 GMT  
		Size: 11.1 MB (11119874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b209cbbae5ab651521bb675ed4042a151633d82f0901e9379c5eb33ca8e247`  
		Last Modified: Wed, 12 Apr 2023 10:04:06 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b23ca6870a64489c24f80f935462e3d6c260c1a29e4e8e6dc3a2d705cb7b65`  
		Last Modified: Wed, 12 Apr 2023 10:04:47 GMT  
		Size: 25.4 MB (25395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6953692ffe544356176bfec9ddd0d96b32b57d0a1d317b55424b9ae02c011`  
		Last Modified: Wed, 12 Apr 2023 10:04:44 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4d2ce864bc5d2b1bd920a2aa703af60cf87e7e37235f1d8dae4dd51023e5a7`  
		Last Modified: Wed, 12 Apr 2023 10:04:44 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499212015f6735da3e3d6c6754d96bdea985230f47d62be74b76656d97f11734`  
		Last Modified: Wed, 12 Apr 2023 10:04:44 GMT  
		Size: 8.7 KB (8720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f27a02314a3bb20f4054093a2023c1655e58d662ffd1c6287aa5c0817ae0522`  
		Last Modified: Wed, 12 Apr 2023 17:08:35 GMT  
		Size: 17.2 MB (17187897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbd7023b11ac98e850aa6729bd8db5718a6f4091d4a1b85680a89470024f0b1`  
		Last Modified: Wed, 12 Apr 2023 17:08:33 GMT  
		Size: 3.8 MB (3760379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0fdb68624f9e81b99003e897fd8f8e1e15048f52ebb704bf442ee888c34838`  
		Last Modified: Wed, 12 Apr 2023 17:08:32 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545557e694fac5048a243a0dd871061ff7b8b7a091bee0c65dcc551734ec47f5`  
		Last Modified: Wed, 12 Apr 2023 17:08:45 GMT  
		Size: 135.3 MB (135300040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b9dece13069523ab73aa8f6716b064c9ac36c4cefc6472bb9153fd3becc6fa`  
		Last Modified: Wed, 12 Apr 2023 17:08:32 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e664c404c7b665e5112017d38e4329a3c9e5acd61b7f04d2b87efd79ed6d027f`  
		Last Modified: Wed, 12 Apr 2023 17:08:32 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; 386

```console
$ docker pull nextcloud@sha256:4475832ef7efc8bd0a9e173981ef0fe634400d9ffd7aa34a9b750773941b1e87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321206384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:def1f1e1394b506be68fe5dbd98fd6beb895f099e9519dd2f954c30e318685fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:10:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 05:10:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 05:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:10:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 05:10:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 05:10:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:10:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:10:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 08:00:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 08:00:19 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 08:00:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 08:00:20 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 08:00:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 08:00:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:15:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 08:15:33 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:15:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 08:15:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 08:15:34 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 08:15:35 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 08:15:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 08:15:35 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 08:15:35 GMT
CMD ["php-fpm"]
# Thu, 13 Apr 2023 00:46:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 13 Apr 2023 00:46:45 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 13 Apr 2023 00:46:45 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 13 Apr 2023 00:49:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 13 Apr 2023 00:49:38 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 13 Apr 2023 00:49:38 GMT
VOLUME [/var/www/html]
# Thu, 20 Apr 2023 20:41:32 GMT
ENV NEXTCLOUD_VERSION=24.0.12
# Thu, 20 Apr 2023 20:42:21 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 20:42:23 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Thu, 20 Apr 2023 20:42:24 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Thu, 20 Apr 2023 20:42:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Apr 2023 20:42:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c63f93493e2a7820d4f2332775c7575bc5ab3d2358b167eadf787455f1f0410`  
		Last Modified: Wed, 12 Apr 2023 08:42:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf8627b0cb08594b65741f86baf83146a59f931e067c980b9b9cbf93b9dae7f`  
		Last Modified: Wed, 12 Apr 2023 08:42:44 GMT  
		Size: 92.7 MB (92720432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef01aa4975c4bb966cd891dd1e9ed26a36289e162af712fae5029523ceba1da2`  
		Last Modified: Wed, 12 Apr 2023 08:42:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b3cc5fae422f164234e0ba4169ac073036ea5e6b2fbf1b2668580506d98df`  
		Last Modified: Wed, 12 Apr 2023 08:53:31 GMT  
		Size: 11.1 MB (11119779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75226724100c86cdb15a3796562a2049b61235a987d8e2e1f7fffd764296393e`  
		Last Modified: Wed, 12 Apr 2023 08:53:30 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e39ca2cf5f5eb6ffca900b7a1c8eff6884f728e2b050cb70aeda77dbd65dcf3`  
		Last Modified: Wed, 12 Apr 2023 08:54:19 GMT  
		Size: 26.4 MB (26422175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e0b93349f4fe3fe6b74ff288200d896d42d80a82c3ed22f47c0f27578560bb`  
		Last Modified: Wed, 12 Apr 2023 08:54:13 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d83c3479b4b10becd3991d2029be4aa3a36078b3f9208d0fb5368fb49bfc57`  
		Last Modified: Wed, 12 Apr 2023 08:54:14 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0efa08eaaaf10df03cdd17572b99d1630a19dd54937018235ce99e00554a079`  
		Last Modified: Wed, 12 Apr 2023 08:54:13 GMT  
		Size: 8.7 KB (8719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1badc99ba206bea394b504f8396c9e14f6fecd9bd06f4bb3b926ea3817691e`  
		Last Modified: Thu, 13 Apr 2023 01:08:38 GMT  
		Size: 19.1 MB (19085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146d183fc717f3c73552a2f48be875ac43bc6f4a7ba7e4134d59a3409b54174b`  
		Last Modified: Thu, 13 Apr 2023 01:08:33 GMT  
		Size: 4.1 MB (4109707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe9859ff63e5405092327c89b5d273a1da79a1af880572642a5beecf66e6894`  
		Last Modified: Thu, 13 Apr 2023 01:08:32 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4dd7611ccb16e3f2079f4919ce47fd8ecfee1d6c632aad7fdba5cd66567f0a`  
		Last Modified: Thu, 20 Apr 2023 20:52:07 GMT  
		Size: 135.3 MB (135331076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc03e48091d14f9b71d98955357ac5f96985e924a05562e11fd73a5ae742fd25`  
		Last Modified: Thu, 20 Apr 2023 20:51:44 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb599b9ee437738028322c4e6eb8753393ad6b8d93c6dc46fcd31c64090ecd7`  
		Last Modified: Thu, 20 Apr 2023 20:51:44 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; mips64le

```console
$ docker pull nextcloud@sha256:c674cc8032c9ee2640b4e87171bba0e6e3d197e62d289f394318fa4328ab73da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.4 MB (293414010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06fda5de0478885d314862458076f084a9b0bb12d34004aed8ba946ad77b31ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:59 GMT
ADD file:2f558bb3cf4bc685f98fcdb12200961e3059267213f0caf7686523305967a663 in / 
# Wed, 12 Apr 2023 00:10:03 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 17:40:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 17:40:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 17:41:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 17:41:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 17:41:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 17:41:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 17:41:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 17:42:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 21:33:52 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 21:33:55 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 21:33:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 21:34:02 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 21:34:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 21:34:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 22:16:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 22:16:26 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 22:16:32 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 22:16:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 22:16:39 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 22:16:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 22:16:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 22:16:53 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 22:16:57 GMT
CMD ["php-fpm"]
# Thu, 13 Apr 2023 10:15:14 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 13 Apr 2023 10:15:18 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 13 Apr 2023 10:15:22 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 13 Apr 2023 10:26:34 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 13 Apr 2023 10:26:41 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 13 Apr 2023 10:26:45 GMT
VOLUME [/var/www/html]
# Thu, 13 Apr 2023 10:26:49 GMT
ENV NEXTCLOUD_VERSION=24.0.11
# Thu, 13 Apr 2023 10:29:26 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 13 Apr 2023 10:29:37 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Thu, 13 Apr 2023 10:29:45 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Thu, 13 Apr 2023 10:29:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 13 Apr 2023 10:30:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8b0f62b0d33641c5348fd31abfd06463bdc4213a072d71479a0765756673777b`  
		Last Modified: Wed, 12 Apr 2023 00:17:28 GMT  
		Size: 29.6 MB (29639206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a69bb16c3f89448ac4380e4a6c9d78eeddcaa3c300324594dd6e2e4cf02617`  
		Last Modified: Wed, 12 Apr 2023 22:31:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92516d65e1f532cbcef2ec02722c2d8bfbe523ae63a6e14f136fad8253bf69e`  
		Last Modified: Wed, 12 Apr 2023 22:32:08 GMT  
		Size: 72.0 MB (72018898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16f0df3f45b7f1adec8d38deb8031c5e01c12d046bf66f6d1b198ad3718dd5f`  
		Last Modified: Wed, 12 Apr 2023 22:31:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e623238c7c163f18a5d4d1486ef8fe283747dcc16f1393cdbd2a9c851a2fa04`  
		Last Modified: Wed, 12 Apr 2023 22:41:22 GMT  
		Size: 10.9 MB (10903219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006439a796ef2e4f0d29e59864f1a055c0af28d73598ab1873c79afd3b631732`  
		Last Modified: Wed, 12 Apr 2023 22:41:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe0689625d048a1f5ce7bf226e2cdededde5e664b35541a695e5be1eba56fa1`  
		Last Modified: Wed, 12 Apr 2023 22:42:42 GMT  
		Size: 25.0 MB (24959633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51970ef1625fd7716263b0bc78571203128dc16dd21de325a912f589f0cb625`  
		Last Modified: Wed, 12 Apr 2023 22:42:27 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fdc04a262d22a2e937b7707919c92710368b082f93b2556e00a9aa4d2beb35`  
		Last Modified: Wed, 12 Apr 2023 22:42:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c48ce0d6b779110533033a2b202df2c7beef9717e1ad5aa5f3220b05096e02c`  
		Last Modified: Wed, 12 Apr 2023 22:42:27 GMT  
		Size: 8.7 KB (8721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0f7b7200d627b774c7a0952d9e3c912588a656eb0e0b4e7946c6243b8162d9`  
		Last Modified: Thu, 13 Apr 2023 11:35:52 GMT  
		Size: 17.3 MB (17311957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d03d4451586d4a91777b1890b38b14a1cf4ec23732ad60afb2db16ee10d32b`  
		Last Modified: Thu, 13 Apr 2023 11:35:42 GMT  
		Size: 3.5 MB (3500113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42853242f6b7b024ffbd695425fc394207c39b2579cdba759b291d99860b9c5a`  
		Last Modified: Thu, 13 Apr 2023 11:35:34 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70a1ffc9417754bee494f3b894e1dff2294625f472484d93d5401530136f80e`  
		Last Modified: Thu, 13 Apr 2023 11:37:05 GMT  
		Size: 135.1 MB (135062760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3325dc08533e13199bf4dcbf217fe39fab709d345f4475ebbaf6b0cbcd5c6ed9`  
		Last Modified: Thu, 13 Apr 2023 11:35:34 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2782c08de4fafef76a1114359ce088dab8a1ae218a9ad5afbd505df992bd2b2`  
		Last Modified: Thu, 13 Apr 2023 11:35:35 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:52b43d5ce7ff9f3c8011aa1eb40d9e8096b28d154e122a5d0f7d78700e134ff3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.0 MB (319037829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca0db11cc75985f75ed4c06e11867597d18ab61abaa42efe100cbfcf0040d107`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:53:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:53:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:54:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:55:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:55:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 02:55:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:55:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:55:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:25:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 04:25:02 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 04:25:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 04:25:08 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 04:26:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:26:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:44:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 04:44:11 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:44:15 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 04:44:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 04:44:17 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 04:44:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 04:44:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 04:44:25 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 04:44:29 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 13:49:35 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 12 Apr 2023 13:49:36 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 12 Apr 2023 13:49:36 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 12 Apr 2023 13:54:18 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 13:54:20 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 12 Apr 2023 13:54:20 GMT
VOLUME [/var/www/html]
# Thu, 20 Apr 2023 20:22:30 GMT
ENV NEXTCLOUD_VERSION=24.0.12
# Thu, 20 Apr 2023 20:23:56 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 20:24:01 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Thu, 20 Apr 2023 20:24:02 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Thu, 20 Apr 2023 20:24:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Apr 2023 20:24:03 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881dab4e16a2b31707f063b4a6d06a7622c29a571e9941b45d4f1dbab9fa535`  
		Last Modified: Wed, 12 Apr 2023 04:52:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7112207942602cdd0c4444cb2cf85085ac4ac494a4140f7ad0d4b40bc5d9af2`  
		Last Modified: Wed, 12 Apr 2023 04:53:17 GMT  
		Size: 86.6 MB (86633054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc8a1d48af817593b6b8be59cd4822dcbbf90138a02afc42d1c359a66cef044`  
		Last Modified: Wed, 12 Apr 2023 04:52:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35c77dceaae566ac4c426441d2af502a6355f7e7614eb4bf9afddea724f55c`  
		Last Modified: Wed, 12 Apr 2023 05:00:46 GMT  
		Size: 11.1 MB (11120752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478160b2f40212221ba5c233ef00d5b8a5b46ebe512c394f0c260369ca806ea7`  
		Last Modified: Wed, 12 Apr 2023 05:00:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9904f6ad6f7ab63b274bbe92b6e42d010aa4ffa4e03e897c76c4beb9baeb6ba2`  
		Last Modified: Wed, 12 Apr 2023 05:01:42 GMT  
		Size: 27.0 MB (26960275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81ff53af54bf23627c53c0ffbfd5b5946179f4cb71c8269cfd2e565ac94a37f`  
		Last Modified: Wed, 12 Apr 2023 05:01:36 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd7394df63feb751ffb796aaf5234cf3edd271ef799f6a5e0bab42c2a1be270`  
		Last Modified: Wed, 12 Apr 2023 05:01:36 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b1d1d669746b409d453f3469a65863ae4f6b5a5ed716b92640239e8b0a7094`  
		Last Modified: Wed, 12 Apr 2023 05:01:36 GMT  
		Size: 8.7 KB (8720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa43ad598ebf87f5b1c4c4e98d0c34e3a62321c4a779bb2a64b7439afd0a9d0a`  
		Last Modified: Wed, 12 Apr 2023 14:25:42 GMT  
		Size: 19.7 MB (19664001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f931c46ead9f3f0061e84f8e6cdaf5c7b4162b0ddb5a9ec9451dc510b5e4b8b9`  
		Last Modified: Wed, 12 Apr 2023 14:25:37 GMT  
		Size: 4.0 MB (4016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa1d9cd156ad7c411b31e0ba9e2c403e29d745135ce9fe0d42a2b9d45d54002`  
		Last Modified: Wed, 12 Apr 2023 14:25:35 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e5b662b360c0defaac0e51693cf33fd7cc22666dfe89cec56a765cc5ce71a1`  
		Last Modified: Thu, 20 Apr 2023 20:37:25 GMT  
		Size: 135.3 MB (135332455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafd09b8689d1943d488b945e7074e5693d8dff8e61158640779b7cdda2d62f0`  
		Last Modified: Thu, 20 Apr 2023 20:36:54 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de34c341cb3b4c55fbcff177705060d05e2edbd325cca6c6804072cba89cdce2`  
		Last Modified: Thu, 20 Apr 2023 20:36:54 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:24-fpm` - linux; s390x

```console
$ docker pull nextcloud@sha256:ca0df6bc6a98f7a39604b195f90c1ac6a17fc0d2e763d21117b74d2901b67b50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293743081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61a49ae1d3fcc23a82a31d00ad17262d9ccfd17192e99b263952721afaae289a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:36:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:36:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:37:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:37:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:37:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:37:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:37:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:27:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 04:27:48 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 04:27:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 04:27:49 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 04:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:27:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:35:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 04:35:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:35:35 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 04:35:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 04:35:35 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 04:35:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 04:35:36 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 04:35:36 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 04:35:36 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 12:54:38 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 12 Apr 2023 12:54:39 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 12 Apr 2023 12:54:39 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 12 Apr 2023 12:57:59 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 12:58:01 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 12 Apr 2023 12:58:01 GMT
VOLUME [/var/www/html]
# Thu, 20 Apr 2023 20:45:02 GMT
ENV NEXTCLOUD_VERSION=24.0.12
# Thu, 20 Apr 2023 20:45:39 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 20 Apr 2023 20:45:45 GMT
COPY multi:38a4739a7ce38db03075117346fff2453db5ff29d27e30f506b9d2fc6a4b4a9a in / 
# Thu, 20 Apr 2023 20:45:46 GMT
COPY multi:1aa0c68034f207c7e2fb6f047fda45b55878afe2781ef10723107e35ee22547e in /usr/src/nextcloud/config/ 
# Thu, 20 Apr 2023 20:45:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Apr 2023 20:45:46 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e763db148606393f8c21697bc30f68ac8de11269141ae6e0d5e8483fe3e26`  
		Last Modified: Wed, 12 Apr 2023 04:40:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f8d95603c0d1c5673103183c025b2e49c72c82f4e8b4b3a86201eb804e7ffa`  
		Last Modified: Wed, 12 Apr 2023 04:40:55 GMT  
		Size: 71.6 MB (71629155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e864c428fd73e9e002327cf91695b364814ad36e7552a314e87ab897ca522f`  
		Last Modified: Wed, 12 Apr 2023 04:40:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b095abf32ac6be9c1b85c4da3999e48f8d01fce5b6f40490d89e2331b76ce65`  
		Last Modified: Wed, 12 Apr 2023 04:45:07 GMT  
		Size: 11.1 MB (11119350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd12f072d018b191ff4e63f287ef2ea3ef49c658770e1e3624040a5b8f896034`  
		Last Modified: Wed, 12 Apr 2023 04:45:07 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9715284724925af0b33b1021ba12f6c43f1334aeb59414cac52b30b9de45d64d`  
		Last Modified: Wed, 12 Apr 2023 04:45:34 GMT  
		Size: 25.0 MB (25040843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677293cc8baf95c76f53f3fc33ab78899f091615292b6f661c79bd33193a6e0`  
		Last Modified: Wed, 12 Apr 2023 04:45:31 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8452e696f434ff6c8d57d44953b040a9c1be0571979fb15f16e367ba06c074`  
		Last Modified: Wed, 12 Apr 2023 04:45:31 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f7e38719fb699533aeeb990501ce709043b88783f2190fee8096e366baec10`  
		Last Modified: Wed, 12 Apr 2023 04:45:31 GMT  
		Size: 8.7 KB (8714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9df6efac24fc558f7d6642b29840562c0163c1347fdca352e01d2b1531ea6f`  
		Last Modified: Wed, 12 Apr 2023 13:12:17 GMT  
		Size: 17.2 MB (17163650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb7fa4bbad9905ec183fb021b882709608b3cb6a261252c8d2095d69aa047aa`  
		Last Modified: Wed, 12 Apr 2023 13:12:14 GMT  
		Size: 3.8 MB (3787754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c78775b191d6156064e113d862a70fc06bafadef9e1de5d38c2f66c8b5b6249`  
		Last Modified: Wed, 12 Apr 2023 13:12:14 GMT  
		Size: 607.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c45cd9e16394744947adcbcccd35bc5e6580f7341dff4e0508ee2ae9ce3eae`  
		Last Modified: Thu, 20 Apr 2023 20:52:58 GMT  
		Size: 135.3 MB (135330899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef38456b3a25840ee3736778bccc26dc534b5e6d5595c10f2d822bb93e975506`  
		Last Modified: Thu, 20 Apr 2023 20:52:44 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095c2a374f78cbb3adbb770e12bb802f23856d9f0f5e8227ce9235a6154e6fb1`  
		Last Modified: Thu, 20 Apr 2023 20:52:44 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
