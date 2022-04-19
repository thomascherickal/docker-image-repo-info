## `nextcloud:production-apache`

```console
$ docker pull nextcloud@sha256:dabce92ba6a2e9328655a908c4e3bed6fdeb93015faaefa71090b74f8b1ef3bf
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

### `nextcloud:production-apache` - linux; amd64

```console
$ docker pull nextcloud@sha256:5d02434aa832398f11824289e6feaf2f91b7fa657ea5904f0c98b490f485d4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.1 MB (327085673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9a3a2fda942244ddb5c5371f2986210acf48c80acb469f5da9705568a6631fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:15:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:15:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:16:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:16:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:16:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:20:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:20:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:20:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:21:00 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:21:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:21:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:21:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:21:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:23:12 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 19 Apr 2022 00:05:52 GMT
ENV PHP_VERSION=8.0.18
# Tue, 19 Apr 2022 00:05:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Tue, 19 Apr 2022 00:05:52 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Tue, 19 Apr 2022 00:06:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:06:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:09:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 00:09:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:09:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 00:09:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 00:09:05 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 00:09:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:09:05 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 00:09:05 GMT
EXPOSE 80
# Tue, 19 Apr 2022 00:09:05 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 04:30:38 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 19 Apr 2022 04:30:38 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 04:30:38 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 04:33:15 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 04:33:16 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 04:33:16 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 04:33:16 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 04:33:17 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Tue, 19 Apr 2022 04:34:02 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 04:34:03 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 19 Apr 2022 04:34:04 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 19 Apr 2022 04:34:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 04:34:04 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e86af584f1e1432f2e919354a76a112af1f3146d6b2342e32a496eca57f70a`  
		Last Modified: Tue, 29 Mar 2022 04:17:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd55b3ae5fafd56f7dc3bbd88b11372bda66b4043b9075a626d392863203a5`  
		Last Modified: Tue, 29 Mar 2022 04:17:44 GMT  
		Size: 91.6 MB (91602066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3a70af964a1258ce68bbae397b3464a892ea2210425230d68ccdfa5e62ab90`  
		Last Modified: Tue, 29 Mar 2022 04:17:31 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5086159710b3ea409b4fa418d18041a81acedf8b2e62b356b16538ac746e49`  
		Last Modified: Tue, 29 Mar 2022 04:18:37 GMT  
		Size: 19.2 MB (19248565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c764dc190cebd90a1661358ab11342866a47bfc7bf5898df1cf82751a6872`  
		Last Modified: Tue, 29 Mar 2022 04:18:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2bb7a6eead8d367aaf40f9a05e9a63913789cb1a551360a57f142680939a67`  
		Last Modified: Tue, 29 Mar 2022 04:18:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc408d051f4feb0834cafae60519863ae32deae189b6bf16e508378947d36424`  
		Last Modified: Tue, 19 Apr 2022 01:55:27 GMT  
		Size: 11.2 MB (11212222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e62542debeda9f8c6dc555cb21d221d1356a3d0032558b076385e633c317bd`  
		Last Modified: Tue, 19 Apr 2022 01:55:24 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d146a3f094464c379b0f7cc99a873e2de285106c8a5caffcff45e7cb275c16`  
		Last Modified: Tue, 19 Apr 2022 01:55:26 GMT  
		Size: 10.8 MB (10831222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77680208673edab559179ad1a4a9ec79a3dac121285749f686370aa4df127e4`  
		Last Modified: Tue, 19 Apr 2022 01:55:24 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c21777aaec1f41f64954bff43c85516f8486175577269259ddef77a3f21206f`  
		Last Modified: Tue, 19 Apr 2022 01:55:24 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab76a6b28dbd0cbfda24c1070cb8be923d1dc205009e54f6d25f508dbae862a7`  
		Last Modified: Tue, 19 Apr 2022 01:55:24 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f89f13a0e2f95985969a4ac4bc0eb8078515f6a46b9886b05ff59050bc37f9`  
		Last Modified: Tue, 19 Apr 2022 04:40:43 GMT  
		Size: 1.7 MB (1701038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1accf4d05c71f43f8c09dade53601f721244e60d9aeb140772cd4de7e766139`  
		Last Modified: Tue, 19 Apr 2022 04:40:45 GMT  
		Size: 17.6 MB (17579241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c68796e668948075f1a333b74601e4c943e742984f942dc38b06819dd0ede3`  
		Last Modified: Tue, 19 Apr 2022 04:40:39 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20b16bb7fc8623f7d0545d7406f38978093478c78c171613e04a9da7611206f`  
		Last Modified: Tue, 19 Apr 2022 04:40:40 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbbcc49abedf9d8cd93f37881119b6667dbbc9838d3493a30744af30b07d133`  
		Last Modified: Tue, 19 Apr 2022 04:40:58 GMT  
		Size: 143.5 MB (143521292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852df7552606f85bc1e423b2c912ec0c5a0af8c100988a1a70a9aee76c13a289`  
		Last Modified: Tue, 19 Apr 2022 04:40:39 GMT  
		Size: 2.6 KB (2632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11a7402f00ef0844ba7a0c9f6ce7b22ac23af5c8f958cfa8bafc9d23be84957`  
		Last Modified: Tue, 19 Apr 2022 04:40:40 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:2fe8e8c9a241b49e5066bc4a2f598a123f4e5af2dc957ab7e6141224a25ff014
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302660833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b681f7d1f1804544803e9718031b828287b158fa1f5f97eeb4c9714de6a14f82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:37 GMT
ADD file:6b9a30e6ef50a46e87cf9d7f5a491c7951fdb6dd6fab3c9d4a9c3c40f92b8db4 in / 
# Tue, 29 Mar 2022 00:50:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:16:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:16:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:17:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:17:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:23:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:23:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:23:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:24:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:24:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:24:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:24:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:24:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:10:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 19 Apr 2022 00:39:54 GMT
ENV PHP_VERSION=8.0.18
# Tue, 19 Apr 2022 00:39:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Tue, 19 Apr 2022 00:39:55 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Tue, 19 Apr 2022 00:40:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:40:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:45:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 00:45:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:45:30 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 00:45:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 00:45:31 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 00:45:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:45:32 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 00:45:33 GMT
EXPOSE 80
# Tue, 19 Apr 2022 00:45:33 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 07:33:33 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 19 Apr 2022 07:33:33 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 07:33:33 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 07:40:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 07:40:42 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 07:40:43 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 07:40:44 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 07:40:45 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Tue, 19 Apr 2022 07:42:19 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 07:42:22 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 19 Apr 2022 07:42:24 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 19 Apr 2022 07:42:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 07:42:25 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9a41aba0a099ec129c20f41f6370b97daa4c3d4d3edc76ea1863bc5f76f9e5e5`  
		Last Modified: Tue, 29 Mar 2022 01:05:21 GMT  
		Size: 28.9 MB (28920513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46f4c5a9bc9955de9826fb0dff7ec089eacc125544c70af55cf4c30a8e79ba`  
		Last Modified: Tue, 29 Mar 2022 03:37:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036fb93b9d2bc083de782babbcfb0df052105b14e970e64c6ef75782dde7230`  
		Last Modified: Tue, 29 Mar 2022 03:38:00 GMT  
		Size: 73.7 MB (73683213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57be801222463b9801716ed946fa048154ecd7575d3fdba525981c6d1bcba244`  
		Last Modified: Tue, 29 Mar 2022 03:37:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dfbd691c3d3220988a7ef18e67d783c317a092640aabc8429bbe24563e1c55`  
		Last Modified: Tue, 29 Mar 2022 03:39:20 GMT  
		Size: 18.5 MB (18545967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b5a1e6b8a36786ac052aa20f3f03053e1b17a587b4bde699a687ce37420b`  
		Last Modified: Tue, 29 Mar 2022 03:39:09 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aefd878aa4f2a8a0ce13c03a80714f78c1fccb1cdd16e63f13cd2de0ba97e5`  
		Last Modified: Tue, 29 Mar 2022 03:39:09 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae8322d49b75b01471c82c09f8c77418e15f919beafbb6ab52d56b26c8df38e`  
		Last Modified: Tue, 19 Apr 2022 02:15:11 GMT  
		Size: 11.2 MB (11211069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e338324f8e8010d34e3b0ec4b65488a6db91f73cff9648a4fc8fd136bab7d1d`  
		Last Modified: Tue, 19 Apr 2022 02:15:06 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dfedd15c0ef0446e89f149a2ea57390c60043599724123f8bb8c50282b5d32`  
		Last Modified: Tue, 19 Apr 2022 02:15:14 GMT  
		Size: 9.8 MB (9844261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bd29eb6e14229ca3a0f60dbb334c76230ae2389e9a846db55d56ff0b7eb7e8`  
		Last Modified: Tue, 19 Apr 2022 02:15:06 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789f2a745e552fdc5f449d3734b84bd5f33f35d112e71a5045f3bcd7d073c16a`  
		Last Modified: Tue, 19 Apr 2022 02:15:06 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d770694df1c8dd05bed82001e219c9a7e492b7e4ebee25685f6bd81c66bd4b0`  
		Last Modified: Tue, 19 Apr 2022 02:15:06 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1abee9be3e1bcdd86921d0a82ebe3e65946b6e0c8747b75c642c40f2c5782`  
		Last Modified: Tue, 19 Apr 2022 07:57:56 GMT  
		Size: 1.7 MB (1656790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a428163086cc250df004e7435992f6958df2b5a0ed957ff46dbbf3d6a75395`  
		Last Modified: Tue, 19 Apr 2022 07:58:05 GMT  
		Size: 15.3 MB (15267308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f67088b5af73023c7562820bccfef87c6c87b30863295d360effc0a2eaa996`  
		Last Modified: Tue, 19 Apr 2022 07:57:54 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6d4197a59b5325f0db85ba64229fd0777f4c5854a4e5d4473dfe4a7433a5bc`  
		Last Modified: Tue, 19 Apr 2022 07:57:54 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e386e3a5ea1635a8c306637fc208a9fb83628dbbe9efa954ddd10530f3f87523`  
		Last Modified: Tue, 19 Apr 2022 07:59:32 GMT  
		Size: 143.5 MB (143520114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc159a1cedfe53c2abc686f273d747f8fd50f7e563922371e0104c2e8cc1a43`  
		Last Modified: Tue, 19 Apr 2022 07:57:54 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4accc8d924911e114c8de43e0cfbfde3780146b624e674cb621689ca5446e371`  
		Last Modified: Tue, 19 Apr 2022 07:57:54 GMT  
		Size: 2.2 KB (2203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:bdf0a6cf7bc28eb0fed741f99e2ff5062b3102b7fb83d42dd47ddd16ca2ca201
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.4 MB (293387433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2663d0df5be1af98fa42ba59674d30ac152e41895d6ba3ff22262b2bdf9d349e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

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
# Tue, 29 Mar 2022 06:55:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 06:55:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 06:55:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 06:55:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 06:55:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 06:55:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:55:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:55:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 07:56:40 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 07:56:41 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 07:56:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 07:56:41 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 07:57:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 07:57:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:01:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 08:01:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:01:35 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 08:01:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 08:01:36 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 08:01:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:01:37 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 08:01:37 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:01:38 GMT
CMD ["apache2-foreground"]
# Tue, 29 Mar 2022 17:23:03 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Mar 2022 17:23:03 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Mar 2022 17:23:03 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Mar 2022 17:29:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:38 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Mar 2022 17:29:39 GMT
VOLUME [/var/www/html]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Mar 2022 17:29:41 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Tue, 29 Mar 2022 17:31:14 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:31:18 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Mar 2022 17:31:20 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 29 Mar 2022 17:31:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 17:31:21 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:7d387fd4a423cc7a5d08660b5cbab93b450e830693bae14bd0b5e74dd3ccabc8`  
		Last Modified: Tue, 29 Mar 2022 10:31:04 GMT  
		Size: 18.0 MB (17993444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ad2abc9ddd2e0652b66bca116bf660d0cc0a718ed979975175469fe3ab60fe`  
		Last Modified: Tue, 29 Mar 2022 10:30:57 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d62c351c39830761e1abfc546b19a7aaae127dfc337b7d13d9711419fad52`  
		Last Modified: Tue, 29 Mar 2022 10:30:57 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e97e0d326f1dba7fae574fcb68be3afb0aa0a80ff8abc2195b852cf39eef1df`  
		Last Modified: Tue, 29 Mar 2022 10:40:11 GMT  
		Size: 11.1 MB (11110900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee24f474fefe90ce8cfad22ed0b15a893bcb19705958ec050bc80b5915bed746`  
		Last Modified: Tue, 29 Mar 2022 10:40:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ae867ac52a1279621c956aa5e055079fddf1504544ef3451f2dc82e1426f2`  
		Last Modified: Tue, 29 Mar 2022 10:40:12 GMT  
		Size: 9.3 MB (9303878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d365dcc7105177d02d07aa9309800d667f1dcec93d9b86b5181421f4e9a6f6c`  
		Last Modified: Tue, 29 Mar 2022 10:40:07 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffa80812b64f44a08f36fd755bd6b7ac42f242fde75101126b625a750fef669`  
		Last Modified: Tue, 29 Mar 2022 10:40:07 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d695e9fe98e6a87f64d6a48c120ed44416257466f077e13903524099efe1c`  
		Last Modified: Tue, 29 Mar 2022 10:40:07 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5da78a434562cebdcc40a10e540d1f4f241e03aef3c02ff7aa6b61e8f18aff1`  
		Last Modified: Tue, 29 Mar 2022 17:55:27 GMT  
		Size: 1.5 MB (1510604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0e09f0484c53496da7ffb78b2ceae1531389db062e6615a439d7d7fee0bfe`  
		Last Modified: Tue, 29 Mar 2022 17:55:34 GMT  
		Size: 14.0 MB (14046018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af636d5df7a395bc39e4f8e61cab890143c88e8c3059fdb8c24edc105eb8cec`  
		Last Modified: Tue, 29 Mar 2022 17:55:24 GMT  
		Size: 601.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd7937c1bda953a7305e5572829c91a89f3604e8a6d5cdc136d69651c59743d`  
		Last Modified: Tue, 29 Mar 2022 17:55:24 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c1bdfa57c797f979c160df4c60d9ddb6d7516d838d04d2fe68486b75dc87`  
		Last Modified: Tue, 29 Mar 2022 17:56:51 GMT  
		Size: 143.5 MB (143519925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34059a056e830dc0ccd808fc1559fc17836af931c65aa8a7c7f1f3d9565f995`  
		Last Modified: Tue, 29 Mar 2022 17:55:24 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b272329d442a613bbf047abacf34369022cf9ac40088300817bd03a4718e2b5`  
		Last Modified: Tue, 29 Mar 2022 17:55:24 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:03848a1ff5a7e80a9fcaa57c5d073b5958e6c58cb46047ac03ec6c3ab84bf7de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316633413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d738cbbd14f87950d4f3589aaacea3525b559a5eeb0cd0d0440bef251f904d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:49:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:49:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:50:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:50:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:55:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:55:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:56:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:56:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:56:07 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:56:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:56:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:56:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:19:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 03:19:46 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 03:19:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 03:19:48 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 03:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 03:20:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:23:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 03:23:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:23:30 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 03:23:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 03:23:31 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 03:23:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:23:33 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 03:23:34 GMT
EXPOSE 80
# Tue, 29 Mar 2022 03:23:35 GMT
CMD ["apache2-foreground"]
# Wed, 30 Mar 2022 18:09:33 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 30 Mar 2022 18:09:34 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 30 Mar 2022 18:09:35 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 30 Mar 2022 18:12:01 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 18:12:02 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 30 Mar 2022 18:12:02 GMT
VOLUME [/var/www/html]
# Wed, 30 Mar 2022 18:12:03 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 30 Mar 2022 18:12:04 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Wed, 30 Mar 2022 18:12:43 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 18:12:45 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Wed, 30 Mar 2022 18:12:46 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Wed, 30 Mar 2022 18:12:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 18:12:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04185688a150624b38e612cca7804e1ceb05264548c47b5e039a5a45060aef8`  
		Last Modified: Tue, 29 Mar 2022 05:29:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facd7dc68db6eed96f10a31d88890a6c08ef4187f51e716d240ae17c0cc9d7cb`  
		Last Modified: Tue, 29 Mar 2022 05:29:15 GMT  
		Size: 86.7 MB (86716093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab6336e386feb8448b58a2dd1a285f186c01d4a3bc00b362b2c626f7a835e31`  
		Last Modified: Tue, 29 Mar 2022 05:29:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b8d351d3b53ca329aa303dff2df30307563b8f986a1addebc6bddfa18e59a1`  
		Last Modified: Tue, 29 Mar 2022 05:30:15 GMT  
		Size: 18.9 MB (18943678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22cecadde3e793a43747880bb2ddc3a13b59482ec865ef62356a97ae54a4af`  
		Last Modified: Tue, 29 Mar 2022 05:30:13 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d678ae3151a74648b652849c8cc6049def503b181cc68bc77a2a896e5fe30e1`  
		Last Modified: Tue, 29 Mar 2022 05:30:13 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4498c5ce08d3335b6707c99fe165cd250e9a1634fb4d96bbc0c0b88a14a967`  
		Last Modified: Tue, 29 Mar 2022 05:37:06 GMT  
		Size: 10.9 MB (10895156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1539c2650543bd1062eed026281f5563b52ac5caa7c9c9ad0f2603d7deb295f1`  
		Last Modified: Tue, 29 Mar 2022 05:37:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8dbfbe139e6c5b0aa1fa4b23b45b0cc427b8eeb97095cb447b723d58e1f8e5`  
		Last Modified: Tue, 29 Mar 2022 05:37:05 GMT  
		Size: 10.2 MB (10222010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d85787ee6bb1ccad41b1cc2519b77ad0d2064c24541d1cd778033b6835e6d3`  
		Last Modified: Tue, 29 Mar 2022 05:37:03 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedc217c41471f8a5bd4d358eb26709a594fc22266569d4ef4c95d56c5af5f6f`  
		Last Modified: Tue, 29 Mar 2022 05:37:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66616e09c59b8900fb4ac3b466637c69750e5c7d421977d0989ecea0d5cff52`  
		Last Modified: Tue, 29 Mar 2022 05:37:03 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082cf677c4bfc2313380a951e92beda11620f4da9f44fa6fa7ec9acaf1f92c3d`  
		Last Modified: Wed, 30 Mar 2022 18:19:44 GMT  
		Size: 1.4 MB (1432150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525cc9ac667909fc5487ca8fa0e0230aa9c22a374321a243383874d97702b77`  
		Last Modified: Wed, 30 Mar 2022 18:19:46 GMT  
		Size: 15.1 MB (15068326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc49d2041497273f4341ad36a272491effa2ed957d4edf1b8a19ee1fc19708a5`  
		Last Modified: Wed, 30 Mar 2022 18:19:42 GMT  
		Size: 569.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b2a993e61a316fb9d281afef610ca68ac42ba4452078f0e9d08fc61e72dd5`  
		Last Modified: Wed, 30 Mar 2022 18:19:42 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f869b91e374b819a1537451571cf5cf9d718a9e5038e57b1f8b81702b63e9f`  
		Last Modified: Wed, 30 Mar 2022 18:20:01 GMT  
		Size: 143.3 MB (143280253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48b4b5144ffd19c8775e856c6f42c25106a1df2a2d76c4c661cb775b443964d`  
		Last Modified: Wed, 30 Mar 2022 18:19:42 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ea0b5803b26575a7a26c144fdd3758e96363c71d99cbf8c3600c6a7a92606f`  
		Last Modified: Wed, 30 Mar 2022 18:19:41 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; 386

```console
$ docker pull nextcloud@sha256:7660226ea8219602e5843eba995b8088227be8624de0333badf7f59ec79cf11c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.1 MB (328109862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b15af7913a00ebff7a08299bdf8672f9c2bd8b5e11dea4dc2a4ee042cce90a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

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
# Tue, 29 Mar 2022 01:17:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:17:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:17:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:17:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:17:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:17:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:17:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 01:59:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 19 Apr 2022 00:22:09 GMT
ENV PHP_VERSION=8.0.18
# Tue, 19 Apr 2022 00:22:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Tue, 19 Apr 2022 00:22:11 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Tue, 19 Apr 2022 00:22:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:22:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:25:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 00:25:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:25:03 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 00:25:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 00:25:04 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 00:25:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:25:06 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 00:25:07 GMT
EXPOSE 80
# Tue, 19 Apr 2022 00:25:08 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 05:21:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 19 Apr 2022 05:21:46 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 05:21:47 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 05:24:18 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:24:19 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 05:24:19 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 05:24:20 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 05:24:21 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Tue, 19 Apr 2022 05:25:09 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:25:10 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 19 Apr 2022 05:25:12 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 19 Apr 2022 05:25:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 05:25:14 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:e5f03504ae01782d4552efcd88dac5836f7fdb6e628ef6076e536f44bd3726ba`  
		Last Modified: Tue, 29 Mar 2022 03:20:40 GMT  
		Size: 19.5 MB (19501820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092d9feff8c5c22bf2dfa04dc0622e669df97a9129396f3c60fbbe8c66efafe6`  
		Last Modified: Tue, 29 Mar 2022 03:20:37 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3dd2fa3ed7eaa550087f72d9a21a7cd0385b2967afcd828745e74e0e5c7b67`  
		Last Modified: Tue, 29 Mar 2022 03:20:37 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e407de6c7d320cc1ccbed3b5d2cd47d2d781d4bf6a8d088b54be9a895c826b2`  
		Last Modified: Tue, 19 Apr 2022 01:51:20 GMT  
		Size: 11.0 MB (10995118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cf8d2dfff474f6906f267aa3c12a6ba26ce4947aa27dbd04ec4b068bf38436`  
		Last Modified: Tue, 19 Apr 2022 01:51:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beb89c38087eaa64b1b9b52781fd9410ac89592c7606d3255b95a48fcdaecde`  
		Last Modified: Tue, 19 Apr 2022 01:51:18 GMT  
		Size: 11.0 MB (11034585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b924433bc18e56b5640ca8309a7dc13eb34460a0a6fa9c4375640d32980573`  
		Last Modified: Tue, 19 Apr 2022 01:51:16 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce560f75746448d8302693c2d8ac535a5bae36ac0d501eb4a9198194fd47955`  
		Last Modified: Tue, 19 Apr 2022 01:51:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da726524c2e8547c5fb6b211ccdd94d12b709ba31ee9b0957c1b73c3d47120c9`  
		Last Modified: Tue, 19 Apr 2022 01:51:16 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae366a558641a6e2e69e3d8d3cabc96d1d42bc267ab8e602604c072cb887cf1`  
		Last Modified: Tue, 19 Apr 2022 05:36:54 GMT  
		Size: 1.5 MB (1516474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f746992ef73c9e9c9f822ef42e1e6b360c3c768412df01d48a900252686e7122`  
		Last Modified: Tue, 19 Apr 2022 05:36:56 GMT  
		Size: 16.9 MB (16869636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f5173504f6b9c17e7d88c8bf9129f0d385495c3545f6e9defd5683c9158c8`  
		Last Modified: Tue, 19 Apr 2022 05:36:51 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879d4f5279b3ac2b2ee6ebd331c8fd654aacc8c377d289eeda83772d51321035`  
		Last Modified: Tue, 19 Apr 2022 05:36:51 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2a8aa3cb77d4cbe7e57a011bb2787c5e5c38ec5a127f110460ffc656ba9928`  
		Last Modified: Tue, 19 Apr 2022 05:37:09 GMT  
		Size: 143.3 MB (143280293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2292f7acf6ab8ba361d98807af02ba94fd9a7b3853e09c0c863a673e551210e2`  
		Last Modified: Tue, 19 Apr 2022 05:36:51 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fab755f84f01eb5d88529fb22908d1081d7aaad5eca1f0ff82e278443d0a9d`  
		Last Modified: Tue, 19 Apr 2022 05:36:51 GMT  
		Size: 2.2 KB (2201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; mips64le

```console
$ docker pull nextcloud@sha256:1c504b818e23c097c5536b388606feb3055b502c0dce9e3ccf65fde364f6debd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301063152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d390448076829ea046e7e337dd5c038e3feb10cba26a571fc8465a19e498cbbc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 07:42:27 GMT
ADD file:32aa9fd7ee5c64e4bd49459e801e3e5dc50138590bbfca671e336a197aa7fa92 in / 
# Tue, 29 Mar 2022 07:42:31 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 19:03:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 19:03:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 19:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:05:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 19:05:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 19:19:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 19:19:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 19:20:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 19:20:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 19:21:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 19:21:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 19:21:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 19:21:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 21:17:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 21:17:41 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 21:17:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 21:17:49 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 21:18:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 21:18:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 21:32:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 21:32:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 21:32:21 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 21:32:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 21:32:28 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 21:32:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 21:32:35 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 21:32:38 GMT
EXPOSE 80
# Tue, 29 Mar 2022 21:32:42 GMT
CMD ["apache2-foreground"]
# Thu, 31 Mar 2022 05:28:24 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 31 Mar 2022 05:28:27 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 31 Mar 2022 05:28:31 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 31 Mar 2022 05:40:01 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 05:40:08 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 31 Mar 2022 05:40:12 GMT
VOLUME [/var/www/html]
# Thu, 31 Mar 2022 05:40:19 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 31 Mar 2022 05:40:23 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Thu, 31 Mar 2022 05:43:02 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 05:43:15 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Thu, 31 Mar 2022 05:43:24 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Thu, 31 Mar 2022 05:43:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 05:43:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5c2a8045f9de06328ab3d0ff505d990892219b7faee393bc9ac342347fc83d04`  
		Last Modified: Tue, 29 Mar 2022 07:52:59 GMT  
		Size: 29.6 MB (29641474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241646a732d87181d18d500ef743d5d3a2d6928dee0e4904828284b8f7781bec`  
		Last Modified: Wed, 30 Mar 2022 00:21:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a39d9c931fe7ab8e8a9112a43a8dd9051f2e0c88cb289d2ea4076929ba3514`  
		Last Modified: Wed, 30 Mar 2022 00:22:24 GMT  
		Size: 71.8 MB (71809415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f70f95d116fa6ab27850a082629e46aebd303d2cbbd450d4e07a47b59babf3`  
		Last Modified: Wed, 30 Mar 2022 00:21:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a830fdb776609fbc90ff477336538e0d0d197a763fbfa0b4ce4e072e5dc057`  
		Last Modified: Wed, 30 Mar 2022 00:23:31 GMT  
		Size: 18.9 MB (18933435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc6ef92a058387f9d0fc45394ee63826e21f2d5e9d4ee2fd88af074297be6ae`  
		Last Modified: Wed, 30 Mar 2022 00:23:19 GMT  
		Size: 439.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd7427591217cd607d3b02a04ca7db9bd14cafbdc3921e594766014fb6662af`  
		Last Modified: Wed, 30 Mar 2022 00:23:18 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dc4519c6c3abb851f842a9b89fc354bc1eb142010cf2eda896bfe1ed305fda`  
		Last Modified: Wed, 30 Mar 2022 00:29:19 GMT  
		Size: 10.9 MB (10893878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c10fc433bab5111bcf2a69de34edbeedb80b77d819cd1a0fa1e9abe3bdd0b9`  
		Last Modified: Wed, 30 Mar 2022 00:29:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952691d2f99069c03946b012a8afddc47561667b8df03137b2b0a77dafc7bf9e`  
		Last Modified: Wed, 30 Mar 2022 00:29:22 GMT  
		Size: 9.9 MB (9913484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3a02c6df89dddeeac011673920cbf7a94b6c3725d4d8f72ec1ef6baf4a7a89`  
		Last Modified: Wed, 30 Mar 2022 00:29:14 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd54e2de6a62eb36af041c6f9949a00f2ec569e5a1488b01368e18db1748a8`  
		Last Modified: Wed, 30 Mar 2022 00:29:14 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2953167c0a294ceaa1cbd4d3c54daf7f2842bd1c2491a01d478e7afa73c241`  
		Last Modified: Wed, 30 Mar 2022 00:29:14 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc7d70b2f80573580c4e611807ff945d71d006102f5100c45e71125eaca0387`  
		Last Modified: Thu, 31 Mar 2022 06:07:02 GMT  
		Size: 1.6 MB (1568622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bb2c7b2d76cabd0ed8ce6758d5cf98078ac72ad9d50ad66be2bf402bba66a0`  
		Last Modified: Thu, 31 Mar 2022 06:07:14 GMT  
		Size: 15.0 MB (15010643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fb64139f76dbee555bbd66c5ba8791de971567ff8918257675112202a15f6e`  
		Last Modified: Thu, 31 Mar 2022 06:06:57 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d37345a57444dd5c299cf353a47a329e5eea9231af3a672f1b2438133772747`  
		Last Modified: Thu, 31 Mar 2022 06:06:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9593c92d2de35c260cd1c8baeba294f575d09068e00e45b291f1880071d1d9d`  
		Last Modified: Thu, 31 Mar 2022 06:08:31 GMT  
		Size: 143.3 MB (143280742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f91470b9474e09f2c2078b876ac8671f3e3df45dc8006eb9ac7a031ab58ada`  
		Last Modified: Thu, 31 Mar 2022 06:06:57 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3dc71e7229687f90b519bb656abcfba2f7f6252c108afd998ee9f97ffb43e4`  
		Last Modified: Thu, 31 Mar 2022 06:06:57 GMT  
		Size: 2.2 KB (2203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:81f6deceefb80139b013da26a06c01dacf627e33ea8d7651ea37eb5ae8c6e0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327015972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e76b071fe84a8d91455597e87641796614f1fe7a6cbb9c5fccb46065c23ed26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:19:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:19:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:21:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:21:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:27:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:27:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:28:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:28:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:28:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:28:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:28:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:28:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:43:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 02:43:05 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 02:43:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 02:43:11 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 02:44:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 02:44:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:50:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 02:50:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:50:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 02:50:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 02:50:17 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 02:50:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:50:20 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 02:50:22 GMT
EXPOSE 80
# Tue, 29 Mar 2022 02:50:24 GMT
CMD ["apache2-foreground"]
# Wed, 30 Mar 2022 21:43:06 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 30 Mar 2022 21:43:12 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 30 Mar 2022 21:43:21 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 30 Mar 2022 22:03:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 22:04:08 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 30 Mar 2022 22:04:15 GMT
VOLUME [/var/www/html]
# Wed, 30 Mar 2022 22:04:28 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 30 Mar 2022 22:04:34 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Wed, 30 Mar 2022 22:06:34 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 22:06:42 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Wed, 30 Mar 2022 22:06:45 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Wed, 30 Mar 2022 22:06:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 22:06:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c087cbc2c7d55cf0725407980efe0470467d5dfd4c5658c2127bd0317fde608`  
		Last Modified: Tue, 29 Mar 2022 05:04:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6894e5460431e4ce8d4f063709daa73369a05689921d0cc6896436ea103f76`  
		Last Modified: Tue, 29 Mar 2022 05:05:20 GMT  
		Size: 86.6 MB (86625963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a2eb86a2490b3a6fc39680ea69efc0c28373b420a70b5482adc541e8b8f366`  
		Last Modified: Tue, 29 Mar 2022 05:04:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3efb01d35af6e00fdfb305fa837992b773d71bb3ec8ef8a05af15d85f5cc6b`  
		Last Modified: Tue, 29 Mar 2022 05:06:34 GMT  
		Size: 20.5 MB (20453935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2947ac755e32bf6c4a782e897715296a71cfeb50ec10b45631db62218f0eeb`  
		Last Modified: Tue, 29 Mar 2022 05:06:29 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c4a2e8c312cc99c4e1f371d4bff5828b533bcb94eaf215a5d418a3378aed09`  
		Last Modified: Tue, 29 Mar 2022 05:06:29 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d45f1dd550df1a428fa34d21139ec57e6084e722894d427d45484a459ad4449`  
		Last Modified: Tue, 29 Mar 2022 05:14:32 GMT  
		Size: 11.1 MB (11112537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93618f31d848b7996c07136c3d56dec5e6fde7a41fc86099d2adcd2ba3e09b0`  
		Last Modified: Tue, 29 Mar 2022 05:14:29 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04349e88e9ba2a8b82aba7a36a1d3b291082c7e2f57ad1e98990dfb24e8aa647`  
		Last Modified: Tue, 29 Mar 2022 05:14:31 GMT  
		Size: 11.1 MB (11133785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d4cc7ce2ce997b109b0229b88dc910902962d5437634195ec61ff64b813be0`  
		Last Modified: Tue, 29 Mar 2022 05:14:29 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3714ff63df2c04441101a9eed41d01a1d68d18458551b446969753d6fa15b4`  
		Last Modified: Tue, 29 Mar 2022 05:14:29 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e02c0d2e1409e472a5bdfd4700d5fe0669aa87cb9d513873836f4db432f701`  
		Last Modified: Tue, 29 Mar 2022 05:14:29 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086e76451402570614421e7ae76ef2eff7468867a369854569f03ac4250ac191`  
		Last Modified: Wed, 30 Mar 2022 22:23:11 GMT  
		Size: 1.9 MB (1871318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb755823fbb86282b007f564a83bed3542d9940d0445e8a6e236d419e93257`  
		Last Modified: Wed, 30 Mar 2022 22:23:14 GMT  
		Size: 17.0 MB (17000312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f160f334a72ed23c1d79691802a418fecf423d264628b20ece2f74c521a03357`  
		Last Modified: Wed, 30 Mar 2022 22:23:08 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fa8855dfb608f223701e893355425d328a989ab2449ab0c98b1a2ccd447253`  
		Last Modified: Wed, 30 Mar 2022 22:23:08 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd66dd87c57f8b4c9c555f5232696244d34cc7e9f82e7147eaf74915c8c9b77`  
		Last Modified: Wed, 30 Mar 2022 22:23:33 GMT  
		Size: 143.5 MB (143524026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f5281d15ebde8c7b8277e214b96ebada6d10f2a8e307733f37476cfdff2f6`  
		Last Modified: Wed, 30 Mar 2022 22:23:08 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e69bd1685d4b54d2c4aa41779d1bec8331d432c2161e58b5a444a887eecc615`  
		Last Modified: Wed, 30 Mar 2022 22:23:08 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-apache` - linux; s390x

```console
$ docker pull nextcloud@sha256:e074c5593ef40e8fe078864e94d1d16ea3191f9aa1e91d6f59b2606bf1068991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.9 MB (301855316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a52f0b6e9e1eca5cdfc9f64629ecf7dd0d87e58a67745001cff19e238fdf38d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:21:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 02:21:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 02:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 02:21:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:21:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:24:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 02:24:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 02:24:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 02:24:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 02:24:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 02:24:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:11:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 19 Apr 2022 00:25:48 GMT
ENV PHP_VERSION=8.0.18
# Tue, 19 Apr 2022 00:25:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.18.tar.xz.asc
# Tue, 19 Apr 2022 00:25:49 GMT
ENV PHP_SHA256=db161652cacae4b31c347fbf2e17b80656473cb365f2bb3460c4552f5647e2e7
# Tue, 19 Apr 2022 00:26:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:26:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:30:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 00:30:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:30:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 00:30:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 00:30:29 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 00:30:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:30:30 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 00:30:31 GMT
EXPOSE 80
# Tue, 19 Apr 2022 00:30:32 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 05:03:27 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static         libldap-common     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 19 Apr 2022 05:03:28 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 05:03:28 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 05:05:43 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:05:45 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 05:05:45 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 05:05:46 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 05:05:46 GMT
ENV NEXTCLOUD_VERSION=22.2.6
# Tue, 19 Apr 2022 05:06:33 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:06:42 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 19 Apr 2022 05:06:43 GMT
COPY multi:cc97af471c8139fd0039f75fa22fa380aab666199ee1a1d59d400410f9e63775 in /usr/src/nextcloud/config/ 
# Tue, 19 Apr 2022 05:06:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 05:06:43 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc646829b4b7797b4933a4313f2ac38c99002eb37cf71d4af56a2cfac7913a`  
		Last Modified: Tue, 29 Mar 2022 04:24:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df487a79caa5ca21be0624e6c16cefe85b4350a4a6c39c5f113490ba6ae82a2`  
		Last Modified: Tue, 29 Mar 2022 04:24:31 GMT  
		Size: 71.6 MB (71619822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51d43600a7dc96e3459ca669fa130d53ddd96bd0b420428ab5d6e7f9ba723e8`  
		Last Modified: Tue, 29 Mar 2022 04:24:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a2a1ea2bd50009aff888b17ef0b2beed432e8d5a63a8b882da2cbf9265cea9`  
		Last Modified: Tue, 29 Mar 2022 04:34:26 GMT  
		Size: 19.1 MB (19054463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e270f6d1aa8cc59b2fde320a29a5b077344626bea8bc99d2812bc601b165ec`  
		Last Modified: Tue, 29 Mar 2022 04:34:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef1a1f8227f7c54b9983422c06f616faabea0efae1940602b5b7557bd697254`  
		Last Modified: Tue, 29 Mar 2022 04:34:15 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0c3804b87df2d5e57a8467bd47aee4c2ad4fca698c45d2436e0a2d8e2654cc`  
		Last Modified: Tue, 19 Apr 2022 02:03:48 GMT  
		Size: 11.2 MB (11211366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8dd82bdc5e025cbd595d876b7999266fd124ba9f76603a2d8f7e2527e188e`  
		Last Modified: Tue, 19 Apr 2022 02:03:46 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386124f41183c190769459bd0360261c0ce4f3514369a72db9c7dc981c82296b`  
		Last Modified: Tue, 19 Apr 2022 02:03:48 GMT  
		Size: 10.0 MB (9979320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38177e52034e7c63ca7b4383013312248ad8910ef2206c913e3105369c7a4e`  
		Last Modified: Tue, 19 Apr 2022 02:03:46 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc8bc60fa16099489c11e158fa5bad3c2366aedd612db02d1c6bb2a2f4477e`  
		Last Modified: Tue, 19 Apr 2022 02:03:46 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c84d35eed4b11772848ab223c06010036efb3f79a63b62a731cf508f54c82f`  
		Last Modified: Tue, 19 Apr 2022 02:03:46 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb510b040553b0ad6ea555ed79b3009fe614c779862e65871012de5c72b5e85e`  
		Last Modified: Tue, 19 Apr 2022 05:18:03 GMT  
		Size: 1.7 MB (1659660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16544a03f2d0ff0ae6df48bc5d14f9cc873a344195c41505366e0f74ba35a6bc`  
		Last Modified: Tue, 19 Apr 2022 05:18:05 GMT  
		Size: 15.1 MB (15143470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb07147bf56fb30dfb2564b5360d2f3ab2e5631f3bb519bf1de4efdb0ca83a0`  
		Last Modified: Tue, 19 Apr 2022 05:18:01 GMT  
		Size: 599.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fdc5aff1717923681c91566847ce9e3921390a67bf0295896dc16770c21312`  
		Last Modified: Tue, 19 Apr 2022 05:18:01 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad649e88c5337a7bd036cc302692c957a0f6ac169f8629985acdeed08640369`  
		Last Modified: Tue, 19 Apr 2022 05:18:17 GMT  
		Size: 143.5 MB (143520209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720302fc03b8897d24c6a5e3af989ad9d9e02855f0e49d527e97bf433541a2d9`  
		Last Modified: Tue, 19 Apr 2022 05:18:01 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f0ce334dc1a7315cd1df202da3e8d98dc3991f4415fcfa27e5239cf78dc2eb`  
		Last Modified: Tue, 19 Apr 2022 05:18:02 GMT  
		Size: 2.2 KB (2203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
