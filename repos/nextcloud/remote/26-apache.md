## `nextcloud:26-apache`

```console
$ docker pull nextcloud@sha256:8b2384472cf42930c42f967eeb94c16e646692645268c60f2c29158ac5dbc1a1
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

### `nextcloud:26-apache` - linux; amd64

```console
$ docker pull nextcloud@sha256:6776b25861ddd03fcf87df1b33e7c49a095e639e14daa1bd29d423dbb64e9f00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.7 MB (395717363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97862e6d561748026fdb9002a700f680c22a4e2022224f7bded25d95503534d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:16:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 17:16:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 17:17:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:17:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 17:17:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 17:21:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 17:21:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 17:21:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 17:21:26 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 17:21:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 17:21:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:21:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:21:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 17:50:27 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 18:18:52 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 18:18:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 18:18:52 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 18:19:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 18:19:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:22:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 18:22:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:22:36 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 18:22:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 18:22:36 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 18:22:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:22:36 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:22:36 GMT
EXPOSE 80
# Wed, 20 Sep 2023 18:22:36 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 08:20:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Sep 2023 08:20:53 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 08:20:53 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 21 Sep 2023 08:23:42 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:23:43 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Sep 2023 08:23:43 GMT
VOLUME [/var/www/html]
# Thu, 21 Sep 2023 08:23:44 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 21 Sep 2023 08:23:44 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Thu, 21 Sep 2023 08:23:44 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Thu, 21 Sep 2023 08:23:44 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Thu, 21 Sep 2023 08:24:39 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:24:41 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Thu, 21 Sep 2023 08:24:41 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Thu, 21 Sep 2023 08:24:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Sep 2023 08:24:41 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84313b8f4350b0dd95a86cc174a0c24fedfb44a7f0970c63186d62b66eb99573`  
		Last Modified: Wed, 20 Sep 2023 20:09:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f42c54df3ff13333050b83b696d6d81c360bc33d0e5bbe2360443aeee97e6e`  
		Last Modified: Wed, 20 Sep 2023 20:09:58 GMT  
		Size: 104.3 MB (104341094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac86b32c02852d5dca280605cfc570d1303cdd5f6e2dabf88e6e87a6e073ad9`  
		Last Modified: Wed, 20 Sep 2023 20:09:43 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e326747c51cbc0fd569b13ffd264d41b236a9154ee1164ea27b0494f7ff923da`  
		Last Modified: Wed, 20 Sep 2023 20:10:25 GMT  
		Size: 20.3 MB (20303148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2241eb3f28be0625dc3bebb339b90d7b2a571247700faa69e2c6821874d6b9e6`  
		Last Modified: Wed, 20 Sep 2023 20:10:23 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dc7266c2a73b605aa539b6d6e05bf1a79e2fb53b7960a307e05749b474efcf`  
		Last Modified: Wed, 20 Sep 2023 20:10:22 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec18efeb39cb678f366ad5aed32b3632e9ca5a7859344400dedf5ade93d81dd`  
		Last Modified: Wed, 20 Sep 2023 20:15:49 GMT  
		Size: 12.4 MB (12373914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9735ceb0061b1514e0ca99248a2916c0fa1c4b3114cb0167fb7df7925b273a67`  
		Last Modified: Wed, 20 Sep 2023 20:15:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee784b440ec19eb8c98fe54540b003d0d0b256b8ca9a40bc90bdacbb1c9a4ca7`  
		Last Modified: Wed, 20 Sep 2023 20:15:48 GMT  
		Size: 11.4 MB (11423145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d23dd4e6e3d65a993f6c8889b132a7188086b7cf139aca8f11361d6e920c3f7`  
		Last Modified: Wed, 20 Sep 2023 20:15:46 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c76f3c377f63c00a9bb85b53fd41e75903a01eb3b040e822e539f46e9252be`  
		Last Modified: Wed, 20 Sep 2023 20:15:45 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c9c239ae747ef9caa49aa18a7dfc73225d6d7631a024590b84e2f51dbd6928`  
		Last Modified: Wed, 20 Sep 2023 20:15:45 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e8e4273ca060433f53bf7365cecf1b87cf3247059c23a5b32105764b874925`  
		Last Modified: Thu, 21 Sep 2023 08:33:09 GMT  
		Size: 22.8 MB (22758280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1736eedf4d9af08eb85bb383870fb5797ec34fc30ac1968507f6cf75513da7`  
		Last Modified: Thu, 21 Sep 2023 08:33:06 GMT  
		Size: 20.9 MB (20892637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9886232e080c52b5f660af775bc1a4eb0c8ec8307660293405bc6b270751a620`  
		Last Modified: Thu, 21 Sep 2023 08:33:02 GMT  
		Size: 762.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9733e7fef4150873f5967b86135d15c2bcf79d69761b512356e5b701e24d25`  
		Last Modified: Thu, 21 Sep 2023 08:33:01 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55909961d61983eab6ddd1ec5ee60f9870f776ee617c2383733d569705096734`  
		Last Modified: Thu, 21 Sep 2023 08:33:01 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed2cbe6e7b64a07630d638b9af0773f99a7a06f1b652d86ef5be992ff1c4fb`  
		Last Modified: Thu, 21 Sep 2023 08:33:21 GMT  
		Size: 174.5 MB (174487249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda77a0e2e2e85689d238cfa8535e2c4e0f28e5b8219cde5bc61e6f77efead93`  
		Last Modified: Thu, 21 Sep 2023 08:33:01 GMT  
		Size: 3.6 KB (3609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f33578951148ee42cb9d2d63d9166e2106c284290901b736eab734bd52a4a2`  
		Last Modified: Thu, 21 Sep 2023 08:33:01 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:0da4091ae1431c929f1f2c32f669111efc8f2346a2d3ad83bef7607a8b1976d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.4 MB (365369228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:723924b56e251b06626f3c03ed7a8cb21a9128a1bb60df40751a631aef4bdd03`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:54 GMT
ADD file:a4ac238e8d5bf843acb96f72c03d55e0a7f2fca33ba16d7631d397176acf8c3a in / 
# Wed, 20 Sep 2023 00:49:54 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 06:49:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 06:49:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 06:49:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 06:49:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 06:49:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 06:54:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 06:54:32 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 06:54:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 06:54:48 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 06:54:49 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 06:54:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:54:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:54:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 07:26:06 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 07:51:25 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 07:51:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 07:51:26 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 07:51:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 07:51:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:55:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 07:55:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:55:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 07:55:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 07:55:27 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 07:55:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:55:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:55:28 GMT
EXPOSE 80
# Wed, 20 Sep 2023 07:55:28 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 18:50:19 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 20 Sep 2023 18:50:20 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 20 Sep 2023 18:50:20 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 20 Sep 2023 18:53:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:53:05 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 20 Sep 2023 18:53:05 GMT
VOLUME [/var/www/html]
# Wed, 20 Sep 2023 18:53:05 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Wed, 20 Sep 2023 18:53:05 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Wed, 20 Sep 2023 18:53:06 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Wed, 20 Sep 2023 18:53:06 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Wed, 20 Sep 2023 18:54:15 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:54:17 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Wed, 20 Sep 2023 18:54:18 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Wed, 20 Sep 2023 18:54:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 18:54:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9de40a7a125e0755ac5cf1e38c2f8a6b3d3c005cfc82323d13f5dceb50381fd7`  
		Last Modified: Wed, 20 Sep 2023 00:54:44 GMT  
		Size: 27.0 MB (26983563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f24cb8696eeb6eb097682650dc67adcf7c35905bcf37e668650c20e7322075b`  
		Last Modified: Wed, 20 Sep 2023 09:21:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f6cfcf70e306a80663819c82c26659b880614c9310da0ac03a6ab26699694b`  
		Last Modified: Wed, 20 Sep 2023 09:22:09 GMT  
		Size: 82.0 MB (82027509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4fc4ddf4c72854063d350e3564b3f32838c43793938eac953ea2b4399b19d8`  
		Last Modified: Wed, 20 Sep 2023 09:21:52 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67fea38d7ceccf8b29a64c351f8b735297a622aed3c9c4b2eddf7815e382d0`  
		Last Modified: Wed, 20 Sep 2023 09:22:36 GMT  
		Size: 19.6 MB (19607878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680be152ab56b5e81049dccf267a1bfdb2cf8d51a5dbe3db8034ae6f7f589a6`  
		Last Modified: Wed, 20 Sep 2023 09:22:32 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17297332032d69653a5325caffb8a0f60878d2dcf486f834b1890d6ecbd9d91f`  
		Last Modified: Wed, 20 Sep 2023 09:22:32 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4396339bbd868366c7ffac829872ef0cb93c2dd3fd439ebbb62b6917304fa119`  
		Last Modified: Wed, 20 Sep 2023 09:27:49 GMT  
		Size: 12.4 MB (12372223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940703492aca92a966795eb1c28c5d377fbe9ca11333e85d4eea3c0f8331e74d`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9b8cb2fbfc2953e9c1796b51dbe88a592ed57837416fd5a68633d8cd1c1afb`  
		Last Modified: Wed, 20 Sep 2023 09:27:49 GMT  
		Size: 10.4 MB (10407272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881010130762a246413e027f20541b1e319f81cc9d3f95f5b0f77172b70cd5d2`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244a3c7256a505b6b6b22c2778ac93b7c3831ec120e550d1d3700731f867a09e`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747443a796021013880137a88fef34ef026f760e927c8aaad5e81cb39da3c8ec`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85acb567b2f024cb1870aefea20ea5f325a303e7c54252de17b61b20283756b`  
		Last Modified: Wed, 20 Sep 2023 19:04:15 GMT  
		Size: 19.9 MB (19876635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02654405ee6b47e66ea8f6e2c7813a0ceb1bdf5260e30139e603df4367f9404`  
		Last Modified: Wed, 20 Sep 2023 19:04:15 GMT  
		Size: 19.6 MB (19596120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd3079eab3c6e7240807661b42995d0b8926db0b3d8b348abefaa5881ca7867`  
		Last Modified: Wed, 20 Sep 2023 19:04:11 GMT  
		Size: 760.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa3b97ff611682f528ace3fae13cdee2c7036bd34c73032846b966e735e39a9`  
		Last Modified: Wed, 20 Sep 2023 19:04:09 GMT  
		Size: 571.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c85e2412b95578062b1bd65dccf435e7481882a2883a951fe2928909194938f`  
		Last Modified: Wed, 20 Sep 2023 19:04:09 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2e7218e0aa737cf293f6b38e054e40f0c18e3db33dea42ae4e2c37857f1ed4`  
		Last Modified: Wed, 20 Sep 2023 19:04:59 GMT  
		Size: 174.5 MB (174484847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6cf210b884d08742d472bec8edd48f4ce05bf5378cea67033628da16ac8ca0`  
		Last Modified: Wed, 20 Sep 2023 19:04:09 GMT  
		Size: 3.6 KB (3609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c0993e4e96f5e6b3e431bab8b1176349af1f67c2bdd33995a652e415e3b654`  
		Last Modified: Wed, 20 Sep 2023 19:04:09 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:6b4d4337d857c7a0a649749e904ec08fc9f126127ca67e2c4c6cefe6c59fd3ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.8 MB (353821015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b80059ce33bc055eac5e2ce83a900dab3abf4658948d89b5625f024e34748a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:56b69c762bd03a9b00a1677740f7209aac08bac69a9e73563e326b9b0efbbfcc in / 
# Wed, 20 Sep 2023 04:57:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:23:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 05:23:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 05:23:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:23:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 05:23:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 05:26:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 05:26:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 05:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 05:26:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 05:26:34 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 05:26:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:26:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:26:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:51:06 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 06:14:48 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 06:14:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 06:14:48 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 06:15:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 06:15:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:17:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 06:17:47 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:17:48 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 06:17:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 06:17:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 06:17:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:17:49 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:17:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 06:17:49 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 08:34:24 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Sep 2023 08:34:24 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 08:34:25 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 21 Sep 2023 08:36:54 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:36:55 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Sep 2023 08:36:55 GMT
VOLUME [/var/www/html]
# Thu, 21 Sep 2023 08:36:56 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 21 Sep 2023 08:36:56 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Thu, 21 Sep 2023 08:36:56 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Thu, 21 Sep 2023 08:36:57 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Thu, 21 Sep 2023 08:38:00 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:38:03 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Thu, 21 Sep 2023 08:38:04 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Thu, 21 Sep 2023 08:38:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Sep 2023 08:38:04 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e0b5206657a67707f4c57136f811162ce89a951fec109a406df7508d59e644cb`  
		Last Modified: Wed, 20 Sep 2023 05:01:16 GMT  
		Size: 24.8 MB (24805628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77c36c63b5620fa1aee28d72b0bf419e4846734ae0ae1b97e499b80227bcccf`  
		Last Modified: Wed, 20 Sep 2023 08:27:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c374a9ddf5ec36045bb90868e1cd2f4c6f97c6b247ec377181e7ad2b2585610`  
		Last Modified: Wed, 20 Sep 2023 08:27:34 GMT  
		Size: 76.2 MB (76217199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96338ea9dbea14d4242de4aff36c62bb61d1d3f0398cf010e726aab82fcf027`  
		Last Modified: Wed, 20 Sep 2023 08:27:18 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d844f4e45f1ec163a8f9434fcf766294ccaa7ea0757e0301bac00778170e01f`  
		Last Modified: Wed, 20 Sep 2023 08:28:02 GMT  
		Size: 19.0 MB (19044685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c7ee66b5423964408cd3bf8365ceda864d08b150bd6d75ecaaa893fc2c5142`  
		Last Modified: Wed, 20 Sep 2023 08:27:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb184499580bd6c5083f272b27d48c06a2bd65390769f5e81b3ce3607dfb804`  
		Last Modified: Wed, 20 Sep 2023 08:27:59 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be9ece81c9ef7cba15dee11fea08fccd9cfbffa1c33e890b0b4cb4bf6ac595`  
		Last Modified: Wed, 20 Sep 2023 08:33:36 GMT  
		Size: 12.4 MB (12372201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47da1fad3fda85c9211a03ccbb977f834006bd468088b2198ee369549385658c`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a7992d3036a41b7bc53eabbed5f94e2dff11480f39ed2f4b7a57c4236ea9f9`  
		Last Modified: Wed, 20 Sep 2023 08:33:35 GMT  
		Size: 9.8 MB (9840138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9f76deec1b31e59d7328c29cb57dc0df063f60a1142d5e463736aa34ef056`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956c2196eb7b34a39a3e5316c32304910c8b6df2363bded0130bbaf4903da3ae`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03192b884044ebefdb064b04a1b9080eaaa1f50a0028cfac8dc373d25fe4a34a`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633db77850aa3ed067b5b78abcfcb289379a2e4af5e90a9f04d5ed2a14c928c1`  
		Last Modified: Thu, 21 Sep 2023 08:46:57 GMT  
		Size: 18.1 MB (18130134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2db19d7dca6698a0bdee4f47716913c1efa82aba74a5070150c6d517efcc464`  
		Last Modified: Thu, 21 Sep 2023 08:46:58 GMT  
		Size: 18.9 MB (18913041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04403bf27b7127a619df82d9ee2a88666f1387d5838fe7f408aa00067fd08cd`  
		Last Modified: Thu, 21 Sep 2023 08:46:55 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ee38551942025d6195bfedbd957ebbadf900f515f54377b7debdcbf72e556`  
		Last Modified: Thu, 21 Sep 2023 08:46:53 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73259691fee1adda679b6064acea5509ae3b8968afc7de633d6f8c648fc8a59b`  
		Last Modified: Thu, 21 Sep 2023 08:46:53 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71641d9e2b7f6969937bc1326046ffb84c5a7b8145545b15848823ebc631bf0`  
		Last Modified: Thu, 21 Sep 2023 08:47:19 GMT  
		Size: 174.5 MB (174484776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600943883d5ac14f4bc36b9e750ecf37d809b95cc0a7977851c3426a4fd95f1d`  
		Last Modified: Thu, 21 Sep 2023 08:46:53 GMT  
		Size: 3.6 KB (3605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8541f33f927f10b39718478028facf1f64a568571db316e32c2a66ce0b95c`  
		Last Modified: Thu, 21 Sep 2023 08:46:53 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:09f6d9c8eeaff1b6e05fbb51d2f78f8f0dabc58c79c06255c8e678e71e49889d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.1 MB (387141132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0307c8f57ceb09462221e329be8ed1a5f28c32eceba8af10004fb53f9956d2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:52:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 02:52:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 02:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 02:53:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 02:53:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 02:57:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 02:57:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 02:57:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 02:57:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 02:57:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 02:57:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 02:57:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 02:57:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:24:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 03:49:56 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 03:49:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 03:49:56 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 03:50:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 03:50:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:53:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 03:53:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:53:19 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 03:53:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 03:53:19 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 03:53:19 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:53:19 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 03:53:19 GMT
EXPOSE 80
# Wed, 20 Sep 2023 03:53:19 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 19:49:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 20 Sep 2023 19:49:29 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 20 Sep 2023 19:49:29 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 20 Sep 2023 19:52:22 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 19:52:23 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 20 Sep 2023 19:52:23 GMT
VOLUME [/var/www/html]
# Wed, 20 Sep 2023 19:52:23 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Wed, 20 Sep 2023 19:52:23 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Wed, 20 Sep 2023 19:52:24 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Wed, 20 Sep 2023 19:52:24 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Wed, 20 Sep 2023 19:53:17 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 19:53:21 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Wed, 20 Sep 2023 19:53:21 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Wed, 20 Sep 2023 19:53:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 19:53:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b1c5363061d299f9340dcbc40e3a72f489e7d4bc4f11a42044267bc480634`  
		Last Modified: Wed, 20 Sep 2023 05:59:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7adc7b3830328e51b6e68419760d8036c87394c9a09fead73478f67f58bb`  
		Last Modified: Wed, 20 Sep 2023 05:59:42 GMT  
		Size: 98.1 MB (98111498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7e7400ce12c1eeba03b34d6a220b7fc38cc011c52134d3ae19cd0e78dc2bd8`  
		Last Modified: Wed, 20 Sep 2023 05:59:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59572f84f3fa9dcf6ef27894127f256922909b98960561e2dedb8b1d7816fe0f`  
		Last Modified: Wed, 20 Sep 2023 06:00:20 GMT  
		Size: 20.3 MB (20304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bc70b64a40a408c9f63882bffe6b850efbbe5f4421c4e4345e5c4b6034434a`  
		Last Modified: Wed, 20 Sep 2023 06:00:17 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f189cf2b806d7ec6e02590c55abf84a6fd6293eb915144796d46edf3fddb2ac6`  
		Last Modified: Wed, 20 Sep 2023 06:00:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8a23963c39912e96c5d8ddb440822c3234c4a87b845f8bc1458bcd07139f6`  
		Last Modified: Wed, 20 Sep 2023 06:05:27 GMT  
		Size: 12.4 MB (12373654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54c9566a317067c0db574ea1c84c5a5a4f948bd0413ca82c47a3ce96fcbabd`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2d13cd3656443c5f2ac7097f5984ee0cd60a76d1d340dc056529ec2c3524dd`  
		Last Modified: Wed, 20 Sep 2023 06:05:27 GMT  
		Size: 11.4 MB (11431517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23974c86c4f8de94ca03677c3cb37ca70d3a4f7292d4fb4171636fadce4c9f2b`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28b1ab0221416706a6067f7fe6e71058ca3c8472ae74168ce076885d2da7bb`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234d29d31d1f72ae93d443f4e2448bfe53c791897c0604da77f2649a35f43898`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ba7c295b41fd930c04cfd4ce85647886b58d42a0fdba2948734c304dff02ce`  
		Last Modified: Wed, 20 Sep 2023 20:01:44 GMT  
		Size: 20.1 MB (20140619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d9f732192d73520ffe0b6c19bb0e7aad64fc8908ad418eed1e196ac22a101c`  
		Last Modified: Wed, 20 Sep 2023 20:01:44 GMT  
		Size: 21.1 MB (21122231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4456e60bfd1fe4bc53e3b6c93f6ed87a0cc7b676a5a8967b1789c2dc066d9`  
		Last Modified: Wed, 20 Sep 2023 20:01:41 GMT  
		Size: 762.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e8daaca3a834f4b2a3137b5d296223c3315e8f5c9d1c453705813c0069ecdb`  
		Last Modified: Wed, 20 Sep 2023 20:01:39 GMT  
		Size: 569.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8fdabd64b93b3635b9f3f7aebd5b15458cc607643509bcb4abe2522bf09399`  
		Last Modified: Wed, 20 Sep 2023 20:01:39 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c363120d3c01aa78661de62373bff16b076aa643330cb3aa2b0dd8c8ee9bd893`  
		Last Modified: Wed, 20 Sep 2023 20:01:56 GMT  
		Size: 174.5 MB (174486711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73b9a6a1b7b9b1196d9eb93316e86c336651dbc5ce5a13a5f176830fe39fa92`  
		Last Modified: Wed, 20 Sep 2023 20:01:39 GMT  
		Size: 3.6 KB (3609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862453988e39bab1ede96793eb7ac55a2bb3150620f73b8f3ff37c894182404`  
		Last Modified: Wed, 20 Sep 2023 20:01:39 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; 386

```console
$ docker pull nextcloud@sha256:013529b5621ef432297b89be7af3bacbe3122da87ff1a76a3cab5c836073b44d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.4 MB (394350484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a499b93b513b8d7a08b9844218589a8dd384162d49346d54c9421fb735bc9db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:41:55 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Wed, 20 Sep 2023 00:41:56 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:53:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 00:53:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 00:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 00:54:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 00:54:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 01:01:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 01:01:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 01:01:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 01:01:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 01:01:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 01:01:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:01:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:01:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 01:52:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 02:42:40 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 02:42:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 02:42:41 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 02:42:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 02:42:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 02:49:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 02:49:17 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 02:49:18 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 02:49:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 02:49:18 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 02:49:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 02:49:19 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 02:49:19 GMT
EXPOSE 80
# Wed, 20 Sep 2023 02:49:19 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 04:36:54 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Sep 2023 04:36:55 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 04:36:55 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 21 Sep 2023 04:40:34 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:40:35 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Sep 2023 04:40:35 GMT
VOLUME [/var/www/html]
# Thu, 21 Sep 2023 04:40:35 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 21 Sep 2023 04:40:35 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Thu, 21 Sep 2023 04:40:36 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Thu, 21 Sep 2023 04:40:36 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Thu, 21 Sep 2023 04:41:42 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:41:46 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Thu, 21 Sep 2023 04:41:46 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Thu, 21 Sep 2023 04:41:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Sep 2023 04:41:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12397f38a26a57209b69b50c272eef21ff3231f698f4d786af3ea55a456de888`  
		Last Modified: Wed, 20 Sep 2023 06:55:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2e20219e6d868557ed66105c7a57bff30ea650ac66dfe8ecc166cbbd8ff815`  
		Last Modified: Wed, 20 Sep 2023 06:55:46 GMT  
		Size: 101.5 MB (101506121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2aad3b4d2af1ab1af74242f2eb116ab6936b6ef54a895f6cb63840802150b9`  
		Last Modified: Wed, 20 Sep 2023 06:55:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297fb8f4dafa3b1aa10125bb95221e72827260df829cb4d6e4f4015980d10c0`  
		Last Modified: Wed, 20 Sep 2023 06:56:17 GMT  
		Size: 20.8 MB (20825359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de889c0746c4310f9955760a3dd696479ad3a8c259fbd2d2aa418935ddcd091`  
		Last Modified: Wed, 20 Sep 2023 06:56:12 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e725db08548938eafc4f03671e385e2562ed5d5b3e8a4ebf2a3611518274195a`  
		Last Modified: Wed, 20 Sep 2023 06:56:12 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304bb6c1681af1a6049412050ed05c58e3522761774d5b583e1e5d94448313f9`  
		Last Modified: Wed, 20 Sep 2023 07:02:39 GMT  
		Size: 12.4 MB (12373151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef7edc6d67e458c1b099cbe95d99ad9fcf7ec04a0a187cc16123784bd023b15`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd80d8f1422625e8486912aa1f8ffe8408ecd75d944d066e85644f84bc1893`  
		Last Modified: Wed, 20 Sep 2023 07:02:40 GMT  
		Size: 11.7 MB (11656472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374045e460123f61ce03c6846462adc26768cbdd3a124d28d8778f8a02f565d2`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51af293379289ffeb897d424954c17fd29464c6408fd62b2e64e4d19f8097302`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d7dfe84e18e2cbd4c87e0f2e8e75710b21329b0e176817c5047f208317278f`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40537a9d495ca8b6c6178082559ea74b112c1abfe3b4c22db52fc17fd293376e`  
		Last Modified: Thu, 21 Sep 2023 04:52:26 GMT  
		Size: 22.2 MB (22249595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6b5483aceb2452cf978110b0f461eb4b17b272394b32801c128544ece3f11f`  
		Last Modified: Thu, 21 Sep 2023 04:52:26 GMT  
		Size: 21.1 MB (21098603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14655c9929df5e8f4f893a6ba37b984fdd0e7ac9b165bcb21c42a676cc5261b8`  
		Last Modified: Thu, 21 Sep 2023 04:52:19 GMT  
		Size: 759.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe4f1101dfc019e5bb6980737cc23f699b3aee05c18687e68ecd161460d0aea`  
		Last Modified: Thu, 21 Sep 2023 04:52:18 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40fa1ae7b18ea3eec491e6e3dd97327989de92aed1050b503359a5091631b2c`  
		Last Modified: Thu, 21 Sep 2023 04:52:17 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba78dc2299709b530fe89a18c4eeb733f19f2073a18e155c6fa73e2343caef06`  
		Last Modified: Thu, 21 Sep 2023 04:52:52 GMT  
		Size: 174.5 MB (174486090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9c95fc5601db79e857ce00f874d907257060f6b3099f62349f2287db57b5e9`  
		Last Modified: Thu, 21 Sep 2023 04:52:17 GMT  
		Size: 3.6 KB (3609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55bede698a4c0f7b43419ad4c3fa119b21dba177a7beb6c72218e0e901bb5e9`  
		Last Modified: Thu, 21 Sep 2023 04:52:18 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; mips64le

```console
$ docker pull nextcloud@sha256:61342e952a804564dc9e6656074f21d4b7514e2b3930bbe5cad9ec159c7d7a41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.0 MB (367033104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a37616cbb3495ffa9a310461ec535b31214f3101334fdd7f2fce3bd16254dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 03:10:01 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Wed, 20 Sep 2023 03:10:05 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:07:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 10:07:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 10:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:09:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 10:09:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 10:25:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 10:25:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 10:26:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 10:26:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 10:26:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 10:26:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 10:27:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 10:27:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 12:33:27 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 14:34:03 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 14:34:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 14:34:10 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 14:35:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 14:35:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:50:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 14:50:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:50:26 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 14:50:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 14:50:33 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 14:50:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:50:39 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 14:50:43 GMT
EXPOSE 80
# Wed, 20 Sep 2023 14:50:46 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 20:42:30 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Sep 2023 20:42:34 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 20:42:38 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 21 Sep 2023 20:54:13 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 20:54:21 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Sep 2023 20:54:25 GMT
VOLUME [/var/www/html]
# Thu, 21 Sep 2023 20:54:32 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 21 Sep 2023 20:54:36 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Thu, 21 Sep 2023 20:54:43 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Thu, 21 Sep 2023 20:54:48 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Thu, 21 Sep 2023 20:57:50 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 20:58:02 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Thu, 21 Sep 2023 20:58:12 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Thu, 21 Sep 2023 20:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Sep 2023 20:58:30 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13be0169bbca45d04b6865d960fa18b85165b8512d8b6586743bc395e961aae5`  
		Last Modified: Wed, 20 Sep 2023 21:18:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78fa1c50adc35b8a5d3ed371ce4ecc5fdd6ddd827aac2af4c9f5dcc0295f4f4`  
		Last Modified: Wed, 20 Sep 2023 21:19:51 GMT  
		Size: 80.7 MB (80671000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a2620da2ab8ff2c4c00daed91ea144d334623c7de2d739f7e905cee010fa21`  
		Last Modified: Wed, 20 Sep 2023 21:18:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe5bafce3f10df8119507b329a6e98146bd701a42fd5f5b51efabde852a3b49`  
		Last Modified: Wed, 20 Sep 2023 21:20:32 GMT  
		Size: 20.1 MB (20053740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658c470a27f164500c0b36465086e61d4bf7c285975323d1760c41218aaa30a4`  
		Last Modified: Wed, 20 Sep 2023 21:20:19 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d8c9be245f2f3600146258dd57026cdb2b92acce2dc51b4990927983266273`  
		Last Modified: Wed, 20 Sep 2023 21:20:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4447aa8cbc0bdc413945a18adcc590be10f6f511e49c828e0b3f931fd25ec49`  
		Last Modified: Wed, 20 Sep 2023 21:29:36 GMT  
		Size: 12.2 MB (12167598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece72f787891fe36bce4674c9c2f458e2157dde1e7265e7e67710f5ca7d8beec`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebaad463f1b0c60d31c831e10f7d6ce95289918eef4da4549a73856d427f947`  
		Last Modified: Wed, 20 Sep 2023 21:29:40 GMT  
		Size: 10.5 MB (10501077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd6d0fb8026cec1e308c0736dc52430f402378082f302bef93008f4f9d7246c`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc9aa5c5dfeca97442ba3b8a33565c370534522927530baeec26de865bd3890`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19fca0609df3058afd752c476d131ca596b7961609819df49d333d8f1ee8ada`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb7eb938a7192b378468feabf6c05025a58e9e1038c43a2e390d8cf1e414c91`  
		Last Modified: Thu, 21 Sep 2023 21:29:42 GMT  
		Size: 19.8 MB (19794357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9beb91343910953f6b51df7a21e3d350e810adbfe6d14cc743cd843e6de09`  
		Last Modified: Thu, 21 Sep 2023 21:29:48 GMT  
		Size: 20.5 MB (20451163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198f5e611b32b8dd9b2bee2593c8e30c5cc0f23c45f94dd16b318183ddf9fff3`  
		Last Modified: Thu, 21 Sep 2023 21:29:24 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7840f38a7c954072c9719550c701af4bb76ac2b7a7385beb976d489b6f37d6c9`  
		Last Modified: Thu, 21 Sep 2023 21:29:21 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940fe0383c43deca3cf7cd7be9aa07f120d4191154a7590c06c7b86d3b09f3a0`  
		Last Modified: Thu, 21 Sep 2023 21:29:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8765d4a4a155591ee8eb30b8e51f569a286ba5db99017f99438ecb21b178318`  
		Last Modified: Thu, 21 Sep 2023 21:31:18 GMT  
		Size: 174.3 MB (174259438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61e6bba5143f6dd3ba32121b1e5d52452d39b3df5198cfe468a31b1a51e51af`  
		Last Modified: Thu, 21 Sep 2023 21:29:21 GMT  
		Size: 3.6 KB (3608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8aea3c8d925e22215b0f3758e1e62b833d60d2e487144b008aa656a9bac368`  
		Last Modified: Thu, 21 Sep 2023 21:29:21 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:b91ae36dd69afcc50d1f5451c1fcbb484fe2e7c48fc603e54457cc2bb415c782
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.0 MB (401048425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed5cfde236694a163d9bcc6787e5bd078c804bd29fcb0bb25f46157bce120eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 21:02:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 21:02:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 21:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 21:03:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 21:03:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 21:08:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 21:08:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 21:08:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 21:08:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 21:08:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 21:08:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:08:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:08:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 21:47:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:27:35 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 22:27:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 22:27:36 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 22:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:28:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:33:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:33:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:33:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:33:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:33:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 22:33:48 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:33:49 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:33:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 22:33:49 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 11:17:42 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Sep 2023 11:17:43 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 11:17:43 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 21 Sep 2023 11:22:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 11:22:39 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Sep 2023 11:22:40 GMT
VOLUME [/var/www/html]
# Thu, 21 Sep 2023 11:22:41 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 21 Sep 2023 11:22:41 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Thu, 21 Sep 2023 11:22:42 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Thu, 21 Sep 2023 11:22:42 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Thu, 21 Sep 2023 11:24:17 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 11:24:25 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Thu, 21 Sep 2023 11:24:26 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Thu, 21 Sep 2023 11:24:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Sep 2023 11:24:26 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115ac42043a1ac5a88aae3fb460d7ad62e1be1c67a7ff8b32864148113e2c22c`  
		Last Modified: Thu, 21 Sep 2023 00:31:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc90eef5a3f1d9aa3a000a7d8b39ed9d502ec6dd626af4d532190988b096da`  
		Last Modified: Thu, 21 Sep 2023 00:32:13 GMT  
		Size: 103.3 MB (103305381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11d9c0b01acf40609ca50b41cf6eec30ca37f7b60346417c98b944cd6ace0d1`  
		Last Modified: Thu, 21 Sep 2023 00:31:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1097574f783abc5487049e48142ce26a921051066df35ed7c1237b8ffc34c1`  
		Last Modified: Thu, 21 Sep 2023 00:32:46 GMT  
		Size: 21.5 MB (21488774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9d9c9bcc6c5d1f1e11956e19d46f88b83606ac3f60d0dbfbcdf47dcad8fc1`  
		Last Modified: Thu, 21 Sep 2023 00:32:41 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4045c5ffebd2a4ecdd6b2d8125275e561d356eb4c30c5967c786f69f2770c303`  
		Last Modified: Thu, 21 Sep 2023 00:32:41 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aeb6c7a5bb3a316b66dad6f26ed141128a76b1258b651b093fe27804f52063`  
		Last Modified: Thu, 21 Sep 2023 00:39:09 GMT  
		Size: 12.4 MB (12373528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e2384a625634256e966321a46a1fb90b78aef6382ea4a564708175858ec7ae`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896407af8187fd1eafb71cf9250d852d4e01fb0ce18e2c96dd4f0fef59502c65`  
		Last Modified: Thu, 21 Sep 2023 00:39:10 GMT  
		Size: 11.8 MB (11836353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db3b8d1c50baeaa413c0d42c4a6f8204e53aa2d4b5633834ec64812854e8a3`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7b9a40352a0d564e434f89b62953bacaba19976fdceb9d83fe303547b1fa4d`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a915ac0dedf520bf23b8352ea551d6e2fdd682b30772f452c27ff60bd729ab8`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84509fb066eaefa81283671cc0eae71e0c606a99dc630ac1cc40695f8d99f00f`  
		Last Modified: Thu, 21 Sep 2023 11:38:51 GMT  
		Size: 22.6 MB (22615361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdaea6f174ed791f54a2df118475ad09e09e9f165879ebc26237c68508dc8a4`  
		Last Modified: Thu, 21 Sep 2023 11:38:53 GMT  
		Size: 21.8 MB (21809028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c947742d1f37ed7cfd3668d4bd00071749c3052d2947457e9ea9f225f16e00d`  
		Last Modified: Thu, 21 Sep 2023 11:38:46 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f58c95c3db75b8dc8995d1c834962ab93e5f88346c585e8ef52a6197422de3`  
		Last Modified: Thu, 21 Sep 2023 11:38:44 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a568e483905ef27aafc612add57af7c37af52dc7dcf97baf7154cbe0b3b2e65d`  
		Last Modified: Thu, 21 Sep 2023 11:38:44 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044d6cc88ae8fcb7b65f1a4252316e96d3c6e70f716485e889326652a3ec5369`  
		Last Modified: Thu, 21 Sep 2023 11:39:22 GMT  
		Size: 174.5 MB (174487321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f45b4f8763ad3f301517e36e7e02a0b57e0b057ceb93dc8e1232019677f13f5`  
		Last Modified: Thu, 21 Sep 2023 11:38:44 GMT  
		Size: 3.6 KB (3609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c33abd6324b49eda1a4f49895813f4b187aacbd6d10bfb43cce5458260dbcd`  
		Last Modified: Thu, 21 Sep 2023 11:38:44 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:26-apache` - linux; s390x

```console
$ docker pull nextcloud@sha256:8fbdf3188fbce929ff6435418069c8e1712f99e710664f21ac723f1cbdf198f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.1 MB (365112073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fa0492937c231a5d5e6161c58f434e21b1d64a6af2012d8708e39febcc2d1f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:15:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:15:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:16:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:16:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:16:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:19:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 03:19:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 03:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 03:19:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 03:19:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 03:19:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:19:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:19:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:43:07 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 04:11:33 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 04:11:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 04:11:34 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 04:11:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 04:11:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:14:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 04:14:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:14:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 04:14:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 04:14:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 04:14:48 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:14:49 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 04:14:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 04:14:50 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 13:43:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         busybox-static         bzip2         libldap-common         libmagickcore-6.q16-6-extra         rsync     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Wed, 20 Sep 2023 13:43:57 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 20 Sep 2023 13:43:57 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 20 Sep 2023 13:45:39 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libgmp-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmagickwand-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libwebp-dev         libxml2-dev         libzip-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         gmp         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         sysvsem         zip     ;         pecl install APCu-5.1.22;     pecl install imagick-3.7.0;     pecl install memcached-3.2.0;     pecl install redis-6.0.0;         docker-php-ext-enable         apcu         imagick         memcached         redis     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query --search         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 13:45:41 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=32';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';         echo 'opcache.jit=1255';         echo 'opcache.jit_buffer_size=128M';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     mkdir -p /docker-entrypoint-hooks.d/pre-installation              /docker-entrypoint-hooks.d/post-installation              /docker-entrypoint-hooks.d/pre-upgrade              /docker-entrypoint-hooks.d/post-upgrade              /docker-entrypoint-hooks.d/before-starting;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 20 Sep 2023 13:45:41 GMT
VOLUME [/var/www/html]
# Wed, 20 Sep 2023 13:45:42 GMT
RUN a2enmod headers rewrite remoteip ;     {      echo 'RemoteIPHeader X-Real-IP';      echo 'RemoteIPInternalProxy 10.0.0.0/8';      echo 'RemoteIPInternalProxy 172.16.0.0/12';      echo 'RemoteIPInternalProxy 192.168.0.0/16';     } > /etc/apache2/conf-available/remoteip.conf;     a2enconf remoteip
# Wed, 20 Sep 2023 13:45:42 GMT
ENV APACHE_BODY_LIMIT=1073741824
# Wed, 20 Sep 2023 13:45:42 GMT
RUN {      echo 'LimitRequestBody ${APACHE_BODY_LIMIT}';     } > /etc/apache2/conf-available/apache-limits.conf;     a2enconf apache-limits
# Wed, 20 Sep 2023 13:45:42 GMT
ENV NEXTCLOUD_VERSION=26.0.6
# Wed, 20 Sep 2023 13:46:21 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2 "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc "https://download.nextcloud.com/server/releases/nextcloud-26.0.6.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 13:46:32 GMT
COPY multi:460d0253b10a0268ebfb8482b4fa36d0d335e8207e35802a68bf2d6134195fbb in / 
# Wed, 20 Sep 2023 13:46:32 GMT
COPY multi:bed047b97a268e53d9af8fc32cf3b9fc25306fd16316e9a09031943c00c6b402 in /usr/src/nextcloud/config/ 
# Wed, 20 Sep 2023 13:46:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 13:46:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca32f8ccfb61fd7b80ac92910bb82312c56b13482192ddeca040f28dee22cc9c`  
		Last Modified: Wed, 20 Sep 2023 05:59:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e52ee364693e5711dc589e82f194e3efe065fd0f053a32ba58338fe64d5ca98`  
		Last Modified: Wed, 20 Sep 2023 05:59:21 GMT  
		Size: 80.8 MB (80804520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8ef296ea27f8b5881996cfcec85005d1b87dcc362dcba3e4ecf2f03b444341`  
		Last Modified: Wed, 20 Sep 2023 05:59:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b098b51a9a89d9da9b5005b21d65949cd9ec75f9f7b130fe596f7ebc07bb6dd2`  
		Last Modified: Wed, 20 Sep 2023 05:59:37 GMT  
		Size: 20.1 MB (20082365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe13c8e74b3f28e948710777e0f4ac759072add1f62785c071a72cae42f6e77`  
		Last Modified: Wed, 20 Sep 2023 05:59:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16cc070d34d9d8fe0040c4f382334b678eb219e7d2aa3b3fee4dfea400bb49b`  
		Last Modified: Wed, 20 Sep 2023 05:59:34 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a2932911b35399b7c80be5e3c6cad913a299008e7e396eca186cbadae993f4`  
		Last Modified: Wed, 20 Sep 2023 06:03:13 GMT  
		Size: 12.4 MB (12372533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17319ba697a9076245bd26130b06568b6edfd5c1df2f4afb81a7a116fb2470de`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b70b8fec8e3abaad19f9454237dd0b96ade8c40392500d42a850bd91958c534`  
		Last Modified: Wed, 20 Sep 2023 06:03:13 GMT  
		Size: 10.5 MB (10474094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79dc37078ce62a3886a1eb2f517fb5da8b727d6e235fd3c11ed611889f903259`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1a386f288221fbb65d01c28f3671e735fb8b9a313abbaa6c9dc1b5629d8950`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d278f95a0fca2757e6a96dfcdcf3f89b94e2ec78e1fee81bfffea59a4b09dce`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10eec5510208b48b8a4f3b7a834b0bedba13dacdcf1bc919582d77c131ee8a39`  
		Last Modified: Wed, 20 Sep 2023 13:53:44 GMT  
		Size: 19.3 MB (19292481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488345eaf22c4062b3f79c3b288404db13fa65fa5f0a850ec392c8971bb42753`  
		Last Modified: Wed, 20 Sep 2023 13:53:45 GMT  
		Size: 20.1 MB (20098296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08eb9630511d53bd80edd2ce6f8b0b22065d97e061972b080799a9c4f7dd620`  
		Last Modified: Wed, 20 Sep 2023 13:53:42 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177ccfe84f8963534998427e120e02e937ff39547ad260f90c84ae57f2b9bb2a`  
		Last Modified: Wed, 20 Sep 2023 13:53:41 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf3c058f1f24f17c35b6f340deb2c7d2e8c7a76007db0fed28636959c07b7e`  
		Last Modified: Wed, 20 Sep 2023 13:53:41 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b46e4c6a2563fd91b427da1165d5f42b9fbb2883602cd26885bd304185552`  
		Last Modified: Wed, 20 Sep 2023 13:54:00 GMT  
		Size: 174.5 MB (174484594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7c9f04c167e377b153396145566c8d1e7bc541178775a56b774fe6638cf94d`  
		Last Modified: Wed, 20 Sep 2023 13:53:41 GMT  
		Size: 3.6 KB (3609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21be939c1976baa87cbe04002d22f2e455048cbb7ace9b9ce2c0a48560901f92`  
		Last Modified: Wed, 20 Sep 2023 13:53:41 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
