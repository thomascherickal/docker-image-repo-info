## `nextcloud:17-apache`

```console
$ docker pull nextcloud@sha256:aa54274641ace16d140d65cd8eb32fd3d7d889baf82ea19ffadf91e2be0837d6
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

### `nextcloud:17-apache` - linux; amd64

```console
$ docker pull nextcloud@sha256:e9eadcfa1d50192c143b9b4248e65c9e7829d28b65b0f3a180b4e6eb23d5bbae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.1 MB (240129642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298e8038628540d33440abe4cf67b23362d8c657c7bd95f181e0c4686930ce19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:21:15 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 13:21:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:21:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 02 Jun 2020 21:25:52 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:25:52 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Jun 2020 21:25:53 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 02 Jun 2020 21:25:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Jun 2020 21:25:54 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Jun 2020 21:25:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:25:54 GMT
WORKDIR /var/www/html
# Tue, 02 Jun 2020 21:25:54 GMT
EXPOSE 80
# Tue, 02 Jun 2020 21:25:54 GMT
CMD ["apache2-foreground"]
# Tue, 02 Jun 2020 22:52:00 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 02 Jun 2020 22:54:55 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Jun 2020 22:54:55 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 02 Jun 2020 22:54:56 GMT
VOLUME [/var/www/html]
# Tue, 02 Jun 2020 22:54:56 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 05 Jun 2020 00:28:11 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Fri, 05 Jun 2020 00:32:14 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 05 Jun 2020 00:32:15 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Fri, 05 Jun 2020 00:32:15 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Fri, 05 Jun 2020 00:32:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 05 Jun 2020 00:32:16 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79fb2b388016d9ef524926aa6e5510ffe2d6643a57cd4e09b991ca90ee2072e`  
		Last Modified: Fri, 15 May 2020 15:09:00 GMT  
		Size: 12.5 MB (12454915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa6f0dd42392167b786a269124c84e7cb00bc7dfcde4ea31a4d63ed938eae5`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a337c36d9faf17171bac8095de0116c196c8d43d3c8ffd191a6cd3c76d8e`  
		Last Modified: Fri, 15 May 2020 15:09:17 GMT  
		Size: 14.1 MB (14059019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758d173f8f745211fb061d3c58c9d26a8a441d130446da9364251c10e2fa9c9d`  
		Last Modified: Tue, 02 Jun 2020 21:31:18 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5659a9ca738392ef1e942f5813b83f6e99cadad31f62ee25c169296183be8009`  
		Last Modified: Tue, 02 Jun 2020 21:31:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b52a3053f0b02134948ba44ad915a2482e133393d61714625c1d7eab5cdea48`  
		Last Modified: Tue, 02 Jun 2020 21:31:18 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960f9e7d09e8e1edd1dd758d87d304d7c44dd6517b8daf62d3e184e57ca287a2`  
		Last Modified: Tue, 02 Jun 2020 21:31:18 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c8debc85af9f915070dedbbbfac4a4e21710270425fd632e8e67d829af3ebb`  
		Last Modified: Tue, 02 Jun 2020 23:48:02 GMT  
		Size: 1.7 MB (1659012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75c28a419026b2eb9cb5e1c317c54506d5064e39594a15e97fec9feffa43485`  
		Last Modified: Tue, 02 Jun 2020 23:48:12 GMT  
		Size: 16.2 MB (16198826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525cf10ab0f0cd045077eab68b626bd781dac511739ad243a5624632f26525ec`  
		Last Modified: Tue, 02 Jun 2020 23:48:00 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1293df934b6fba2e072286045e6b72b9b62362250c10b9f0491bbc9a2ffb0088`  
		Last Modified: Tue, 02 Jun 2020 23:48:00 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9c70defabc70e67b52039b6427f1d301d00f634b9f421b3d5ff49ce34cc3a`  
		Last Modified: Fri, 05 Jun 2020 01:26:48 GMT  
		Size: 73.3 MB (73320448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecce0bc844c46a0cd9f7f1d51efbe04f087e13eecb466fa36414f072f3bde21`  
		Last Modified: Fri, 05 Jun 2020 01:26:21 GMT  
		Size: 2.6 KB (2552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de5a092748762895dc546d964735d6f308a34c061008272e316221a61da8e04`  
		Last Modified: Fri, 05 Jun 2020 01:26:21 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:d5a01d16ae59ea18ede8a697d03aff59cc1c5d6e90595e229e06e5857eafa3d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216875305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82dd06b62e123b539192e31dc91e0e63c76944c50320c579ad495675c29012ad`
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
# Tue, 09 Jun 2020 03:33:12 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 03:33:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 03:33:13 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 03:33:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 03:33:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:37:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 03:37:14 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:37:17 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 03:37:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 09 Jun 2020 03:37:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 03:37:21 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Jun 2020 03:37:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:37:23 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 03:37:23 GMT
EXPOSE 80
# Tue, 09 Jun 2020 03:37:24 GMT
CMD ["apache2-foreground"]
# Tue, 09 Jun 2020 15:37:18 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 09 Jun 2020 15:42:09 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 15:42:12 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 15:42:13 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 15:42:15 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 09 Jun 2020 15:42:16 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Tue, 09 Jun 2020 15:43:06 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 15:43:10 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Tue, 09 Jun 2020 15:43:12 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Tue, 09 Jun 2020 15:43:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 15:43:14 GMT
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
	-	`sha256:3f17c47c8624fb48feb2f3fc675ae0c82c076c29367fb3d60e4bf518bd7a8255`  
		Last Modified: Tue, 09 Jun 2020 04:45:45 GMT  
		Size: 12.5 MB (12453054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d411751e41476899bf732aa5098b5309319adec821b979736acc0f92c2b27373`  
		Last Modified: Tue, 09 Jun 2020 04:45:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a9f02efcd63a694b86364a86d20042f682abb997059842f860baff9bae6e5`  
		Last Modified: Tue, 09 Jun 2020 04:45:47 GMT  
		Size: 13.1 MB (13073880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d705debf973062cf1bbb7341c63a93e5fbd14a9c8320293773361fbd039cc531`  
		Last Modified: Tue, 09 Jun 2020 04:45:42 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da26ea3b5f63605383e30614910d91aa63b1a95960389977ef72b337a0d5797`  
		Last Modified: Tue, 09 Jun 2020 04:45:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b3967d8cc1a511c49739f26c201ff1e1dc2272e8a7bd0a55655dd833d532a0`  
		Last Modified: Tue, 09 Jun 2020 04:45:43 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94714750f7d1cb7a9010de50e271f0f15fbb944a1cb4befa5823dc9b5c065bc`  
		Last Modified: Tue, 09 Jun 2020 04:45:44 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8f07266abf0a5b281f1359f2ebdac7113a19e2285cad7ad5a6693c31538255`  
		Last Modified: Tue, 09 Jun 2020 16:07:57 GMT  
		Size: 1.6 MB (1596605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a6fea19b9c3357252ffac3fa8ba5b2aeb28461c13331098b775c083483875c`  
		Last Modified: Tue, 09 Jun 2020 16:08:01 GMT  
		Size: 14.8 MB (14761105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6683665956a4ade3252c7ab9389aaf14117e62381cc0c03af585389497524d6`  
		Last Modified: Tue, 09 Jun 2020 16:07:55 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69588d2a577648fa86d72ac295a4f85143612d6fdee147375998ddfe287f703f`  
		Last Modified: Tue, 09 Jun 2020 16:07:55 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb57139a4b60e5c0b8aa4262dab19a9fc4cf220986e79b4cdc451f8585443fa6`  
		Last Modified: Tue, 09 Jun 2020 16:08:22 GMT  
		Size: 73.3 MB (73317750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556a3f0d75e083c8906db2ef06297ed7758c0ca1fe39c58c49e5e165923f3148`  
		Last Modified: Tue, 09 Jun 2020 16:07:55 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6701fcc73b4e2324172916a6c09a805b2bfa4959af4a96421ea991c5eafef54`  
		Last Modified: Tue, 09 Jun 2020 16:07:56 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:dab9d2a7dcc05aa1366fa4ded8bf364bffbf9117612950c682ea520e0a8191c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213036270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fcba7199cd29597d5b1f34ec0c232a0845eaf7869cb2a1e390883d68212b77`
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
# Tue, 09 Jun 2020 09:59:54 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 09:59:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 09:59:55 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 10:00:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 10:00:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:03:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 10:03:32 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:03:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 10:03:39 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 09 Jun 2020 10:03:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 10:03:44 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Jun 2020 10:03:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:03:47 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 10:03:48 GMT
EXPOSE 80
# Tue, 09 Jun 2020 10:03:49 GMT
CMD ["apache2-foreground"]
# Wed, 10 Jun 2020 00:32:47 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 10 Jun 2020 00:38:30 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 00:38:35 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 10 Jun 2020 00:38:38 GMT
VOLUME [/var/www/html]
# Wed, 10 Jun 2020 00:38:45 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 10 Jun 2020 00:38:48 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Wed, 10 Jun 2020 00:39:43 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 00:39:47 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Wed, 10 Jun 2020 00:39:50 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Wed, 10 Jun 2020 00:39:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 00:39:52 GMT
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
	-	`sha256:5cb0f7788ffe6de7c7223fdde924ef01669afdbf8a6b2d3ea7ecf69865ad0b36`  
		Last Modified: Tue, 09 Jun 2020 11:13:44 GMT  
		Size: 12.5 MB (12453032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8510fbcea001655c0fd4649334e38da58f29dd0961fef9ce27404a5c447fe1b`  
		Last Modified: Tue, 09 Jun 2020 11:13:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8e7ac339fabf8e19de2101a8af9608a13262aa8b400ecb403857f046daaa6e`  
		Last Modified: Tue, 09 Jun 2020 11:13:45 GMT  
		Size: 12.4 MB (12370823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81626fbf9c1e9810f21b72da9d6b6588b1ee9437ca6292a8a2fb7bc21b1db8d9`  
		Last Modified: Tue, 09 Jun 2020 11:13:39 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13d94c70db679f23ef658d2350687176d98829d91cf3b53a1ef27951215e85b`  
		Last Modified: Tue, 09 Jun 2020 11:13:39 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f4f0b988aef4650318ac740c71a3f77f228bec093d5317b4aa1832d081207c`  
		Last Modified: Tue, 09 Jun 2020 11:13:39 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657b50556e497abf510aa9e66324762dfd7fc999863fd73d6082ba665b41bce`  
		Last Modified: Tue, 09 Jun 2020 11:13:40 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24baceeb222732b2581a16f6493b9d911a75e27822dbd766a66a908f97a0ed8`  
		Last Modified: Wed, 10 Jun 2020 01:06:00 GMT  
		Size: 1.4 MB (1448733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f02597bee1ec5cd10b25e4e3b7dc2d9d953565fdb91d0009fe143383c7a29d`  
		Last Modified: Wed, 10 Jun 2020 01:06:03 GMT  
		Size: 13.7 MB (13741287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003366a5ef7279ed384f10d2709abcfe75f374c7dfce222217a111b0202d30f3`  
		Last Modified: Wed, 10 Jun 2020 01:05:57 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06701b770d42844017335cdf502c451663745aecd51e3dbb79f06036e5b88c0b`  
		Last Modified: Wed, 10 Jun 2020 01:05:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd91c12bde8dbf398489a1e4473bbe2ba0eb6c46a3c6863fe6dd95b3aa6544d`  
		Last Modified: Wed, 10 Jun 2020 01:06:26 GMT  
		Size: 73.3 MB (73318141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e63d0bbcc64b98f320e24eea34734853825edaaaf179a991f176c7a05c81e7`  
		Last Modified: Wed, 10 Jun 2020 01:05:56 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2e3c03f9b2b034300184ce5c51ded04ba3f42060a42b704ab21f4f9b5d01c9`  
		Last Modified: Wed, 10 Jun 2020 01:05:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:5041ac41eaff564eeacc28d301c8c120fa8aae5c3bf5d7d38ddb3bdb63d5941f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230457261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd52d895262998abf4954e4df45faa12d7ca68a8d383d0f9d2b3637ff1bad219`
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
# Tue, 09 Jun 2020 10:48:29 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 10:48:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 10:48:30 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 10:48:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 10:48:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 10:52:16 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:52:18 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 10:52:20 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 09 Jun 2020 10:52:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 10:52:22 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Jun 2020 10:52:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:52:23 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 10:52:24 GMT
EXPOSE 80
# Tue, 09 Jun 2020 10:52:25 GMT
CMD ["apache2-foreground"]
# Wed, 10 Jun 2020 02:00:35 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 10 Jun 2020 02:06:47 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:06:50 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 10 Jun 2020 02:06:51 GMT
VOLUME [/var/www/html]
# Wed, 10 Jun 2020 02:06:53 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 10 Jun 2020 02:06:54 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Wed, 10 Jun 2020 02:07:38 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:07:44 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Wed, 10 Jun 2020 02:07:46 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Wed, 10 Jun 2020 02:07:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:07:48 GMT
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
	-	`sha256:6ec312407d595e34512f0c445ee806d35c4d542e35d3c576e16ef31e125656ed`  
		Last Modified: Tue, 09 Jun 2020 11:59:36 GMT  
		Size: 12.5 MB (12453676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5be53565236e7bc33c2a994970a28650697b7b1b56a49b188c0e6de82246c6`  
		Last Modified: Tue, 09 Jun 2020 11:59:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ad724c4df62d24ec779d357e802277b58d961f27fc0048c6edd196eab9f819`  
		Last Modified: Tue, 09 Jun 2020 11:59:39 GMT  
		Size: 13.7 MB (13744517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016c71adedf2197778a1fe19ac1c12cca9069a014e65b184802f1997b10fe61a`  
		Last Modified: Tue, 09 Jun 2020 11:59:34 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b73adc136768c3dec3d78f95b1582b1aca6a3f7ab4984f3889f36436e39855`  
		Last Modified: Tue, 09 Jun 2020 11:59:33 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41556e087abc7a285812a561f2334d0e09d8eb7dd0e8b37a731cd2870985487c`  
		Last Modified: Tue, 09 Jun 2020 11:59:33 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aecc78c23f55da3aeddbe8241d40688f58d700c58f3c86a12ae6b25c0d7b3a`  
		Last Modified: Tue, 09 Jun 2020 11:59:34 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983ade281dc3aa43a0579db287483cc28041283fe58e8c15c38a5b2011cfe520`  
		Last Modified: Wed, 10 Jun 2020 02:32:07 GMT  
		Size: 1.6 MB (1625462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d9b72de85b66c5d193d5859f5ff5863e8a6122eb8723db0436d7f95c65f978`  
		Last Modified: Wed, 10 Jun 2020 02:32:10 GMT  
		Size: 14.5 MB (14529089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e73ce5ece913e92b77a0f7c5e7a9dc9b0817199e47fc84311a95199920672a`  
		Last Modified: Wed, 10 Jun 2020 02:32:05 GMT  
		Size: 534.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c8d5f456022bbfc55d6e022fb377ad04fcfbbc5a0cec10979a7150efcbc851`  
		Last Modified: Wed, 10 Jun 2020 02:32:05 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f4368bf673be6f4eb8d55be9b75bb1f9fbfda9ea40781b1f970940c2ec83e6`  
		Last Modified: Wed, 10 Jun 2020 02:32:27 GMT  
		Size: 73.3 MB (73319381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6c812d02b50ee4fbc6188e84f5eae9aeb5f6cf2a002e62f6359ae371422e87`  
		Last Modified: Wed, 10 Jun 2020 02:32:05 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca03b4bd3f0dff2e6c7b25143b756cc60d0d22c15cdbbea27158fa924cdd22`  
		Last Modified: Wed, 10 Jun 2020 02:32:05 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; 386

```console
$ docker pull nextcloud@sha256:b16861b007df771fceda85ff6ad456e6313491bf2deceb8651d5e3a30e7dcf91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.4 MB (245435270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eca5964e10c7cead0d9d4edb7fa428df2b53a7d1b23f8617c9040a0d8c877cfd`
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
# Tue, 09 Jun 2020 08:01:09 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 08:01:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 08:01:09 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 08:01:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 08:01:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 08:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 08:05:23 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 09 Jun 2020 08:05:24 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 08:05:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 09 Jun 2020 08:05:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 08:05:26 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Jun 2020 08:05:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Jun 2020 08:05:27 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 08:05:27 GMT
EXPOSE 80
# Tue, 09 Jun 2020 08:05:27 GMT
CMD ["apache2-foreground"]
# Tue, 09 Jun 2020 21:03:19 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 09 Jun 2020 21:06:19 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:06:20 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 21:06:21 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 21:06:21 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 09 Jun 2020 21:06:22 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Tue, 09 Jun 2020 21:06:54 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:06:55 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Tue, 09 Jun 2020 21:06:56 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Tue, 09 Jun 2020 21:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 21:06:56 GMT
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
	-	`sha256:4eb95bb75658978c0dffa0fcb3fb5e9f4dd5efc2fdd04eb8cb5d1397d1f3a167`  
		Last Modified: Tue, 09 Jun 2020 10:02:07 GMT  
		Size: 12.5 MB (12454142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bfcc8ff6a924f8ebaa87ef7de0fea0ceea7ff53ac2aabc7784d2c85b8788ca`  
		Last Modified: Tue, 09 Jun 2020 10:02:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2521ea39ef8dfdf5687d9a78c8d5958fd6da108a841b1ed50bfa500f418d0`  
		Last Modified: Tue, 09 Jun 2020 10:02:11 GMT  
		Size: 14.4 MB (14375359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b2eb82b4212b89293ca4037e3572a10e23349fd3297ba6c8557f45e8d6fa29`  
		Last Modified: Tue, 09 Jun 2020 10:02:03 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e9f0bfb7d06979d85092f79d3e4bd0c4313d5840c6be03302ded8243d1f54a`  
		Last Modified: Tue, 09 Jun 2020 10:02:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9545db1fc0880d66a30f6e73815e9e55f6866cb5a3ecff62591cbff4e191f9ab`  
		Last Modified: Tue, 09 Jun 2020 10:02:02 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642ab643b5952ee3b12e9f36479ce607e79e78bd51d4c1a27450c4343257c3c2`  
		Last Modified: Tue, 09 Jun 2020 10:02:03 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7237fd997fc3c1d45bd075a87a39640cfab72c9ba0605e1e552c67054c602a`  
		Last Modified: Tue, 09 Jun 2020 21:24:09 GMT  
		Size: 1.7 MB (1682757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08319982e19573ab9a539605988eed93466622b1bc3b35b18db2deae8645b63`  
		Last Modified: Tue, 09 Jun 2020 21:24:19 GMT  
		Size: 15.5 MB (15530335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d0eb86f8db3ff26ca3627c5b8ed835a1976ba0fc70f571ee529b1eae904e35`  
		Last Modified: Tue, 09 Jun 2020 21:24:07 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107912b851167fbbc2869f37e52e66e4d289a10252e7bc3ce305e45d700c44`  
		Last Modified: Tue, 09 Jun 2020 21:24:06 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae09d509181852f4958fc05fe859f1da79b6494351b17bd4fe52078a0ec7a7d4`  
		Last Modified: Tue, 09 Jun 2020 21:24:51 GMT  
		Size: 73.3 MB (73319349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a792525897d625aa305e2b6c86417844a7ac41c71e84a981037f211265b7714`  
		Last Modified: Tue, 09 Jun 2020 21:24:06 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdd1fa0c5814836cfbafd7322f7337ccd96f01c6c4c7eb76713ebf4163346bc`  
		Last Modified: Tue, 09 Jun 2020 21:24:07 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; mips64le

```console
$ docker pull nextcloud@sha256:aed071dbdc24aab60a1b6c86f55ecfb80f80cfea40d48552108c69c612ee07ec
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221226670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc76459c47032453b8fc91c0b8b37aea250037a6e44f23e8970dccd6db0ea58c`
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
# Tue, 09 Jun 2020 04:47:39 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 04:47:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 04:47:40 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 04:48:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 04:48:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 04:58:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 04:58:14 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 09 Jun 2020 04:58:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 04:58:18 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 09 Jun 2020 04:58:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 04:58:19 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Jun 2020 04:58:19 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Jun 2020 04:58:20 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 04:58:20 GMT
EXPOSE 80
# Tue, 09 Jun 2020 04:58:20 GMT
CMD ["apache2-foreground"]
# Tue, 09 Jun 2020 22:14:59 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 09 Jun 2020 22:22:56 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:22:58 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 22:22:59 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 22:23:01 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 09 Jun 2020 22:23:01 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Tue, 09 Jun 2020 22:24:21 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:24:23 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Tue, 09 Jun 2020 22:24:25 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Tue, 09 Jun 2020 22:24:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 22:24:26 GMT
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
	-	`sha256:2fba759d832de2a7605183f7140281d66f9052b89c325a355a7c4fedb2053a8d`  
		Last Modified: Tue, 09 Jun 2020 06:38:52 GMT  
		Size: 12.5 MB (12452280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bfdbc12cf6e222390e9dfa6ae917148d305f82a9734d407345356f1135da6d`  
		Last Modified: Tue, 09 Jun 2020 06:38:47 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a858722fd821ca1a1f13d6e1a97903cdf798fedd7a08058492b163d91b97c`  
		Last Modified: Tue, 09 Jun 2020 06:38:58 GMT  
		Size: 13.3 MB (13335586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ede83212fbd3ccfd2bb022a55376e88ffd83bfac969144b909db37be2eb7f91`  
		Last Modified: Tue, 09 Jun 2020 06:38:44 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91fb40617536814bd5d89bd111bdd2a1f0913c8c6e8aea1fc5d6783906224a0`  
		Last Modified: Tue, 09 Jun 2020 06:38:44 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b15daebd6ecfe8660bf6da0e085c9fc06ce9f0f57884ea3709714b52fef178`  
		Last Modified: Tue, 09 Jun 2020 06:38:44 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37030a9bf3239197d7d4ced71b6f1323869e89ab068c112be22717702d7d5be5`  
		Last Modified: Tue, 09 Jun 2020 06:38:45 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431b66034c70e29a6e537d24b39e78a1557ae0d92eb4486eb8feb45346839c3`  
		Last Modified: Tue, 09 Jun 2020 22:52:07 GMT  
		Size: 1.8 MB (1763156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10519b0337745a0a2a921627149a18370f9662f5cceff16e62b916252573e000`  
		Last Modified: Tue, 09 Jun 2020 22:52:19 GMT  
		Size: 14.6 MB (14590058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82185c8e9daffd41af4883bc9a0f5d1841d4f01343a8eaa10ec6daec3b1b949`  
		Last Modified: Tue, 09 Jun 2020 22:51:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b21663ba935e13d898f90d7f685b814ae22dabe6c729b58134b39d12f347c`  
		Last Modified: Tue, 09 Jun 2020 22:51:59 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508a82e8efeec8a8c41242ab8c4ccad4adbd1823feac3064566c575358134bd8`  
		Last Modified: Tue, 09 Jun 2020 22:53:00 GMT  
		Size: 73.3 MB (73317811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd06b84fa6a55a381c2dce7293dd3efc12fea87708dc80f9df173bc2af882b3`  
		Last Modified: Tue, 09 Jun 2020 22:51:59 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b88c5982df4cf8671a1bb59e4e9af84f25b304dc2ead5c4a19c70ddaec7f2`  
		Last Modified: Tue, 09 Jun 2020 22:51:59 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:fa495e8a18d9ce13fc9b623e564e882a3510359060572c021d4698756fa5f11d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251702589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80cf6b4826e17444fa80b26ab9c752ca142c33c8da3faf11239526a5d092fde2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 09:03:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Mon, 18 May 2020 09:03:57 GMT
ENV PHP_VERSION=7.3.18
# Mon, 18 May 2020 09:04:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Mon, 18 May 2020 09:04:02 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Mon, 18 May 2020 09:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 09:04:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 02 Jun 2020 21:25:19 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:25:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Jun 2020 21:25:34 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 02 Jun 2020 21:25:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Jun 2020 21:25:37 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Jun 2020 21:25:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:25:40 GMT
WORKDIR /var/www/html
# Tue, 02 Jun 2020 21:25:43 GMT
EXPOSE 80
# Tue, 02 Jun 2020 21:25:44 GMT
CMD ["apache2-foreground"]
# Wed, 03 Jun 2020 00:41:37 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 03 Jun 2020 00:57:18 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 03 Jun 2020 00:57:29 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 03 Jun 2020 00:57:32 GMT
VOLUME [/var/www/html]
# Wed, 03 Jun 2020 00:57:45 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 05 Jun 2020 00:27:39 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Fri, 05 Jun 2020 00:29:59 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 05 Jun 2020 00:30:02 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Fri, 05 Jun 2020 00:30:05 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Fri, 05 Jun 2020 00:30:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 05 Jun 2020 00:30:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5778da4b9e5d7a88f35ba1be2447f4f549ba69a64e3d51f25a3d12ffcd3cb2`  
		Last Modified: Mon, 18 May 2020 12:18:41 GMT  
		Size: 12.5 MB (12455153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71128df22a3960c05cabb8404ffb23bc6a97a69eceecf88249d546ec4b569`  
		Last Modified: Mon, 18 May 2020 12:18:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe189a8a7aa4a630396336b029b1c309e64143334b9269b1fde2ea84d02a64a7`  
		Last Modified: Mon, 18 May 2020 12:18:44 GMT  
		Size: 15.1 MB (15099913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca91aecf90e74c5991531d2ecfb18b31d27f658f1882d727fd0c3ec00aa86ab`  
		Last Modified: Tue, 02 Jun 2020 21:42:40 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6e24ee1f70cf6159041fdbe2639645efea773ffb7635cdb1fccb90600d5b95`  
		Last Modified: Tue, 02 Jun 2020 21:42:40 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac04f5a9808c29e02e8d66f3a12f4dfcfc0fcc58a40cccad0d55f6e525319d7`  
		Last Modified: Tue, 02 Jun 2020 21:42:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20dbbabb11525149e6494dd751d010be9f1a170901089515bfad115814d1f3a`  
		Last Modified: Tue, 02 Jun 2020 21:42:40 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb9c327f17ff04887cf5df4ad5c22f45815a0b0a17245e7c62f22c8afceca84`  
		Last Modified: Wed, 03 Jun 2020 02:27:55 GMT  
		Size: 1.8 MB (1826721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7057c2149d27abef0fd404b326c1e246148a7a20f311c25cc39db5e581995ebf`  
		Last Modified: Wed, 03 Jun 2020 02:28:21 GMT  
		Size: 16.4 MB (16389499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39978a3e3e4d2f51a38324b27af3d5ef928c86287f848363defc6683484a2603`  
		Last Modified: Wed, 03 Jun 2020 02:27:49 GMT  
		Size: 536.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2a918f09f8ecb0fb9dbf847d37f4305139dfe91d92bfc9d0630a44c87c948b`  
		Last Modified: Wed, 03 Jun 2020 02:27:49 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecd67e99ee79334f1e932c881d9dc0411a0c9801f648498e478bdada7f17b69`  
		Last Modified: Fri, 05 Jun 2020 01:37:30 GMT  
		Size: 73.3 MB (73322469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae14ed4db279669f293dbf5e2f5510a2619a34c5369c87fb7ce4957df18f2f4`  
		Last Modified: Fri, 05 Jun 2020 01:35:42 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e37198e33a75a312f041e8c1109fef64990134cc827851c045e6be04f682f5`  
		Last Modified: Fri, 05 Jun 2020 01:35:42 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:17-apache` - linux; s390x

```console
$ docker pull nextcloud@sha256:7754831cc2c70fe0578d7ea1ca19cb6cd00aed41eff8b255b54f9b1b1c429aef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224300302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:291f9c93e2e4f0cd2936b903e81885b90b705e6fe0843a2946bb4cf5c0092d9c`
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
# Tue, 09 Jun 2020 06:49:37 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 06:49:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 06:49:38 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 06:49:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 06:49:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 06:51:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 06:51:12 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 09 Jun 2020 06:51:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 06:51:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 09 Jun 2020 06:51:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 06:51:14 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Jun 2020 06:51:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Jun 2020 06:51:14 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 06:51:14 GMT
EXPOSE 80
# Tue, 09 Jun 2020 06:51:14 GMT
CMD ["apache2-foreground"]
# Tue, 09 Jun 2020 16:45:42 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 09 Jun 2020 16:47:32 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure gmp --with-gmp="/usr/include/$debMultiarch";     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:47:33 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 16:47:33 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 16:47:34 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 09 Jun 2020 16:47:34 GMT
ENV NEXTCLOUD_VERSION=17.0.7
# Tue, 09 Jun 2020 16:47:57 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:48:02 GMT
COPY multi:57de70033920dd582f0dbb812d28f0cfdcf6a102d5b4374faf9435d87a0a7585 in / 
# Tue, 09 Jun 2020 16:48:02 GMT
COPY multi:641d9647b02e0716fa98d67c2bd719ff1b296a8a83ca009f972756c58c2e5fed in /usr/src/nextcloud/config/ 
# Tue, 09 Jun 2020 16:48:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 16:48:03 GMT
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
	-	`sha256:c43cbd1d21c4edf5cff0b21707556cea308c8ad1d45bd82b695efee5f6db50f5`  
		Last Modified: Tue, 09 Jun 2020 08:12:23 GMT  
		Size: 12.5 MB (12453300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ceb91c25c833302ec52ad6b756091aa61c93dcfdfb764014fd33ccd200f1e85`  
		Last Modified: Tue, 09 Jun 2020 08:12:31 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02860f354b76207fd240f853c8d8541eda1e3049074c53a2628ade33a4f7141a`  
		Last Modified: Tue, 09 Jun 2020 08:12:01 GMT  
		Size: 13.3 MB (13291107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e1884c886b9e1676d33e364ec5c2478906ccc75586c4161fe284c15f3b7d5f`  
		Last Modified: Tue, 09 Jun 2020 08:12:01 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f51ea778cc6b975de48bc6185765c9ed1f73d9b56e2601a3b88a450618aa12`  
		Last Modified: Tue, 09 Jun 2020 08:12:14 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ff22741266f1dcab05bf3e29a26b50f1862c48859219d7be4a533af415fc85`  
		Last Modified: Tue, 09 Jun 2020 08:12:14 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4483517ef306b4c9b6fcdfa3342738b705196f1d172ecc6533c30ea92e9cb8a`  
		Last Modified: Tue, 09 Jun 2020 08:12:14 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54ef75ce49998c8eb5dd6df3011590b64c995fa40bed5f41c921b7e7a4e24a0`  
		Last Modified: Tue, 09 Jun 2020 16:58:14 GMT  
		Size: 1.6 MB (1618034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0c11784c0e65200973a6c1257e00a212ea15c5ae63b2f1a20b3b73ff8aee2`  
		Last Modified: Tue, 09 Jun 2020 16:58:15 GMT  
		Size: 14.7 MB (14676154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b2f25edeb705a6c6a98fe6e2d59f624ea613a41b44becb1844efbcdeec434`  
		Last Modified: Tue, 09 Jun 2020 16:58:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db3328b8e9d2456eb2bf3afafd41c10b466e9bf75c96725bc06a3d402ad548`  
		Last Modified: Tue, 09 Jun 2020 16:58:12 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103cd02b20e3734db466d1235441c5bcef5b6266552a60cde087cd4c3c1d3bc4`  
		Last Modified: Tue, 09 Jun 2020 16:58:24 GMT  
		Size: 73.3 MB (73317707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0ad459289b793863f3b5d63565b5b8b9dd0ba5869dffcab4e78aa5361d56a4`  
		Last Modified: Tue, 09 Jun 2020 16:58:27 GMT  
		Size: 2.6 KB (2553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8fd81d95c3a8fb44987a7f5f0cea6a4fba2a08eb0cadfb090e2c391a3f7bc3`  
		Last Modified: Tue, 09 Jun 2020 16:58:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
