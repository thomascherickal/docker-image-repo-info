## `nextcloud:stable`

```console
$ docker pull nextcloud@sha256:4b98cb123cc3152a38e8760adbb05deee949505ccd81227f304d92b47a9a6c43
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

### `nextcloud:stable` - linux; amd64

```console
$ docker pull nextcloud@sha256:3e6795ff57a514a1d40d0a1278dd2386d76b61b270475a54fab4a65b8a097739
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.6 MB (262603414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8ce7cac85e6f828db6534fe119632f9a33566dace051a51c0a5ccd2d1816ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 13:35:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 13:35:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 13:35:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 13:35:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 13:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 13:43:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 13:43:46 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 13:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 13:43:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 13:43:56 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 13:43:56 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 13:43:57 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 13:43:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 13:43:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 13:43:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 14:12:42 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 19:53:58 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 19:53:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 19:53:59 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 19:54:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 19:54:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:00:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 20:00:07 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:00:08 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 20:00:08 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 20:00:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 20:00:09 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 20:00:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:00:09 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 20:00:10 GMT
EXPOSE 80
# Thu, 11 Jun 2020 20:00:10 GMT
CMD ["apache2-foreground"]
# Fri, 12 Jun 2020 02:00:22 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 12 Jun 2020 02:03:19 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 02:03:20 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 12 Jun 2020 02:03:20 GMT
VOLUME [/var/www/html]
# Fri, 12 Jun 2020 02:03:21 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 12 Jun 2020 02:30:45 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Fri, 12 Jun 2020 02:40:38 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 02:40:39 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Fri, 12 Jun 2020 02:40:40 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Fri, 12 Jun 2020 02:40:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Jun 2020 02:40:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0276193a084c10343c4ce4b455dfb8ffc8bfdf6812492ee8307475bac574514`  
		Last Modified: Tue, 09 Jun 2020 15:58:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2d00c10344025e5f7a6826b8e2600cd2f8b89eae906d651f34dbc931baa44c`  
		Last Modified: Tue, 09 Jun 2020 15:58:26 GMT  
		Size: 76.6 MB (76648863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54006e0dc2977f45274054d49dcbbf6494d375b13337a5724d904107e9c64da`  
		Last Modified: Tue, 09 Jun 2020 15:58:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d3d12445921370d9c186b5ad6eeca9bd4f25d0b71185c1632eb44a7192a0fa`  
		Last Modified: Tue, 09 Jun 2020 15:58:51 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60f364b0c5c01784e9cfd217440f8a9ff2bbda1faa94b23b6a613ce00d5e79`  
		Last Modified: Tue, 09 Jun 2020 15:58:46 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e309988c00b7156ba21dcd7154b8042518df210e748c51015dea7b2e48a807c`  
		Last Modified: Tue, 09 Jun 2020 15:58:46 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff5c52c95f4009ffb47db0942c573736c6af70b39235cb6d10e153fe83b634e`  
		Last Modified: Thu, 11 Jun 2020 22:17:06 GMT  
		Size: 12.5 MB (12456462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9086065e8969ad57f43d9339ec26b832bd18371729367dc944c12887bca1d45`  
		Last Modified: Thu, 11 Jun 2020 22:17:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07bb8dcc770ea8b2b2aabf82cc3732089579d979fae390f74036bb88a553083`  
		Last Modified: Thu, 11 Jun 2020 22:17:07 GMT  
		Size: 14.1 MB (14058995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad826bc362350488a284a4ad003b5d5b390b163206693eccc2d52ccaf9ff080`  
		Last Modified: Thu, 11 Jun 2020 22:17:03 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a0743d9734fed09f53ef5ce1dfe4eb01abf00d3dc158bb427e835c10cde70`  
		Last Modified: Thu, 11 Jun 2020 22:17:06 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b190adf511694057657a204e87bb1ca909b8265c6f1e6ad89a0862dec9f906`  
		Last Modified: Thu, 11 Jun 2020 22:17:03 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc02e4c247acb84a43377e2be9106d507a98e88c303ea3c7ebeea23e029f8907`  
		Last Modified: Thu, 11 Jun 2020 22:17:03 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482c10091c25250602db179e63c0d58325b3bd09b83aa7c0c3555010d627a5bf`  
		Last Modified: Fri, 12 Jun 2020 03:31:42 GMT  
		Size: 1.7 MB (1658958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b33a9520149a040cbdc730b86746b27c0983260d8b44b5ff1b4d98dbff80c8`  
		Last Modified: Fri, 12 Jun 2020 03:31:45 GMT  
		Size: 16.2 MB (16198729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07950e773a580ee9c3c837fad9e19279faa9cfdcb16b367c286d3c2b5e87f332`  
		Last Modified: Fri, 12 Jun 2020 03:31:40 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c4504452e10c5fb3757f274c97ce3792d0e5efab2e2fa99d5037140493c08c`  
		Last Modified: Fri, 12 Jun 2020 03:31:40 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6f0cc853b026ebc63651c744a8ddbec7adbb90a18aac467291e18e8b462fda`  
		Last Modified: Fri, 12 Jun 2020 03:33:23 GMT  
		Size: 95.8 MB (95796646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1499f82e421ba38510e9205d778ee8928486c90d4923f49d2b1e38c9c911aaba`  
		Last Modified: Fri, 12 Jun 2020 03:33:03 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a02970bda3ba2ef404125b1523dcfed9fd15448d558a3648d0693bf03588d5`  
		Last Modified: Fri, 12 Jun 2020 03:33:04 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:9174808389b38e5a5a46248a8c88d3a724d7880836fca7095d6f6f1585c1d4d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.4 MB (239354190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895973ee8134a1e76ba00eb4362be5972d6f65e933712bd08fd4ac747decaa87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:10:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 03:10:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 03:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:10:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 03:10:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 03:14:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 03:14:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 03:15:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 03:15:34 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 03:15:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 03:15:36 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 03:15:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 03:15:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 03:15:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 03:15:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 03:33:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 18:41:33 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 18:41:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 18:41:39 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 18:42:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 18:42:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:45:30 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:45:33 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:45:36 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 18:45:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:45:38 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 18:45:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:45:40 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 18:45:41 GMT
EXPOSE 80
# Thu, 11 Jun 2020 18:45:42 GMT
CMD ["apache2-foreground"]
# Thu, 11 Jun 2020 20:43:00 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 11 Jun 2020 20:48:46 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 20:48:50 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 11 Jun 2020 20:48:52 GMT
VOLUME [/var/www/html]
# Thu, 11 Jun 2020 20:48:58 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 11 Jun 2020 20:59:17 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Thu, 11 Jun 2020 21:00:36 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 21:00:40 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 11 Jun 2020 21:00:42 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Thu, 11 Jun 2020 21:00:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Jun 2020 21:00:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c59829855f6b9cf9ed11eac29dfab1d2404aaa7f8271e7b8094fe8fa504826`  
		Last Modified: Tue, 09 Jun 2020 04:43:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b5b6ca74676b662141f56903c72f19688a5a4371073acdce1ff972f5d2b6ab`  
		Last Modified: Tue, 09 Jun 2020 04:43:57 GMT  
		Size: 58.8 MB (58800169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2007b021f74b717a083b49fbc784030ebc6afd3f87f38f0b441253aac4a2fd`  
		Last Modified: Tue, 09 Jun 2020 04:43:35 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab99ab7c53ed09b548fa031932e44905efba42442074ba659ee05509c70359c`  
		Last Modified: Tue, 09 Jun 2020 04:44:24 GMT  
		Size: 18.0 MB (18024799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc3693fde00cab659e05609e2ca0abf20413147758b7902db63f418466017a8`  
		Last Modified: Tue, 09 Jun 2020 04:44:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22971b742bcc572cf190ed570da154e402877b39877f20f574d605122f86643`  
		Last Modified: Tue, 09 Jun 2020 04:44:19 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194eff91ebb3eca033ee7c51a7e9bdbd66b8e5069348379cb41e3021329c8cf7`  
		Last Modified: Thu, 11 Jun 2020 19:23:01 GMT  
		Size: 12.5 MB (12454678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d94086d068ee8d80b4033b41ff90767f0b930e4dab1109faab78b870b539fc`  
		Last Modified: Thu, 11 Jun 2020 19:23:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442c44ad22cf0514e94ee0b07b9b923bb5c598faa75da8ee6e2724d9b6c22878`  
		Last Modified: Thu, 11 Jun 2020 19:23:01 GMT  
		Size: 13.1 MB (13074230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec6e2206e2d80f463bc655c81370f0b428774aa2cf5f4b94060a77c1d7b49b4`  
		Last Modified: Thu, 11 Jun 2020 19:22:58 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9296131c5b2aae14fa8c272f864e64f72c745754d7d10c5fab5da5317d3cdca`  
		Last Modified: Thu, 11 Jun 2020 19:22:59 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237be5451d47cc334f9d2dce23c11dc64758493ad5465b11685303a85c0c9a5e`  
		Last Modified: Thu, 11 Jun 2020 19:22:59 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920dd862a6c1a79d1e9ba4caf4a07518decac8b5c8917e191676ab2f9fa7ba6d`  
		Last Modified: Thu, 11 Jun 2020 19:22:58 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29940114f7bd6269cc5f408b24ef531c418bf29f1b626f4b4cd270583861b1bd`  
		Last Modified: Thu, 11 Jun 2020 21:34:18 GMT  
		Size: 1.6 MB (1596645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98309a154b3829c66ba6a64534d722d0a84ccdb0040c3c6c0642c707e9cc6e0`  
		Last Modified: Thu, 11 Jun 2020 21:34:22 GMT  
		Size: 14.8 MB (14761328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50710fd9fcb64da861f4f2d80610edb56e65ee9a898d0acedc575d92d7f8194`  
		Last Modified: Thu, 11 Jun 2020 21:34:15 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5a070bb08a355a6b3ae3aae8d972f0ffdfbb8de4f073547a39746d7d83ead5`  
		Last Modified: Thu, 11 Jun 2020 21:34:15 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78367f736e1bfb96b2a66332f4b30b8e92861ad7cb5dbf84025ee33300184bc5`  
		Last Modified: Thu, 11 Jun 2020 21:36:03 GMT  
		Size: 95.8 MB (95794438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fec6aa0f8acd3f2558845e910749928373dc8d18c4f4cba035a26465476fe7`  
		Last Modified: Thu, 11 Jun 2020 21:35:26 GMT  
		Size: 2.5 KB (2525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7909f7afc3e2ee9a4c10157b67da1140b5b054a23beda26d370e4ba0943ea9b9`  
		Last Modified: Thu, 11 Jun 2020 21:35:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:223246e8ab4864ee8782b8482d9808224b89392245f95e7032a7cdcdd31af82b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235513894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe4366d5ad399a3baf984c2b09e6aa2a7b75caaebe6b04b78d1988b58d6916b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 09:38:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 09:38:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 09:39:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 09:39:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 09:39:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 09:43:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 09:43:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 09:43:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 09:43:34 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 09:43:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 09:43:38 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 09:43:40 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 09:43:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 09:43:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 09:43:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 09:59:53 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 19:00:56 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 19:01:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 19:01:05 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 19:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 19:01:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:04:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:04:45 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:04:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:04:58 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 19:05:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:05:02 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 19:05:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:05:07 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 19:05:10 GMT
EXPOSE 80
# Thu, 11 Jun 2020 19:05:12 GMT
CMD ["apache2-foreground"]
# Fri, 12 Jun 2020 00:02:15 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 12 Jun 2020 00:06:58 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 00:07:01 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 12 Jun 2020 00:07:02 GMT
VOLUME [/var/www/html]
# Fri, 12 Jun 2020 00:07:04 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 12 Jun 2020 00:18:45 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Fri, 12 Jun 2020 00:19:36 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 00:19:41 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Fri, 12 Jun 2020 00:19:43 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Fri, 12 Jun 2020 00:19:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Jun 2020 00:19:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06dc047a60bc8c7f6dd7236a59edd0ac74556e9f9a4375cd2d64e1b5ef56dd`  
		Last Modified: Tue, 09 Jun 2020 11:11:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8445ea067b9b6c8bbaff4521c1fcd1b8e9cbcf970e9144d4d3d4ec2a419b83ea`  
		Last Modified: Tue, 09 Jun 2020 11:11:45 GMT  
		Size: 59.5 MB (59505705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3427b10e03731502c05abd929b3f5877453d9bd99926d1c7fd6454d036781a0`  
		Last Modified: Tue, 09 Jun 2020 11:11:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34345889541e5a3064f962af2fd34100dcda9d5fa472610f39e81e1dedfaabc2`  
		Last Modified: Tue, 09 Jun 2020 11:12:14 GMT  
		Size: 17.5 MB (17481931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53401c3488310a3bb0ec1ba3f8292c2e073b6c48cfb5ed4f3d54c8b6d3b5634a`  
		Last Modified: Tue, 09 Jun 2020 11:12:09 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4089189859792978c711aea78a5530956e07c24ba5cb5a9d3fa3cd28bcdf3e1`  
		Last Modified: Tue, 09 Jun 2020 11:12:09 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f1ab648e4b64f5dffa747fafb7216c57a1366751ae3b16d12b572929cfadc`  
		Last Modified: Thu, 11 Jun 2020 20:15:12 GMT  
		Size: 12.5 MB (12454681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b85ef71509c17576603514ce4ba6a8a72f250bd9db5ac7d0e929ed9c8678b3`  
		Last Modified: Thu, 11 Jun 2020 20:15:08 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea38911e7425de6ee1d1e02a020f467fd28623b4545392a19e465d893849982`  
		Last Modified: Thu, 11 Jun 2020 20:15:14 GMT  
		Size: 12.4 MB (12370879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f86f17ecae80c7be69822117938445959742e506ecfee20e0b37f38df97ba7`  
		Last Modified: Thu, 11 Jun 2020 20:15:07 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bca6db9a4da7414faa66fd57905c586257373a42808ff074b1ca1eea482ab95`  
		Last Modified: Thu, 11 Jun 2020 20:15:07 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463b282825c90550afe89292c32f02e68d4d70a2959b497a71da2171bd47c5bc`  
		Last Modified: Thu, 11 Jun 2020 20:15:07 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c5fa73d3924380a276ab652125f0d9847c4c97b9ed53717c2f7af061af906e`  
		Last Modified: Thu, 11 Jun 2020 20:15:07 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32228917f79e3c66aa7209dc9d2207ff1d3a70114c413263624384a1293a29c8`  
		Last Modified: Fri, 12 Jun 2020 00:42:58 GMT  
		Size: 1.4 MB (1448711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9145b62dbd0c40ac44fe86ef742d74d9c89931e5366fd78076a0aff44a83b`  
		Last Modified: Fri, 12 Jun 2020 00:43:01 GMT  
		Size: 13.7 MB (13740982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa32cb8c0b8bbe3f8c7a59b173efcc37b3dba1d2bef541968451e672e87e041`  
		Last Modified: Fri, 12 Jun 2020 00:42:56 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9e81d5514b6ffac707193787b29540652090a68e3a3cb6a0f948f5e8e98d8`  
		Last Modified: Fri, 12 Jun 2020 00:42:56 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf75e966ee231688557502a6e516e1469b88b48ded9943a007bcae9ef792508`  
		Last Modified: Fri, 12 Jun 2020 00:45:15 GMT  
		Size: 95.8 MB (95794438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b46cd698c6cc3c2b44716b45a459878a35066e4f0d8183d52a0b96912df836`  
		Last Modified: Fri, 12 Jun 2020 00:44:47 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9424e1d085ed3f27888e4377e9a4d0839f6d89cb9f18b76469594e0a4f5050`  
		Last Modified: Fri, 12 Jun 2020 00:44:47 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:c69c59b1993ec4f4fa4986c5a6489026d8a8bd738320b505e7823d1e6af2d4d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252933077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eca3bc4f150e9856c9d60bb3ffaeaae581bc02221eb051e4e065635a96fd451`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 10:22:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 10:22:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 10:23:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 10:23:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 10:23:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 10:27:53 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 10:27:53 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 10:28:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 10:28:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 10:28:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 10:28:24 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 10:28:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 10:28:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 10:28:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 10:28:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 10:48:27 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 19:14:22 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 19:14:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 19:14:27 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 19:14:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 19:14:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:18:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:18:53 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:18:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:19:00 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 19:19:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:19:02 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 19:19:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:19:04 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 19:19:05 GMT
EXPOSE 80
# Thu, 11 Jun 2020 19:19:06 GMT
CMD ["apache2-foreground"]
# Fri, 12 Jun 2020 00:53:23 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 12 Jun 2020 01:00:35 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 01:00:48 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 12 Jun 2020 01:00:52 GMT
VOLUME [/var/www/html]
# Fri, 12 Jun 2020 01:00:58 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 12 Jun 2020 01:14:38 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Fri, 12 Jun 2020 01:15:29 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 01:15:33 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Fri, 12 Jun 2020 01:15:35 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Fri, 12 Jun 2020 01:15:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Jun 2020 01:15:37 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e42a0c192db5b0cb97d83007911b8069b7120ef4d150564a32e9ec94753ca03`  
		Last Modified: Tue, 09 Jun 2020 11:57:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23edfc2b677695687c477af83edbcfb24140f7186ed405faef4d5947c0a0c9`  
		Last Modified: Tue, 09 Jun 2020 11:57:42 GMT  
		Size: 70.3 MB (70337397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22952435701f91bcb4b63b22ba1c37c84d3a2c0d2f3c98109e18618040b7bb32`  
		Last Modified: Tue, 09 Jun 2020 11:57:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4090b847c63cf622d705238850718bfaa914a66c26c09c72b4d9799d275f05`  
		Last Modified: Tue, 09 Jun 2020 11:58:10 GMT  
		Size: 18.6 MB (18579309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb37ac8c34eaa4fd0192c5f0d5fa5ba67a1be74bdb0715850f35818fad6ee35`  
		Last Modified: Tue, 09 Jun 2020 11:58:05 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a637d0146b6020a2407694c81449ec07e33b411830a64f1b7bf3a652ec302adf`  
		Last Modified: Tue, 09 Jun 2020 11:58:05 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1044a9b004fa9ece5ad2d7f2a8cd55c9ba464abf84dffea93742a1c74a533e71`  
		Last Modified: Thu, 11 Jun 2020 20:32:21 GMT  
		Size: 12.5 MB (12455334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1188ef46e090f2d3cb74867e46e0ee85d8601c8894a39f4aeb38d8f63530d2`  
		Last Modified: Thu, 11 Jun 2020 20:32:18 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fea05a4d5283e89cf15eb6e8a869407cba152f568a9b5819cc165876154e452`  
		Last Modified: Thu, 11 Jun 2020 20:32:21 GMT  
		Size: 13.7 MB (13742021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9646b6a0b558e60a65e07e3381d27f7bc2aa34ac891a8596183f0f7cfa40df`  
		Last Modified: Thu, 11 Jun 2020 20:32:17 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ead19c0409d0e3ad7020f38425f89d3dfdd95a0feff190fbfb4e681b364cbd`  
		Last Modified: Thu, 11 Jun 2020 20:32:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24ad6bf84308279499bccb03a95f199beb61e75fd447d1cf19cfdab67b21b78`  
		Last Modified: Thu, 11 Jun 2020 20:32:17 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53beea2e0d2a751fa08e4ea0cb12d9ca7348b068e2b7618d52c7bf5da9ce9739`  
		Last Modified: Thu, 11 Jun 2020 20:32:17 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181ed46c94cde213e93efda241fecfcefee06f04173f6c23a2f11d3c8461aa78`  
		Last Modified: Fri, 12 Jun 2020 01:39:43 GMT  
		Size: 1.6 MB (1625513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cbfae40fad4dbf3ddbd3828ee1137d1a4f17e95e6b0a1ba24d049c449cfe28`  
		Last Modified: Fri, 12 Jun 2020 01:39:47 GMT  
		Size: 14.5 MB (14529217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7b8c5508b592289df9e9e254f415db89f06eaaa42414ca38f0ecada31ef922`  
		Last Modified: Fri, 12 Jun 2020 01:39:43 GMT  
		Size: 532.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78764eb06cfd84f43161c394f3393c45917576aaa3941d095719300bbf6faab9`  
		Last Modified: Fri, 12 Jun 2020 01:39:42 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599b4d10bc25e0acc7a1a967f5894c8f45118160edbfbadcf6d1f7f11cba68bd`  
		Last Modified: Fri, 12 Jun 2020 01:41:51 GMT  
		Size: 95.8 MB (95795921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8234086b1908cd3aad5d1bdf59a02d314359bd6eef5646bb7b96972f7db4f252`  
		Last Modified: Fri, 12 Jun 2020 01:41:21 GMT  
		Size: 2.5 KB (2525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48e8d139e957691236dd4284b88a1446a504966eff21e08bac6180655377705`  
		Last Modified: Fri, 12 Jun 2020 01:41:21 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; 386

```console
$ docker pull nextcloud@sha256:8dcbbcc4750b89186a141bf3a938c5fed45da6ff83eaa37f52f14a95f5ba027e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267913604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0b25cd9845e7c31c8580248fc4a038f69a55a4b195f734ed7bab99c8b0ef9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:29:01 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 07:29:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 07:29:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 07:29:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 07:29:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 07:36:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 07:36:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 07:36:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 07:36:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 07:36:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 07:36:21 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 07:36:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 07:36:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 07:36:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 07:36:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 08:01:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 20:00:52 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 20:00:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 20:00:52 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 20:01:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 20:01:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:07:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 20:07:31 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:07:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 20:07:33 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 20:07:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 20:07:33 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 20:07:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:07:33 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 20:07:34 GMT
EXPOSE 80
# Thu, 11 Jun 2020 20:07:34 GMT
CMD ["apache2-foreground"]
# Fri, 12 Jun 2020 02:24:23 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 12 Jun 2020 02:27:05 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 02:27:06 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 12 Jun 2020 02:27:06 GMT
VOLUME [/var/www/html]
# Fri, 12 Jun 2020 02:27:07 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 12 Jun 2020 02:55:14 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Fri, 12 Jun 2020 03:03:51 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 03:03:52 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Fri, 12 Jun 2020 03:03:53 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Fri, 12 Jun 2020 03:03:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Jun 2020 03:03:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56aaa35138d917890d6385d97e3551b2c7f733e0ffb4190f8ab0926d45535d`  
		Last Modified: Tue, 09 Jun 2020 09:59:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cde5a58e2a1076acb6f13762ae3b1f732448e2f9fdef2e266ca694f8699139`  
		Last Modified: Tue, 09 Jun 2020 10:00:10 GMT  
		Size: 81.2 MB (81195220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b360659c28c29c8e5663391e3f169aee77802ea8c4fdc2aa8d23201818fcaae`  
		Last Modified: Tue, 09 Jun 2020 09:59:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd23cd61177bdbdcc4db1030fc9f13b5ea125fcafab4fc880ea4e64f9ceb40`  
		Last Modified: Tue, 09 Jun 2020 10:00:41 GMT  
		Size: 19.1 MB (19112646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3fdcec853cb1f90ba0e4a79a68c0b1907af37893288b77faf0a68bf50fe7cd`  
		Last Modified: Tue, 09 Jun 2020 10:00:32 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d180d5d8242623311c0d71ed5fbef0b5135bb9833d4512f953833d89cfc53`  
		Last Modified: Tue, 09 Jun 2020 10:00:32 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160c93e34c645532d2405552623a47b0ced59f8a7bbf7cf16adc79341df85b9`  
		Last Modified: Thu, 11 Jun 2020 22:30:51 GMT  
		Size: 12.5 MB (12455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae189c13cc7607de07b56a566d6498a25478926040c1d591a8e6299bac1524e`  
		Last Modified: Thu, 11 Jun 2020 22:30:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcea790670d2cf67d1fb3cd50d31ff8c678395539a7462c75807c6a7c84f3ded`  
		Last Modified: Thu, 11 Jun 2020 22:30:54 GMT  
		Size: 14.4 MB (14375450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdc613f5cc02fa8ce7e15a0068f9de1436cb22fe851827e5cefd7c83c3398c8`  
		Last Modified: Thu, 11 Jun 2020 22:30:48 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15bce4d2e0f2e9fc7085fca418c243d839ac572c2c4b5f0dfbcb3c6c1fd8efa`  
		Last Modified: Thu, 11 Jun 2020 22:30:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5006afd69ba776e549922de6ef59d42d208460f3b5dbb83a533ab05eabe9f701`  
		Last Modified: Thu, 11 Jun 2020 22:30:47 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c3f58356337dd51f8421a82f3a7ce2a6a0b6a52e8c57175e3e733caa7a9814`  
		Last Modified: Thu, 11 Jun 2020 22:30:47 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e438628b366feacf0c6208bfb860cc606173e8e7d5ffe9c2932b2d1826c8bb`  
		Last Modified: Fri, 12 Jun 2020 03:48:50 GMT  
		Size: 1.7 MB (1682775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebb18c90ea744d2d9b2ff84e72d6b374e49cc819a1103e362410bd1dd0909f2`  
		Last Modified: Fri, 12 Jun 2020 03:48:54 GMT  
		Size: 15.5 MB (15530563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda3bfb346cc64be3dba13c9f0fd95e18745c8b35d787a4ebd68539dc2df6769`  
		Last Modified: Fri, 12 Jun 2020 03:48:48 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7b4207400614fc726a73ac06ffcdde7f8d65b9dfb450263156b547c2f35751`  
		Last Modified: Fri, 12 Jun 2020 03:48:48 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae73c18aa27dc35d34c6fd0edd8878a4cb965fe60c87eb38bf6d4278aa094c6`  
		Last Modified: Fri, 12 Jun 2020 03:50:59 GMT  
		Size: 95.8 MB (95795762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1199471851bcac1c35db495e6fadbb19dde97b703a3ffc67c4f9004d67424b53`  
		Last Modified: Fri, 12 Jun 2020 03:50:29 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600e146887270404c366571a251b9f38284bd4346c1160fa83123e641a520677`  
		Last Modified: Fri, 12 Jun 2020 03:50:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; mips64le

```console
$ docker pull nextcloud@sha256:8146d7d84dd381b98035a9f015c6419ce5f69f88d88b1685b827006904a3e014
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.7 MB (243705355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35ffb160d35ce2f909ecac3dab38ab74701e11cb706f0c198f95f92479901dd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:10:06 GMT
ADD file:faf18b832680e98050b98c329add242425904e64c6a5a491c22d33e9417ef323 in / 
# Tue, 09 Jun 2020 01:10:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:28:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 03:28:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 03:29:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:29:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 03:29:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 03:45:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 03:45:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 03:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 03:46:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 03:46:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 03:46:24 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 03:46:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 03:46:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 03:46:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 03:46:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 04:47:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 19:31:53 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 19:31:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 19:31:53 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 19:32:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 19:32:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:42:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:42:29 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:42:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:42:34 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 19:42:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:42:34 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 19:42:35 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:42:35 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 19:42:35 GMT
EXPOSE 80
# Thu, 11 Jun 2020 19:42:36 GMT
CMD ["apache2-foreground"]
# Thu, 11 Jun 2020 22:54:38 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 11 Jun 2020 23:02:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 23:02:53 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 11 Jun 2020 23:02:53 GMT
VOLUME [/var/www/html]
# Thu, 11 Jun 2020 23:02:56 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 11 Jun 2020 23:14:51 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Thu, 11 Jun 2020 23:16:24 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 23:16:27 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 11 Jun 2020 23:16:29 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Thu, 11 Jun 2020 23:16:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Jun 2020 23:16:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:76f2a0c8ea98ebd699a77ced9c677e97cd54b038a8c5e89670af78f38b047b33`  
		Last Modified: Tue, 09 Jun 2020 01:18:14 GMT  
		Size: 25.8 MB (25764040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66057b0e3024c84ecd4fde2e861cd01182c33e645370ffbfbecd3e939835a2b2`  
		Last Modified: Tue, 09 Jun 2020 06:33:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c8820ce45f9089ffda8e85c4969f694f892adc1c74edd416e85be67bfa35f4`  
		Last Modified: Tue, 09 Jun 2020 06:34:45 GMT  
		Size: 61.4 MB (61387138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4898d95a55bf57000442bb8618a50d70a49721758e2e1e057fab8c0113e1ed14`  
		Last Modified: Tue, 09 Jun 2020 06:33:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4b400703521b2010d3a9bbdcab2a53f9446504117c28266176999ae3b19ef6`  
		Last Modified: Tue, 09 Jun 2020 06:35:51 GMT  
		Size: 18.6 MB (18606033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d7c3e9870eaf6641c9e124721e5d1affee39a644b9f3abe2582ea14422d183`  
		Last Modified: Tue, 09 Jun 2020 06:35:36 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2d6c709b1806cc619f5db3923e00a56c9697142ff5e14f09e63e03eaadd540`  
		Last Modified: Tue, 09 Jun 2020 06:35:36 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e2d138efbfa9d05cdcba9729207c3bca9fc078a4894f0d5e4d2517e9685971`  
		Last Modified: Thu, 11 Jun 2020 21:24:56 GMT  
		Size: 12.5 MB (12453882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de3f6bbd5092f1b780e5b7187bba31cf515cca0cae0b40af1233a1701c6ae97`  
		Last Modified: Thu, 11 Jun 2020 21:24:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2945d78d8af7c163338c40de1737804422b029aff6a04effeab5fa69cd87dc5b`  
		Last Modified: Thu, 11 Jun 2020 21:25:07 GMT  
		Size: 13.3 MB (13335924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acac600c2267b05d9b721edab9f0143052f5e5797c2e6b3000c48f3cfed9261f`  
		Last Modified: Thu, 11 Jun 2020 21:24:50 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d33259c3c23498442a8f35e200e70574a9e59c9c1ebd079c3ccd2ca86d9eeeb`  
		Last Modified: Thu, 11 Jun 2020 21:24:50 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ec012d15f7a58cd06b9431db813ce126ce2122d2bb4c433d89e9fc496e28a4`  
		Last Modified: Thu, 11 Jun 2020 21:24:50 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33775b0c38ba2fde809632f79e5559612b534c10f4777b16cde87e1ace96f72e`  
		Last Modified: Thu, 11 Jun 2020 21:24:49 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a80ff8dfe89b1aadff199d5230f7a78ddcab26c8e9de912ac52f61a5224b125`  
		Last Modified: Thu, 11 Jun 2020 23:42:17 GMT  
		Size: 1.8 MB (1763108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87735f9e97863b9e0ec5028e90eb3946bceefd35c18cff153d22bc11e836c02d`  
		Last Modified: Thu, 11 Jun 2020 23:42:29 GMT  
		Size: 14.6 MB (14590215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c489205d3f46c3477f9c776003f26fe9474ab611e9d08db489c8a416696438e6`  
		Last Modified: Thu, 11 Jun 2020 23:42:12 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cdb45965fa0dc55006f2ac4e29f39f7e38a8d6138d660f975a657bd5b5fcfc`  
		Last Modified: Thu, 11 Jun 2020 23:42:12 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2503bb0498f08eb7b1fd887c04597667bd4de28666cd7777928d7954d9e8369`  
		Last Modified: Thu, 11 Jun 2020 23:46:05 GMT  
		Size: 95.8 MB (95794510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d7441aff2aef80a5b08f337d9bf36af4a17317080e7d4e38296f502c42a49`  
		Last Modified: Thu, 11 Jun 2020 23:44:56 GMT  
		Size: 2.5 KB (2523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f832a86aea913a28c6407f4145093db3d0da22b0c4187f0ac40354e0bf10680`  
		Last Modified: Thu, 11 Jun 2020 23:44:56 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:08788012e3fb18e97082a55177498ff5c7af77de0f4847eceb9419999bf478e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.2 MB (274178672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b54195f97ed4ecf82c54c137f3f1fded10a86c6f25aaba2d25a3f073ddbc5e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 05:09:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 05:09:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 05:11:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 05:11:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 05:11:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 05:17:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 05:17:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 05:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 05:18:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 05:19:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 05:19:03 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 05:19:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 05:19:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 05:19:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 05:19:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 05:48:17 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 19:20:08 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 19:20:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 19:20:17 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 19:21:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 19:21:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:25:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:25:23 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:25:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:25:41 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 19:25:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:25:48 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 19:25:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:25:52 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 19:25:55 GMT
EXPOSE 80
# Thu, 11 Jun 2020 19:25:58 GMT
CMD ["apache2-foreground"]
# Thu, 11 Jun 2020 23:35:10 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 11 Jun 2020 23:42:35 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 23:42:40 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 11 Jun 2020 23:42:42 GMT
VOLUME [/var/www/html]
# Thu, 11 Jun 2020 23:42:47 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 12 Jun 2020 00:01:05 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Fri, 12 Jun 2020 00:05:43 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 12 Jun 2020 00:05:53 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Fri, 12 Jun 2020 00:06:01 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Fri, 12 Jun 2020 00:06:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Jun 2020 00:06:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad44f0796ea364793d3ac145c002c7ed180fe56cd09eed97a971a2e20999794`  
		Last Modified: Tue, 09 Jun 2020 08:55:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501de6851c5eeb5b1bd75588fa67abb74d85b869f36d4815f1e4ae4e007fc4f1`  
		Last Modified: Tue, 09 Jun 2020 08:56:28 GMT  
		Size: 82.3 MB (82262725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4824564d8a89ca8405d5fcf32fb84ff63852689cf385a5bcffa8023a86fa4a69`  
		Last Modified: Tue, 09 Jun 2020 08:55:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99532398782658ac58577cecae6ae5f90b9b6e04b25df6a369510bcea7b411ec`  
		Last Modified: Tue, 09 Jun 2020 08:57:27 GMT  
		Size: 19.8 MB (19812684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30f5e03cf0ea1fb57a099769f112d8c96d3cb625b7d6a3ae17c001cdfcf1`  
		Last Modified: Tue, 09 Jun 2020 08:57:15 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61fef0479b4be6972b0063d25644a438b9427dd75421d9166d822ae7bdf81c3`  
		Last Modified: Tue, 09 Jun 2020 08:57:15 GMT  
		Size: 522.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45e94c45ce2d45cccfcf398100efae34c889e734bcae5baadf4f280bf65a1bb`  
		Last Modified: Thu, 11 Jun 2020 21:00:35 GMT  
		Size: 12.5 MB (12456332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5867a7582d1b32f1858072dad1f2523fc611a583ab5bc7c5e22f5ccf45b9b78d`  
		Last Modified: Thu, 11 Jun 2020 21:00:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf4d0ea2b0e1aec90cb7db5b52e664a84050c8c9fd61a4c719605853ca9c94c`  
		Last Modified: Thu, 11 Jun 2020 21:00:32 GMT  
		Size: 15.1 MB (15099476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0119703c547e825e0f20f43aba5f7580c658dbd66ba07ce2c00f1a7d328763a`  
		Last Modified: Thu, 11 Jun 2020 21:00:27 GMT  
		Size: 2.3 KB (2287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67ca084637ca611a057ab267ad20937b11546be6cc5c781ade0b4553b02c2c6`  
		Last Modified: Thu, 11 Jun 2020 21:00:27 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51ca374380053fa9432b5b9e33e5509b6cc220c78da1b2c35b9bf9631fbd3eb`  
		Last Modified: Thu, 11 Jun 2020 21:00:27 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c14845c1b8a66f4830796440af7ed8f586c72c086353d6a1b98537dce71d6`  
		Last Modified: Thu, 11 Jun 2020 21:00:27 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a2ec27d9fea89b36e8998c30112d8abc0b0dee9f2db6a6b6387bf51a09ef89`  
		Last Modified: Fri, 12 Jun 2020 00:48:34 GMT  
		Size: 1.8 MB (1826363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758dee8e584028196b7c26b7ea456f7cf2a563b718799ed38dfdca8746a4601c`  
		Last Modified: Fri, 12 Jun 2020 00:48:45 GMT  
		Size: 16.4 MB (16387762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a999daf5f5df487f5105472306881f5b87a3226974a3b9a8ccdda994f0ab5392`  
		Last Modified: Fri, 12 Jun 2020 00:48:30 GMT  
		Size: 534.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4687d3aeceb3abfea2159edef468d4656310859aeef417881a95ae2f77db46d8`  
		Last Modified: Fri, 12 Jun 2020 00:48:30 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642681577e2712a51e7b1ece9621cb45571eac22fdf268b4dd5fb7552f7f212e`  
		Last Modified: Fri, 12 Jun 2020 00:54:12 GMT  
		Size: 95.8 MB (95798262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57919137a2cb667bd5cc9e93315859abb2ac98d48636b9bd3b7de82f615204`  
		Last Modified: Fri, 12 Jun 2020 00:53:41 GMT  
		Size: 2.5 KB (2525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e2f79ea1fbccefab375a314d4561616511988d600ec981e7968f9f88c1ed85`  
		Last Modified: Fri, 12 Jun 2020 00:53:41 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable` - linux; s390x

```console
$ docker pull nextcloud@sha256:975d17ff82ff69107c52a0475c9af3019083a654bb8378c25f1b401cdc396f72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.8 MB (246778222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199b057e8b42b122dcdb57ab150920fb9aa6f4ae00b718e7a2103f4a855d4915`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:37 GMT
ADD file:b21d426de40a194c6c76ed27593f33fb1ea470e15d4d43b00d7601472110de1a in / 
# Tue, 09 Jun 2020 01:42:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:37:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 06:37:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 06:38:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 06:38:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 06:38:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 06:40:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Jun 2020 06:40:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Jun 2020 06:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Jun 2020 06:40:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Jun 2020 06:40:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Jun 2020 06:40:33 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Jun 2020 06:40:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Jun 2020 06:40:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 06:40:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 06:40:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 06:49:37 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 11 Jun 2020 18:47:53 GMT
ENV PHP_VERSION=7.3.19
# Thu, 11 Jun 2020 18:47:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.19.tar.xz.asc
# Thu, 11 Jun 2020 18:47:54 GMT
ENV PHP_SHA256=6402faa19b1a8c4317c7612632bce985684a5bbae0980a5779a4019439882422 PHP_MD5=
# Thu, 11 Jun 2020 18:48:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 11 Jun 2020 18:48:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:49:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:49:32 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:49:33 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:49:33 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 11 Jun 2020 18:49:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:49:34 GMT
STOPSIGNAL SIGWINCH
# Thu, 11 Jun 2020 18:49:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:49:34 GMT
WORKDIR /var/www/html
# Thu, 11 Jun 2020 18:49:34 GMT
EXPOSE 80
# Thu, 11 Jun 2020 18:49:34 GMT
CMD ["apache2-foreground"]
# Thu, 11 Jun 2020 21:52:35 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 11 Jun 2020 21:54:30 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 21:54:31 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 11 Jun 2020 21:54:31 GMT
VOLUME [/var/www/html]
# Thu, 11 Jun 2020 21:54:32 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 11 Jun 2020 22:00:01 GMT
ENV NEXTCLOUD_VERSION=18.0.6
# Thu, 11 Jun 2020 22:00:37 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 11 Jun 2020 22:00:45 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 11 Jun 2020 22:00:46 GMT
COPY multi:33e77d62bcc8d3785b05ff335da53732e518a402288e1ca59e572a0f6fd75aff in /usr/src/nextcloud/config/ 
# Thu, 11 Jun 2020 22:00:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Jun 2020 22:00:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:405e75bf6bb0104d67fcebf58e07cd21bf344589df9c1a41c00354a60ea3a604`  
		Last Modified: Tue, 09 Jun 2020 01:46:30 GMT  
		Size: 25.7 MB (25712668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dab5ec1d9ed4e6ade1e7c68e458251c8a79a69d2ec7d423210d68de7840a48`  
		Last Modified: Tue, 09 Jun 2020 07:51:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098d3fb4981972309584ef3f5804808f74198493492dbfbcedffab5aa8ec88f0`  
		Last Modified: Tue, 09 Jun 2020 07:51:44 GMT  
		Size: 64.7 MB (64698115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd389fe6334989b50fd7ae261df2710def59b4d1e379d843feea09f0ba083e`  
		Last Modified: Tue, 09 Jun 2020 07:51:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd35d993db3e5a287580b6ec35918249181ceaf28c4b7538240edf1dfe1d92c`  
		Last Modified: Tue, 09 Jun 2020 07:52:14 GMT  
		Size: 18.5 MB (18522535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3f7720a66884179a2578d0b4025070541736e594d5f212445d65225117f232`  
		Last Modified: Tue, 09 Jun 2020 07:52:09 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4378c6dc9fbfabc6567ae9c8b82f3fe016ed07e5d693adffcd062f6e91a23e6`  
		Last Modified: Tue, 09 Jun 2020 07:52:08 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e88caa7666b5eff6e2284042f171ec53ddaecf36f174109979d70f0842d2f4`  
		Last Modified: Thu, 11 Jun 2020 19:34:41 GMT  
		Size: 12.5 MB (12454928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39db448b7d3fccb5274023337d9a4b33bb35be5467d7b5cafa5835a1f0fa2bc`  
		Last Modified: Thu, 11 Jun 2020 19:34:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481884fef6a3811c804ce1b12b20a8280db970e7336ac4ffb4ada7797e63a2bc`  
		Last Modified: Thu, 11 Jun 2020 19:34:41 GMT  
		Size: 13.3 MB (13290685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de579acb8a6ab96e1ab0c4cf6157da3cb02fedff4878944af94cab2d892b53f4`  
		Last Modified: Thu, 11 Jun 2020 19:34:38 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab67d89916664a10f4d0d4f78f020c83390e88d0c2171f288d6009d5587b667c`  
		Last Modified: Thu, 11 Jun 2020 19:34:38 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86651e741312ee2faa73b11f31c93ab61d8c0a84dce802114e424d6e462d66aa`  
		Last Modified: Thu, 11 Jun 2020 19:34:38 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4419e6963cf67a499699b22c2179a88efee7f75abf8015393d39a3cfa02afdfe`  
		Last Modified: Thu, 11 Jun 2020 19:34:44 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd10355825ab090fc829a6a67b1639ab06b6ab68997604d9972e95441c2f85`  
		Last Modified: Thu, 11 Jun 2020 22:13:39 GMT  
		Size: 1.6 MB (1618100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c830eb7616a9095993d48bf6ea3c153a5b72e5fcf7a8214fd31530ae01020cb5`  
		Last Modified: Thu, 11 Jun 2020 22:13:41 GMT  
		Size: 14.7 MB (14676337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e127766c52ec96de5a92fa8f902dd44884f76fb7d5b24ffd5ac0e55fb246fd`  
		Last Modified: Thu, 11 Jun 2020 22:13:38 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdcbbfa49730e187fae7ea998b66d78338917f4aef4c832ce964d31673d7c15`  
		Last Modified: Thu, 11 Jun 2020 22:13:38 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857c461d0cdc6685344c4f58966cc4eaa3e07c98a020d8e7384da97809a8f7fc`  
		Last Modified: Thu, 11 Jun 2020 22:15:01 GMT  
		Size: 95.8 MB (95794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94293eb95181dcd571a1f46ba018364e0709620e195df0aa759b05bd51334055`  
		Last Modified: Thu, 11 Jun 2020 22:14:50 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245fa21037426afd633f0f6522997b8a27b521605d7b460f405b35fc2c7fd37e`  
		Last Modified: Thu, 11 Jun 2020 22:15:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
