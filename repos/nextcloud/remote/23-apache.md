## `nextcloud:23-apache`

```console
$ docker pull nextcloud@sha256:5f113a006516e5e30ebf1aad527f6ba359737a3e41912b6419a8c23dd7bc3e87
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

### `nextcloud:23-apache` - linux; amd64

```console
$ docker pull nextcloud@sha256:3537d773f3beb3e4163fcc490d12285c4a1455f914b9015733780e9043d01da2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.7 MB (343737844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41ebddd8821ecaaff422dc20eeea35e3554e96ab665fd1be4a057f97535b5e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:33:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 18:33:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 18:34:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:34:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 18:34:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 18:37:50 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 18:37:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 18:38:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 18:38:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 18:38:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 18:38:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 18:38:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 18:38:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 19:31:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 19:31:13 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 19:31:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 19:31:14 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 19:31:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 19:31:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 19:34:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 19:34:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 19:34:21 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 19:34:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 19:34:21 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 19:34:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 19:34:21 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 19:34:21 GMT
EXPOSE 80
# Sat, 04 Feb 2023 19:34:22 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 04:18:54 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 05 Feb 2023 04:18:54 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 05 Feb 2023 04:18:54 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 05 Feb 2023 04:21:33 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 04:21:33 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 05 Feb 2023 04:21:33 GMT
VOLUME [/var/www/html]
# Sun, 05 Feb 2023 04:21:34 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 05 Feb 2023 04:21:34 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sun, 05 Feb 2023 04:22:23 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 04:22:25 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sun, 05 Feb 2023 04:22:25 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sun, 05 Feb 2023 04:22:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 04:22:25 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45244a9928d1453c90e25e75fdd7f2668b22f1fc895527554840b617b7622f3e`  
		Last Modified: Sat, 04 Feb 2023 19:56:34 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139d4815e950b14b9cc0609e63773573cf7f2e92f4fbfc156e3cc694b9c96a58`  
		Last Modified: Sat, 04 Feb 2023 19:56:47 GMT  
		Size: 91.6 MB (91636355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a420fd884ad456eee0071195987b9967e5083bb49c4696338f669c0cd2d1872`  
		Last Modified: Sat, 04 Feb 2023 19:56:33 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de46a46cfcd6274017e2674483b191d4fd0d0d9e93f9afd4e9a8c3186f2dda8`  
		Last Modified: Sat, 04 Feb 2023 19:57:32 GMT  
		Size: 19.2 MB (19244791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc46e699e97f5ba7b258113cc6a05902b2f80971d5bbcd8c88bd9eb3c41ecb3`  
		Last Modified: Sat, 04 Feb 2023 19:57:29 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d67ebc9db940d758cd7d7a318c77d6123e08ca0e2f474eb6abf2082a20276`  
		Last Modified: Sat, 04 Feb 2023 19:57:29 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59c438619152e3ef3419fe183b302f4007cf48a74c52ce3b6955ff65d2c5bf`  
		Last Modified: Sat, 04 Feb 2023 20:03:29 GMT  
		Size: 11.1 MB (11143399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9195cab71d030d866624b1f60021f6b1df81811a1bee6c83a328d75c6fffd87f`  
		Last Modified: Sat, 04 Feb 2023 20:03:26 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaa1559de60a885e54f0000ef77ce60730bff87061cd92ce29ac565cbe4db43`  
		Last Modified: Sat, 04 Feb 2023 20:03:28 GMT  
		Size: 10.8 MB (10775780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98ea42e90a6551568f0a57ba8524ae2d1ff34e6bf72bf756e4d975733b1dfa5`  
		Last Modified: Sat, 04 Feb 2023 20:03:26 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25586855c63469da8d96285421f448a963c96ca5ed0c8d0c16fa8117243fa96`  
		Last Modified: Sat, 04 Feb 2023 20:03:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c6d5ce99796deb62182fc678b3a9b9ec3e425c354c0b9beb402cb563373a1`  
		Last Modified: Sat, 04 Feb 2023 20:03:26 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f5feacbebd502cfe51a15d94a89e69909187a66b7380f28eb97c282ce4c736`  
		Last Modified: Sun, 05 Feb 2023 04:36:12 GMT  
		Size: 19.4 MB (19446574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4b40d83dcb38150d533869b5d7f60221f4ceea54339723780b6f046cbde1f2`  
		Last Modified: Sun, 05 Feb 2023 04:36:10 GMT  
		Size: 4.2 MB (4183459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eeb5e5f2b801d0768be792dc335c81064f1547174951faca11403655c97bb41`  
		Last Modified: Sun, 05 Feb 2023 04:36:07 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849f285eda13198fe7820aa23a766b47618d32ac97f695efb2b2af000545d30e`  
		Last Modified: Sun, 05 Feb 2023 04:36:07 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e4dff9d32e778d3161da3886ea886d4425ade37f70765d54fb25679f935cf4`  
		Last Modified: Sun, 05 Feb 2023 04:36:28 GMT  
		Size: 155.9 MB (155898365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360925ab6ebf5ba766e4a56385cc9a84ea8e421b44477e00aec821ea0339770e`  
		Last Modified: Sun, 05 Feb 2023 04:36:07 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac976a7943f600a5d3cf8963817b91f76dc29fe9e194d1c19f0e1a6f8a424382`  
		Last Modified: Sun, 05 Feb 2023 04:36:07 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:df1799dc2ede0a0fa45eb2883c0aec2b2f1405f4d4c03af8ab99f111e2bbe4ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.0 MB (319012049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2a4c0696b2afdde13d440bcd035700e0c279d1fc862ae9e2906d63b14949b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:38:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 06:38:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 06:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:38:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 06:38:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 06:41:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 06:41:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 06:42:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 06:42:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 06:42:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 06:42:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 06:42:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 06:42:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 07:09:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 07:09:10 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 07:09:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 07:09:10 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 07:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 07:09:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 07:12:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 07:12:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 07:12:29 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 07:12:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 07:12:30 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 07:12:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 07:12:30 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 07:12:30 GMT
EXPOSE 80
# Sat, 04 Feb 2023 07:12:30 GMT
CMD ["apache2-foreground"]
# Sat, 04 Feb 2023 14:58:18 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 04 Feb 2023 14:58:18 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 04 Feb 2023 14:58:18 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 04 Feb 2023 15:01:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 15:01:18 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 04 Feb 2023 15:01:18 GMT
VOLUME [/var/www/html]
# Sat, 04 Feb 2023 15:01:19 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sat, 04 Feb 2023 15:01:19 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sat, 04 Feb 2023 15:02:13 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 15:02:19 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 04 Feb 2023 15:02:19 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sat, 04 Feb 2023 15:02:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 15:02:19 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2a9a379621b51539531deb7a9f9a755c10b4a6dd3a3018e0566273c0729727`  
		Last Modified: Sat, 04 Feb 2023 07:21:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278d1ef4a15afc92d15698e1ca81abd95a0482f3d3e0d326d5ddddf34e8c66d9`  
		Last Modified: Sat, 04 Feb 2023 07:22:09 GMT  
		Size: 73.7 MB (73685555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997b7c9b51503e70b772520aaf1584c7ea8b08c3830c6cca94cf619dba11ae02`  
		Last Modified: Sat, 04 Feb 2023 07:21:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185a6662e25e9b1f0a4c6851a30b5d9716575dde915b3633fcf1e274c03d5417`  
		Last Modified: Sat, 04 Feb 2023 07:23:12 GMT  
		Size: 18.6 MB (18554319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fe23d51393f5c20ff2f080b817466291ee86095d367f2785f7b616aecfd5dc`  
		Last Modified: Sat, 04 Feb 2023 07:23:09 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6028a184b6703c79c9990dadd993c69312ea89eab6d2d957549b964fb72a8e42`  
		Last Modified: Sat, 04 Feb 2023 07:23:09 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de65b60ef3b7fa6d4ba20951eec51877516ff816550bcc2593f5bf03e27460f`  
		Last Modified: Sat, 04 Feb 2023 07:27:20 GMT  
		Size: 11.1 MB (11141842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a83bf2f50fb032fea43d03c09e9084bd875b550b76d19b87e292197a228553`  
		Last Modified: Sat, 04 Feb 2023 07:27:17 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265c73ca5ffa5db3797c600baf4fc5d5d392cad9a4afbef3c7502ea1547422f`  
		Last Modified: Sat, 04 Feb 2023 07:27:19 GMT  
		Size: 9.8 MB (9789731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69572f99425a735c1750dfc1804d65f3ed245826b0f54e90c87139bb6e85adbb`  
		Last Modified: Sat, 04 Feb 2023 07:27:17 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386bf913ade4e4bf3a171ef228054eeff126bbab68510b3125fba3df136c60fd`  
		Last Modified: Sat, 04 Feb 2023 07:27:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cc04ad1cb4d396ee320f3408ec6c5bc99fe144c72d405ccb112afb0e884dd`  
		Last Modified: Sat, 04 Feb 2023 07:27:17 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec5a75b4c573f7b1c5fb0209104db61d9a9282df7cba8f5d7dbfe1fd873486c`  
		Last Modified: Sat, 04 Feb 2023 15:18:50 GMT  
		Size: 17.4 MB (17404662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c5771a62080319647861cb4f3fddf1930dc8c33e9b07e4803cf85493e8ca96`  
		Last Modified: Sat, 04 Feb 2023 15:18:48 GMT  
		Size: 3.6 MB (3628671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f10aee2e5bf04ea5b4afc7c56ad070104abc727b827d2e0f70a3a8bb4d14fbe`  
		Last Modified: Sat, 04 Feb 2023 15:18:44 GMT  
		Size: 567.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74b341c43b76ab0257da971e153571abc45bf4402c39032fcb2ac0aa7ae5b3c`  
		Last Modified: Sat, 04 Feb 2023 15:18:44 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c50959527a74b7ec2cb86f4544a76f532933b3e342d49919c2a2061ac2ce8fa`  
		Last Modified: Sat, 04 Feb 2023 15:19:15 GMT  
		Size: 155.9 MB (155896577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b7cea392b1176329c925cb8bf849358c42d79c7534958948be6520abeaad27`  
		Last Modified: Sat, 04 Feb 2023 15:18:44 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f47fe0aa570c7a85e216a4fc9c1772a06e2e3591e0803d15e0a2cedfe56b34`  
		Last Modified: Sat, 04 Feb 2023 15:18:44 GMT  
		Size: 2.2 KB (2210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:a91cabc2e27c1d0cd883a8aa36ceb86d4e2f2ad4b9852c5da01b4ee59962311a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.6 MB (309602063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664d73ac736202d33fdb77a279e8bf10a66f927f80a63995c381599176c9c9af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:33:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 17:33:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 17:34:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:34:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 17:34:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 17:37:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 17:37:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 17:37:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 17:37:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 17:37:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 17:37:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 17:37:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 17:37:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 18:22:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 18:22:11 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 18:22:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 18:22:11 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 18:22:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 18:22:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:24:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 18:24:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:24:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 18:24:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 18:24:42 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 18:24:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:24:43 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 18:24:43 GMT
EXPOSE 80
# Sat, 04 Feb 2023 18:24:43 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 07:49:44 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 05 Feb 2023 07:49:44 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 05 Feb 2023 07:49:45 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 05 Feb 2023 07:52:08 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 07:52:08 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 05 Feb 2023 07:52:08 GMT
VOLUME [/var/www/html]
# Sun, 05 Feb 2023 07:52:09 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 05 Feb 2023 07:52:09 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sun, 05 Feb 2023 07:52:58 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 07:53:01 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sun, 05 Feb 2023 07:53:01 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sun, 05 Feb 2023 07:53:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 07:53:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e99a581cb2817e40eb85d7abf6335048f4b22ad551abbc855b53afc98b5fb2d`  
		Last Modified: Sat, 04 Feb 2023 18:49:03 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da95bf5359e309f984a5070fc23599be40287bd16b4052cddd92b4678c728e9`  
		Last Modified: Sat, 04 Feb 2023 18:49:15 GMT  
		Size: 69.3 MB (69321531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe2b22eabcdd6b435933e6a20b4958e1039fe7ba43cb54be7afdaa4f9c2522`  
		Last Modified: Sat, 04 Feb 2023 18:49:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3691b67cd4e4294386cf6ac7d94f67af4cf8e14740d84e608b78c7575d47430d`  
		Last Modified: Sat, 04 Feb 2023 18:50:18 GMT  
		Size: 18.0 MB (17997668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021872cfa5b0c4f6a28c91a8d0144fc0bb160100d2bbf18361a4afe48d37432c`  
		Last Modified: Sat, 04 Feb 2023 18:50:15 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce51dca55116e88ecea9b7eb9423d8b84e69bd25c24d2f9d6cea3dc1c6fcde5`  
		Last Modified: Sat, 04 Feb 2023 18:50:15 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bf7a94202d04fb1f1a7589cf47f4bbea7aa2f4f805f637ea64c6a34103b6e`  
		Last Modified: Sat, 04 Feb 2023 18:58:24 GMT  
		Size: 11.1 MB (11141768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97fb1a4529be310de5fa0740da9a16927b6cf4729e836b9965ae111637d166e`  
		Last Modified: Sat, 04 Feb 2023 18:58:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a8b821e265ec08eb7ca0a22ed1556a8593e471aa3fa2fcd89a37555fc0870f`  
		Last Modified: Sat, 04 Feb 2023 18:58:23 GMT  
		Size: 9.3 MB (9305919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d734bbd69ebc224b6882327fda02b714d37cc5e0f15370fe980651f3082ea7`  
		Last Modified: Sat, 04 Feb 2023 18:58:21 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adeb6ce70ed6bb1328f8bb62776102df07eb89aa35e7154dad27940674f6e20`  
		Last Modified: Sat, 04 Feb 2023 18:58:21 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331b649a85019c6b50a7969aa02fb4d7e6ddb1d450e3a50bf4a16cf4745c7e0`  
		Last Modified: Sat, 04 Feb 2023 18:58:21 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f882f0e5663cb1ffcc3f6244bccc164c1b4e110df954cd4aca3ca3566cdbe970`  
		Last Modified: Sun, 05 Feb 2023 08:08:30 GMT  
		Size: 15.9 MB (15855444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9f9fb05c778d4ce40d6bfb71ff4b0bcc06689d89154761ebc461461c414f15`  
		Last Modified: Sun, 05 Feb 2023 08:08:28 GMT  
		Size: 3.5 MB (3511643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039853f60bf5641b0716348a222360f29a6ffaa5e96c6170e6ff29bb7cc48f43`  
		Last Modified: Sun, 05 Feb 2023 08:08:25 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1048a55fb0d47549be180e7416f3c773c926ece821fe3955d3c5bb2fd641a563`  
		Last Modified: Sun, 05 Feb 2023 08:08:25 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7b4fb98028a9ed7b8743f680b40f0cf4a6089597298c8834527f4bb6415bc3`  
		Last Modified: Sun, 05 Feb 2023 08:08:54 GMT  
		Size: 155.9 MB (155896563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e753582d88790f877abc5da4acd3625ea32f3b10614d076896d964e82c012`  
		Last Modified: Sun, 05 Feb 2023 08:08:25 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308e17e7f10ababdcf363bc5b6247d6fc6f3966a35623dbeb63b75e3480e5b25`  
		Last Modified: Sun, 05 Feb 2023 08:08:25 GMT  
		Size: 2.2 KB (2212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:9a26e40126d2f3c1c7925be2d3ebf6d9d61823ba873a34a0ed361e91a3637eb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334362028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26c7838ee400dea863ab8744ad59aa16b8352cd72c0022643ed2e1fd3ee26ec7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:06:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 12:06:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 12:06:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:06:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 12:06:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 12:09:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 12:09:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 12:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 12:09:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 12:09:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 12:09:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 12:09:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 12:09:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 12:58:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 12:58:01 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 12:58:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 12:58:01 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 12:58:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 12:58:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:00:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 13:00:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:00:09 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 13:00:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 13:00:09 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 13:00:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:00:09 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 13:00:09 GMT
EXPOSE 80
# Sat, 04 Feb 2023 13:00:09 GMT
CMD ["apache2-foreground"]
# Sat, 04 Feb 2023 23:30:08 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 04 Feb 2023 23:30:08 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 04 Feb 2023 23:30:08 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 04 Feb 2023 23:32:00 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 23:32:01 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 04 Feb 2023 23:32:01 GMT
VOLUME [/var/www/html]
# Sat, 04 Feb 2023 23:32:01 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sat, 04 Feb 2023 23:32:01 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sat, 04 Feb 2023 23:32:46 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 23:32:50 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 04 Feb 2023 23:32:50 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sat, 04 Feb 2023 23:32:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 23:32:50 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da18c5374c4d255e7dafff40d0aa1678eb619d4db6e9d1d9c88e10511e30463a`  
		Last Modified: Sat, 04 Feb 2023 13:16:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96df88fb307c1e07b72f4ae92690b53033413991cb08b8a7a1781eab2d118c3`  
		Last Modified: Sat, 04 Feb 2023 13:16:51 GMT  
		Size: 86.9 MB (86928244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907de944f221eeca88d8c6d1a6c5693a487a11c313b95a04e2d34c8d3d453676`  
		Last Modified: Sat, 04 Feb 2023 13:16:41 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8889a574aff3bd403f2467b2d08b85c5868f5577454b81aeb1381be6ba1fe78e`  
		Last Modified: Sat, 04 Feb 2023 13:17:36 GMT  
		Size: 19.2 MB (19166295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823226209ae32886f6c4ff15dd12574d7a702f87d7acba675b185d6c8d411e87`  
		Last Modified: Sat, 04 Feb 2023 13:17:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bc4a6f650ef4193ee453be30f80e863bb928b75af666584c6403531f200426`  
		Last Modified: Sat, 04 Feb 2023 13:17:33 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17654936086f15f014e3e7e07d9f007e44c5afcf5635eb798723ac08ff5796a5`  
		Last Modified: Sat, 04 Feb 2023 13:23:22 GMT  
		Size: 11.1 MB (11142632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0feda6b4647b975bd6ffc6fe9d52e0ee2d68ad512d5bf5d6cf64f8fff99c3fa0`  
		Last Modified: Sat, 04 Feb 2023 13:23:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d473cb414555b287aa9720d634b3348a6191095463bfc3195544b337c5f5e58b`  
		Last Modified: Sat, 04 Feb 2023 13:23:21 GMT  
		Size: 10.2 MB (10232430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8255e04c8f2ddc3227c36ec6a4740366434df66ab17e1824a791e5b1c393c3e`  
		Last Modified: Sat, 04 Feb 2023 13:23:19 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d942051562a56a884d73b92ff084397a26b480e630c47336c2669523f0ba741a`  
		Last Modified: Sat, 04 Feb 2023 13:23:19 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d7981a4a27905b5418d430ec56bb782d443d49938fbd3a82643d067c6c9ea7`  
		Last Modified: Sat, 04 Feb 2023 13:23:19 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ec5e6e008e5e09257d0ee239bd5720036048cbed6f99c0a67289cb17c46aff`  
		Last Modified: Sat, 04 Feb 2023 23:45:45 GMT  
		Size: 17.2 MB (17153679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae625158ed10c33ee976b970aa62d1e08a02b8e607bfce51957f174ca55e0dc`  
		Last Modified: Sat, 04 Feb 2023 23:45:44 GMT  
		Size: 3.8 MB (3784154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5c0cea2366fe6fb664ac0a896d5e2febc4712a0e75fc464a4b6021896bc316`  
		Last Modified: Sat, 04 Feb 2023 23:45:41 GMT  
		Size: 599.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26da23ad77472f9340caf7d80e52c0d6c33d68065e1910246a965999e16e7100`  
		Last Modified: Sat, 04 Feb 2023 23:45:41 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fdd09e83f3d15851b86e8bd41002e3491237cdf2c089d78f8e496e6292d6d0`  
		Last Modified: Sat, 04 Feb 2023 23:45:57 GMT  
		Size: 155.9 MB (155897606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9f93c1b2851090dbf77eac1039e530eca3893a729ea736ae881f64ef3c4591`  
		Last Modified: Sat, 04 Feb 2023 23:45:41 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9c3d1e4bf5e578f263b3965181ec62e0615f6a12d53d429bef760e0119528c`  
		Last Modified: Sat, 04 Feb 2023 23:45:41 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; 386

```console
$ docker pull nextcloud@sha256:3dd99fb11105d5bcdae0b3401abcd84ea58fd438a949bc45543e4600736f38d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345125023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf28b723c3afa6892b886a674fe462d2685a5ffbb478368332587fbc8c06071`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:16:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 14:16:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 14:17:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:17:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 14:17:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 14:20:29 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 14:20:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 14:20:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 14:20:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 14:20:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 14:20:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 14:20:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 14:20:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 15:12:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 15:12:03 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 15:12:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 15:12:05 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 15:12:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 15:12:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 15:14:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 15:15:00 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 15:15:00 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 15:15:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 15:15:02 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 15:15:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 15:15:04 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 15:15:05 GMT
EXPOSE 80
# Sat, 04 Feb 2023 15:15:06 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 01:41:33 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 05 Feb 2023 01:41:33 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 05 Feb 2023 01:41:34 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 05 Feb 2023 01:43:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 01:43:52 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 05 Feb 2023 01:43:53 GMT
VOLUME [/var/www/html]
# Sun, 05 Feb 2023 01:43:54 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 05 Feb 2023 01:43:55 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sun, 05 Feb 2023 01:44:46 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 01:44:48 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sun, 05 Feb 2023 01:44:50 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sun, 05 Feb 2023 01:44:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 01:44:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a321222e001cd5e88835744c33121c005059d526245dadc96d073e0ebbcbef`  
		Last Modified: Sat, 04 Feb 2023 15:39:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df692c85155e1069b9b93a9f5a97745dee439e163361ee8153af9c77e0c30ef6`  
		Last Modified: Sat, 04 Feb 2023 15:40:07 GMT  
		Size: 92.7 MB (92716641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff08046d135a823f8b4f09797f06c51826c29274c0fc0e55965306af9d734263`  
		Last Modified: Sat, 04 Feb 2023 15:39:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a2d61d900281e5661eb5bec8ebc8e2966bd7957d41f6e08c0045a6cde7ae25`  
		Last Modified: Sat, 04 Feb 2023 15:41:05 GMT  
		Size: 19.5 MB (19515950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2708a99d8dff10d9c4458c192382a6559a6491e655ed75e9a7a270e2211508e`  
		Last Modified: Sat, 04 Feb 2023 15:41:02 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0557af0a3e0745cfbaab2c07a324c7c23b27fa2a90f66e5288dcefbd01344cee`  
		Last Modified: Sat, 04 Feb 2023 15:41:02 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd877413ebfc89586f6df46dc10a91773cc4f0ea080607044bb9fe0636bf98bb`  
		Last Modified: Sat, 04 Feb 2023 15:48:20 GMT  
		Size: 10.9 MB (10926211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7617a4413fac307cb8bfd70a005075f22a8e5d4c923364e98b872760941d51`  
		Last Modified: Sat, 04 Feb 2023 15:48:17 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4516ccd1e76482573c549bf41a2dfd8577784444613bcd5b8c60a9b315614331`  
		Last Modified: Sat, 04 Feb 2023 15:48:19 GMT  
		Size: 11.0 MB (10980923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bef9e0c5c73f9861505c1da30515bd2c74d00472b043bc620ef1a3daa00b93`  
		Last Modified: Sat, 04 Feb 2023 15:48:17 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf8c51fb4ad7712a2eaf955cef706ffca2431cc6b74c331ab76fe95a5725a4f`  
		Last Modified: Sat, 04 Feb 2023 15:48:17 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3f220900c67d5b747d51e281ad49d9b53337e71d10668157bf3ae632414216`  
		Last Modified: Sat, 04 Feb 2023 15:48:17 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4df45c7075fcada0a4097ba687c983450f18022aad861a6fd3ec26cb9d663b`  
		Last Modified: Sun, 05 Feb 2023 02:00:01 GMT  
		Size: 19.0 MB (19046103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c9090d9eee78d82bd9832471de540659084e2b3e56d782c461fb4a903a69fa`  
		Last Modified: Sun, 05 Feb 2023 01:59:58 GMT  
		Size: 3.9 MB (3893189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd3d80f52eeb0c9ebc4452d9568afb4690a25a78ca162345a4ba1676ebe1e5a`  
		Last Modified: Sun, 05 Feb 2023 01:59:55 GMT  
		Size: 567.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715e311126da28e450e8276c0b5639ca12f9444c6de0ec8d4dffacd50d570c6`  
		Last Modified: Sun, 05 Feb 2023 01:59:55 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cdcd9410a776bc1476b58703abe6cda0937c0e1d69166a6f3bd421e467e0fe`  
		Last Modified: Sun, 05 Feb 2023 02:00:15 GMT  
		Size: 155.7 MB (155658168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4f3d9a8fdfc49c459bd56a32fb465e4748128b19c8f2b3aef063f11fbc599`  
		Last Modified: Sun, 05 Feb 2023 01:59:55 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c095149284ddfd46ecd325a0a693d31d5efe7eea7a5036c14dfd63632c19c3`  
		Last Modified: Sun, 05 Feb 2023 01:59:55 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; mips64le

```console
$ docker pull nextcloud@sha256:66eaeb1284bf9f2bd89282cdabebb1b142786357b46b4089ffdf0cac75d9cfe3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.9 MB (317888072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d76c0b1e2057b69043a4ee9fb385422572fd694c6cde8f96488853e5efbcd15`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:20:15 GMT
ADD file:03d6cf2d45a21e59975a1d17c6ca9fc83bb7a0da235873315c9c7940245beb1e in / 
# Sat, 04 Feb 2023 06:20:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:20:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 08:20:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 08:22:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:22:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 08:22:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 08:37:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 08:37:31 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 08:38:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 08:38:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 08:38:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 08:38:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 08:38:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 08:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 10:32:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 10:32:56 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 10:33:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 10:33:04 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 10:33:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 10:33:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:47:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 10:47:21 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:47:27 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 10:47:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 10:47:35 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 10:47:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:47:42 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:47:45 GMT
EXPOSE 80
# Sat, 04 Feb 2023 10:47:49 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 07:49:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 05 Feb 2023 07:49:33 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 05 Feb 2023 07:49:37 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 05 Feb 2023 08:00:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 08:00:43 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 05 Feb 2023 08:00:47 GMT
VOLUME [/var/www/html]
# Sun, 05 Feb 2023 08:00:54 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 05 Feb 2023 08:00:58 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sun, 05 Feb 2023 08:03:42 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 08:03:53 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sun, 05 Feb 2023 08:04:01 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sun, 05 Feb 2023 08:04:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 08:04:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:aedd2a952aead0f89a308f23f44377263665bf76192d5542abd66473ea799d44`  
		Last Modified: Sat, 04 Feb 2023 06:28:25 GMT  
		Size: 29.6 MB (29619892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff43158f49324badc4ea902c1c2ec7dc1b8f7c9f2869404a04b577b1c1464ec`  
		Last Modified: Sat, 04 Feb 2023 11:15:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52542ce06c84ba89cc8bd539bf1f2d6db5c1d20cb71ee57a8e7160cd9180b73c`  
		Last Modified: Sat, 04 Feb 2023 11:16:35 GMT  
		Size: 72.0 MB (72018579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dea0ac97e0895aef2d803c14a9abb3185ee4daa4ea889e8c209f1c1a2e4c76`  
		Last Modified: Sat, 04 Feb 2023 11:15:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bfa5685c8a273fdf65424dfb932d5a843c6e96d002ea0c7c078f5357e37306`  
		Last Modified: Sat, 04 Feb 2023 11:17:35 GMT  
		Size: 18.9 MB (18940104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929b3d4eb360c3018b530e16add345accc1f860b270875d6498c9046a288417`  
		Last Modified: Sat, 04 Feb 2023 11:17:23 GMT  
		Size: 440.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8d223dd4c1b855a4d7cba1330c3753ee72e67fa89ba10fa6a4726a22f1267`  
		Last Modified: Sat, 04 Feb 2023 11:17:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64e61d4c6e47709947474dbf252dd64fa9d029ec58c084c8bf064ebb1b95ec4`  
		Last Modified: Sat, 04 Feb 2023 11:22:22 GMT  
		Size: 10.9 MB (10925368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e58e2f4e33da9cf539f759da7da42fc2e74ea17f54ee99cf0fac243e2e68a0`  
		Last Modified: Sat, 04 Feb 2023 11:22:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e823137a965200a7de6db794467a93a4a31e14039941ab908c46244473dff3b0`  
		Last Modified: Sat, 04 Feb 2023 11:22:25 GMT  
		Size: 9.9 MB (9918256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1a8bfe92094e5c87af8ee4c9d0bb3ab64872e1767624ae551bcb6ea079a0c7`  
		Last Modified: Sat, 04 Feb 2023 11:22:17 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015b527810a55593023c851e4b0ced26ee9d1fac5bec5851e82334f09bd53201`  
		Last Modified: Sat, 04 Feb 2023 11:22:17 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a7fabb6a64644d4a2b15c124791f4477d1b91a181d8a4341b90cca2d72103a`  
		Last Modified: Sat, 04 Feb 2023 11:22:17 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57097c62ee1bd82f95bc311a828b25b610f53dcf3a4cefc9c45fbbae6a93fc2`  
		Last Modified: Sun, 05 Feb 2023 09:00:37 GMT  
		Size: 17.3 MB (17269534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44de2de0239b9f7d49be05bd358b8728dc0999065821d07afdb59962fb59b77f`  
		Last Modified: Sun, 05 Feb 2023 09:00:29 GMT  
		Size: 3.5 MB (3524956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddeafe926b4e3ad0e1dc84676d8db546807626e83a319323ad69f92a4a4ae6f9`  
		Last Modified: Sun, 05 Feb 2023 09:00:22 GMT  
		Size: 566.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fb3c37b8d3f5b8e459a8e08292d3c83f723de67942143e81dbc51030f20adb`  
		Last Modified: Sun, 05 Feb 2023 09:00:21 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3883c0bbe41f4a5363a35b1b30e11aecee6bbaf22c5fca9bbde4b2cd123b6606`  
		Last Modified: Sun, 05 Feb 2023 09:02:07 GMT  
		Size: 155.7 MB (155659294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea92a11c7f5b585777f7afe465174c359c389d77306bfe2ca7f8ca8a96724202`  
		Last Modified: Sun, 05 Feb 2023 09:00:22 GMT  
		Size: 3.2 KB (3240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e73064e8993dbe95d7a9f6a683689401584fc58c7ea3ce9e0be132aec1cb514`  
		Last Modified: Sun, 05 Feb 2023 09:00:22 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:ae656463d9d2a2742efdf6d3d963555740949768940af93bc1afffbb221d5d3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.2 MB (344227067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f4122a2c501b437ee5210af0c41d584589600ab2460dbf91bf1c580b3082d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 15:37:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 15:37:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 15:38:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 15:38:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 15:38:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 15:43:37 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 15:43:37 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 15:43:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 15:44:00 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 15:44:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 15:44:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 15:44:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 15:44:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 16:21:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Feb 2023 16:21:17 GMT
ENV PHP_VERSION=8.0.27
# Sat, 04 Feb 2023 16:21:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Sat, 04 Feb 2023 16:21:18 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Sat, 04 Feb 2023 16:21:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 16:21:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 16:26:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 16:26:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 16:26:15 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 16:26:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 16:26:16 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 16:26:16 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 16:26:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 16:26:17 GMT
EXPOSE 80
# Sat, 04 Feb 2023 16:26:17 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 00:27:54 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 05 Feb 2023 00:27:55 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 05 Feb 2023 00:27:55 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 05 Feb 2023 00:32:13 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:32:14 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 05 Feb 2023 00:32:15 GMT
VOLUME [/var/www/html]
# Sun, 05 Feb 2023 00:32:16 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 05 Feb 2023 00:32:17 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Sun, 05 Feb 2023 00:33:27 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:33:42 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sun, 05 Feb 2023 00:33:43 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Sun, 05 Feb 2023 00:33:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:33:44 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7dbc2248969aa57feae4670752b57711781d9c8c62063b62fa737199e7a7e3`  
		Last Modified: Sat, 04 Feb 2023 16:40:56 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0eb6131ffd41950a30a7a08aec0640110e260b088e80bc21bd2b7e113c9a88a`  
		Last Modified: Sat, 04 Feb 2023 16:41:22 GMT  
		Size: 86.6 MB (86632976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a41c57b232a8430c20b9982f232ddf7d398d59be773fd96bd319965b4a1241f`  
		Last Modified: Sat, 04 Feb 2023 16:40:56 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c269f47870af442cc7fd9c13a60ca939060d9398cf81a76486d6af6ec738751a`  
		Last Modified: Sat, 04 Feb 2023 16:42:28 GMT  
		Size: 20.5 MB (20464272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0649a2345bfec97d1a81012b03e12a3773fefc467f963cd6ed9c9749524880e9`  
		Last Modified: Sat, 04 Feb 2023 16:42:22 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188f66379105c5a09dfaa76a8ec4584d1c4acf1f4b30f06626e598b25f319dec`  
		Last Modified: Sat, 04 Feb 2023 16:42:22 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ad1fcf3f33cb46033245f48f4ccb2fc7ae08eb83c186e0514fc0777663d0e1`  
		Last Modified: Sat, 04 Feb 2023 16:47:57 GMT  
		Size: 11.1 MB (11143324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d208ce28fc0e1b666adc52d00ef4e026d61be7fb7d8d98267e0d97ca9698a6`  
		Last Modified: Sat, 04 Feb 2023 16:47:54 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fad1a12923bff4ea8c8c3e280ad7791b78f565c5d65d70cea4f66dc24e8723`  
		Last Modified: Sat, 04 Feb 2023 16:47:58 GMT  
		Size: 11.1 MB (11139621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fa17effc964b07ebe4d3f9ec90a0237498d3faae23fbff03a0355bbd04ea70`  
		Last Modified: Sat, 04 Feb 2023 16:47:53 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1f2b45414426f07061c420519600499da18d974f2a454f6a6fbb695df30eaf`  
		Last Modified: Sat, 04 Feb 2023 16:47:53 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef3e153a86a9b60ca1cdbb91b687f609d6ee03b693ba4e3512ce12e322a1723`  
		Last Modified: Sat, 04 Feb 2023 16:47:54 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c68d1279601f7324e7b582349d727de56a8dcae71a423346499435591bbca28`  
		Last Modified: Sun, 05 Feb 2023 00:59:58 GMT  
		Size: 19.6 MB (19625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8daaddd54efb3cea400d62fe17b6bff148f8f5b0a32b008240dd1da226c9120e`  
		Last Modified: Sun, 05 Feb 2023 00:59:54 GMT  
		Size: 4.0 MB (4041499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b95d47551bfaf3a558d0b1fdb6de85649770d7e0c2834a155e356fc1152ffe`  
		Last Modified: Sun, 05 Feb 2023 00:59:51 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0860c706a110ce7975f0cdd5cb1163323492f88e4b7a067cf36c4db577c1618`  
		Last Modified: Sun, 05 Feb 2023 00:59:51 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2949a85ab8e737f7b775e423b52133d07b14fddb22b40ca852edd780c9151e30`  
		Last Modified: Sun, 05 Feb 2023 01:00:27 GMT  
		Size: 155.9 MB (155899208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d241f2af6da654b754bdec4be20518b5e6fadb08ed810ccfe7ce2c242d7e16e0`  
		Last Modified: Sun, 05 Feb 2023 00:59:51 GMT  
		Size: 3.2 KB (3242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71498535ad15c81b720476545a9f88a8200f5772c30c25b6a98de5b7c72cb3f5`  
		Last Modified: Sun, 05 Feb 2023 00:59:51 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:23-apache` - linux; s390x

```console
$ docker pull nextcloud@sha256:868f200ff90e15144f4e02957028a0313be0851fbea83885480c69bfa7ec28bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318270840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7f553750ce26b78691f28ff7cee6de4d8c3ac057ef7df4dfb048e842c1760d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:19:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 05:19:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 05:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:20:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 05:20:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 05:25:31 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 05:25:31 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 05:25:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 05:25:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 05:25:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 05:25:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:25:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:25:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 06:00:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Thu, 09 Feb 2023 06:00:32 GMT
ENV PHP_VERSION=8.0.27
# Thu, 09 Feb 2023 06:00:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.27.tar.xz.asc
# Thu, 09 Feb 2023 06:00:33 GMT
ENV PHP_SHA256=f942cbfe2f7bacbb8039fb79bbec41c76ea779ac5c8157f21e1e0c1b28a5fc3a
# Thu, 09 Feb 2023 06:00:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Feb 2023 06:00:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:03:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Feb 2023 06:03:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:03:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Feb 2023 06:03:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Feb 2023 06:03:05 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Feb 2023 06:03:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:03:06 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:03:06 GMT
EXPOSE 80
# Thu, 09 Feb 2023 06:03:06 GMT
CMD ["apache2-foreground"]
# Thu, 09 Feb 2023 13:19:35 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common         libmagickcore-6.q16-6-extra     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 09 Feb 2023 13:19:39 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 09 Feb 2023 13:19:39 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 09 Feb 2023 13:22:18 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:22:19 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 09 Feb 2023 13:22:19 GMT
VOLUME [/var/www/html]
# Thu, 09 Feb 2023 13:22:20 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 09 Feb 2023 13:22:20 GMT
ENV NEXTCLOUD_VERSION=23.0.12
# Thu, 09 Feb 2023 13:24:10 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:24:40 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Thu, 09 Feb 2023 13:24:42 GMT
COPY multi:5ae4d3e2c333d07b72b698ef5d54be9ec19b520851d7d23aff0a612bc28d533d in /usr/src/nextcloud/config/ 
# Thu, 09 Feb 2023 13:24:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 13:24:44 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3df263a1c9e1be6bb9ae8d3128a5b370055484fccdb14fb616c797eb10b605`  
		Last Modified: Thu, 09 Feb 2023 06:13:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12a22024ac2b88388a15678ebf2257c430a770dbc92181a3d46ee4a6e7925c2`  
		Last Modified: Thu, 09 Feb 2023 06:13:48 GMT  
		Size: 71.6 MB (71628890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d91b6fd48d29a549f5f9e77d78578b0a170890a62eaf70107d6f4a80126cba0`  
		Last Modified: Thu, 09 Feb 2023 06:13:38 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46ec046fc8903c85a12c9c8c61db044bb40931eb7405e5f31266b87ef480922`  
		Last Modified: Thu, 09 Feb 2023 06:14:23 GMT  
		Size: 19.1 MB (19072273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cccefc82c4ed82bb1808bdbbe8937b84723ddc35929d41b619ad61b8912dc`  
		Last Modified: Thu, 09 Feb 2023 06:14:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e10114ab4dab1689ab15f5c09c932fc512030217b27d6999d48ec1e6a2b4e86`  
		Last Modified: Thu, 09 Feb 2023 06:14:20 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bb6487a1282a62c510ecd5ab1fb376ce59659cc028a29453d0fc2df61f1d6d`  
		Last Modified: Thu, 09 Feb 2023 06:17:42 GMT  
		Size: 11.1 MB (11142456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25a0e6718d323d680d70897dcf939ba5c5d930541115fc0794a41abbd08a8ea`  
		Last Modified: Thu, 09 Feb 2023 06:17:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a36e91a04bd1eb6061769cd2ce1ab695e00cead16085ca8a6ac1a4c2f23e324`  
		Last Modified: Thu, 09 Feb 2023 06:17:42 GMT  
		Size: 9.9 MB (9923374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71164fb4f3279fed56d2104a14e98a4d57c412581820fe3d904217a2a41d2b`  
		Last Modified: Thu, 09 Feb 2023 06:17:40 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4aac8793a68bed9b69084ef5589103e4af081ca79ffa94b1efbd7e515c3c98`  
		Last Modified: Thu, 09 Feb 2023 06:17:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cd9e348fd85d2c37046e419182024b28e17be27f2185718214ca75158f34f5`  
		Last Modified: Thu, 09 Feb 2023 06:17:40 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c702710368fc6a88be9faa6b78f113832fc3a7bb5a286315494ed94c2fe8800`  
		Last Modified: Thu, 09 Feb 2023 13:52:26 GMT  
		Size: 17.1 MB (17133154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fdaa64f0d247252dc62ae682f85ed8a9fe4d878293d54ae839d45e44380c9b`  
		Last Modified: Thu, 09 Feb 2023 13:52:24 GMT  
		Size: 3.8 MB (3813644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c4511f5df74ca4818a1b3ffff3fa959ba311835b66d780e43369e2f27b9cd`  
		Last Modified: Thu, 09 Feb 2023 13:52:22 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7298d4d7b1d225edbf9e409001e2a9671ab63643b3a6c816e56a17fef6d7e568`  
		Last Modified: Thu, 09 Feb 2023 13:52:22 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57589dbcb621424c25e28dba6985400367697897143eb11306a8193c4c849b5b`  
		Last Modified: Thu, 09 Feb 2023 13:52:40 GMT  
		Size: 155.9 MB (155897323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65cb5d791aa84454bf95937ce6cd3ae481dd6fac77eb1eddec4169559417d09`  
		Last Modified: Thu, 09 Feb 2023 13:52:22 GMT  
		Size: 3.2 KB (3241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b7b2888790b4dd9048f5c630f14ec103860e3b44090583a8321f0c20e7357d`  
		Last Modified: Thu, 09 Feb 2023 13:52:22 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
