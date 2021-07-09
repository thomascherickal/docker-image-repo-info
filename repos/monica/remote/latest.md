## `monica:latest`

```console
$ docker pull monica@sha256:c5df61b7ca64c4c3683dddeeb0c69e9cd9e5c1d0759b06e6a4b080aca069d64a
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

### `monica:latest` - linux; amd64

```console
$ docker pull monica@sha256:26f3be02f2b870f410620cb4678dda190a93173f05c9b556479f9ca36ad62a4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.9 MB (188936242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0244d9510f3341d460de74516294f0d9e72442164d5d359eda1e7a2763531e`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 11:48:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 11:48:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 11:48:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 11:48:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 11:48:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 11:55:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 11:55:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 11:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 11:55:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 11:55:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 11:55:55 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 11:55:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 12:25:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 22:25:50 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 22:25:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 22:25:51 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 22:26:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 22:26:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:33:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 22:33:11 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:33:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 22:33:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 22:33:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 22:33:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:33:15 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 22:33:16 GMT
EXPOSE 80
# Thu, 01 Jul 2021 22:33:16 GMT
CMD ["apache2-foreground"]
# Fri, 02 Jul 2021 01:20:20 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 02 Jul 2021 01:20:25 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 01:22:00 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 01:22:01 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 02 Jul 2021 01:22:01 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 02 Jul 2021 01:22:03 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 02 Jul 2021 01:22:04 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 02 Jul 2021 01:22:05 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 02 Jul 2021 01:22:05 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 01:22:05 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 02 Jul 2021 01:22:06 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 02 Jul 2021 01:22:25 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 01:22:26 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 02 Jul 2021 01:22:26 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 02 Jul 2021 01:22:27 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b85dd8f01492a64ab518247894d5b93db91b5ef9c770b601b37f612278b602`  
		Last Modified: Wed, 23 Jun 2021 13:53:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8589b26a90be6577309788924232d8900e0e44f0a7fb4ca01c32c6467578a27d`  
		Last Modified: Wed, 23 Jun 2021 13:53:50 GMT  
		Size: 76.7 MB (76680976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5af5d6419462987bdb2cd60de0729dcf0c35933ca87692f2eb9ca1ae292a642`  
		Last Modified: Wed, 23 Jun 2021 13:53:31 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614ec6f0b8d6a562071e6a2584ca97b4237364aa3b78b00aa6c601a00c80d019`  
		Last Modified: Wed, 23 Jun 2021 13:54:26 GMT  
		Size: 18.7 MB (18679261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b28f3797fbefaacc6339a39139cd689c6038bdbe1ee96bd947d58397be3538`  
		Last Modified: Wed, 23 Jun 2021 13:54:22 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bcb7d2e6b049343069918b727a239aa0ae67500a2f20744af37dd6c89d90d9`  
		Last Modified: Wed, 23 Jun 2021 13:54:22 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e392fffccd27c0805336bea7438b6bc9edb2668be13f12cdc620c79a2446e7`  
		Last Modified: Thu, 01 Jul 2021 23:23:26 GMT  
		Size: 11.0 MB (11012860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae69fa2279aa8ac4fe1ddebf9cceba0616c7169834f0e5ed25c5595912b92d`  
		Last Modified: Thu, 01 Jul 2021 23:23:22 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4178ef63c89a872ef795e80aa423fabf22f97901e49e4ddfe159d804ba470`  
		Last Modified: Thu, 01 Jul 2021 23:23:26 GMT  
		Size: 14.5 MB (14495057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de485468a90ce29299f5e02ab1ae0f08bc8871106737a68533c5dbdffc0e3030`  
		Last Modified: Thu, 01 Jul 2021 23:23:22 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654ffd37175d69da64f21014036d4824fcd1007ef4a5372da07408c4cfdcc87`  
		Last Modified: Thu, 01 Jul 2021 23:23:22 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49deb1d5a62eb8fcd25265dfec3f0f3b2b4cf129f6989adbfe8b2acfccd71b80`  
		Last Modified: Thu, 01 Jul 2021 23:23:22 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e6aa240c9e06f7b6f1c9edd82e65c6e04fa9c3b790d480b369a1444c4b979`  
		Last Modified: Fri, 02 Jul 2021 01:27:29 GMT  
		Size: 1.4 MB (1356533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd1b11b9fe65525e25e7e217ce7c80cff5b81fe30839e938a0b2093f564cb6e`  
		Last Modified: Fri, 02 Jul 2021 01:27:30 GMT  
		Size: 5.0 MB (5018510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668e6bde2c5dace0a4ff68f2edb8236f15d162b4a25bd2965ea13f42468b660c`  
		Last Modified: Fri, 02 Jul 2021 01:27:28 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05ce118d08793f81ed9648f8e2edda4418c788b4959589e373b7d8c926c2590`  
		Last Modified: Fri, 02 Jul 2021 01:27:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f845670e4e7a557cd60d559d1850f19ef0cd41074cb6cb0358cce4626ecf84`  
		Last Modified: Fri, 02 Jul 2021 01:27:26 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ef04da123918f4d2868e4948e50365ca53387528f97d3ad3d62a88dc3e9d97`  
		Last Modified: Fri, 02 Jul 2021 01:27:26 GMT  
		Size: 8.3 KB (8298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f1c08c6b08764d4c53acd540601866d2aff4301e56209ea672ab7c68df15ee`  
		Last Modified: Fri, 02 Jul 2021 01:27:36 GMT  
		Size: 34.5 MB (34530343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2155f0b23845cf1b594ef6d330b68bf584613d64303cf9b4a2dfa6a97f7fb9a8`  
		Last Modified: Fri, 02 Jul 2021 01:27:26 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; arm variant v5

```console
$ docker pull monica@sha256:62afcd6fc3dcc4725d70aae8718c4e1aa276aaa830eb8e24a843f58a87b38da9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166518549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0080474b23879f51ff74b7ed366849d5d0c79f6123023d0c99cb9442e77b242`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:34:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 06:34:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 06:35:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:35:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 06:35:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 06:41:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 06:41:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 06:41:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 06:41:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 06:41:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 06:41:35 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 06:41:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 07:04:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 23:02:08 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 23:02:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 23:02:09 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 23:02:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 23:02:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:07:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 23:07:20 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:07:22 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 23:07:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 23:07:23 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 23:07:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:07:24 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 23:07:24 GMT
EXPOSE 80
# Thu, 01 Jul 2021 23:07:25 GMT
CMD ["apache2-foreground"]
# Fri, 02 Jul 2021 00:59:20 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 02 Jul 2021 00:59:31 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 01:03:53 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 01:03:55 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 02 Jul 2021 01:03:56 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 02 Jul 2021 01:03:58 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 02 Jul 2021 01:04:00 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 02 Jul 2021 01:04:02 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 02 Jul 2021 01:04:03 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 01:04:04 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 02 Jul 2021 01:04:04 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 02 Jul 2021 01:04:59 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 01:05:02 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 02 Jul 2021 01:05:02 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 02 Jul 2021 01:05:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4201a900b66f4e05c8ee53ef7ecdffa56d4cfc141826c4899ba2c7ea1565c3`  
		Last Modified: Wed, 23 Jun 2021 08:37:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8759f5b6f404f221d7035198880caf6e5b60d43c01daf59b9c7ff32e8ba5038f`  
		Last Modified: Wed, 23 Jun 2021 08:37:51 GMT  
		Size: 58.8 MB (58820428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee84cde96b6e1abd89640d87273fd846cad74593b3ec8bdd0167bb76f06398`  
		Last Modified: Wed, 23 Jun 2021 08:37:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d04a75937c26e6facc2a34e28c4f30008fb2c8c38d4a6109ab3bd73a1a4d516`  
		Last Modified: Wed, 23 Jun 2021 08:38:40 GMT  
		Size: 18.0 MB (18026172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ecd491048519ab1e7d82a3cf53d86795ba9b3b230f90332de7efe0d76f16cd`  
		Last Modified: Wed, 23 Jun 2021 08:38:29 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b63bc3f991d218876d985827b11cbce08ca267e836215529cbbfbd0a0abf7b`  
		Last Modified: Wed, 23 Jun 2021 08:38:29 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbc1650cde5b61032f9d21a506193f3985f71e237d9b79d00f7bfa2a6e59282`  
		Last Modified: Thu, 01 Jul 2021 23:31:02 GMT  
		Size: 11.0 MB (11010895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03520e9997e75b63041db70ba89c6c4363ca4bca7039312855ec226b4a11dba6`  
		Last Modified: Thu, 01 Jul 2021 23:30:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70034c8afe446f0d9aa9e4e4df7337ae01a96a8dc12f2829e8007f1d07b1e351`  
		Last Modified: Thu, 01 Jul 2021 23:31:08 GMT  
		Size: 13.2 MB (13206722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bb002cf3cb89bdd38bcf17b81ec79f5e3b4ca4c11f29d101af4382c4541489`  
		Last Modified: Thu, 01 Jul 2021 23:30:57 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8d2f178a1d1fa775fc11eff2d6ac476e96a4598a2c870d81bf02db61de6e29`  
		Last Modified: Thu, 01 Jul 2021 23:30:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b859f05ea298c92f6ee1db2d1d15877d5f8f36f8f3c38ed0c91aa32a27994`  
		Last Modified: Thu, 01 Jul 2021 23:30:57 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe590960d967108663012ea5c71ae9263e5d467e89b34e98e4187e45119b7db`  
		Last Modified: Fri, 02 Jul 2021 01:11:56 GMT  
		Size: 1.3 MB (1295777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cc8b5e66b7b62409715ae03cfa38b2c005f65ae6e10eb3a2552c1a5edd4af5`  
		Last Modified: Fri, 02 Jul 2021 01:11:58 GMT  
		Size: 4.7 MB (4736118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0199a5f0ee1c3f3fa591f5f93f8b0743610b95761b1e7f58441a2ecd5b467856`  
		Last Modified: Fri, 02 Jul 2021 01:11:55 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7f87dc9591aa16b770d5af9a997c8a04ea3a782a3f05a0d7f590c36bcda364`  
		Last Modified: Fri, 02 Jul 2021 01:11:53 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8127ad665b92aa218f3cb8792486c4b230040ff3b2cdbdfccf920caa52c4bb3a`  
		Last Modified: Fri, 02 Jul 2021 01:11:53 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2613b04f26533ea2b5c6f2bddf161a1d2fca5d888a17bee507c2621d2bca04a7`  
		Last Modified: Fri, 02 Jul 2021 01:11:53 GMT  
		Size: 8.3 KB (8307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36adba0694c363fbb2857b6fb5521b405663b9a7427a5f9edd30eaf52a63f32b`  
		Last Modified: Fri, 02 Jul 2021 01:12:41 GMT  
		Size: 34.5 MB (34526620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d1f1fa4740dc054626ed3951c8fdb2fd9c3e0fed5251fbc4adddde406d7d96`  
		Last Modified: Fri, 02 Jul 2021 01:11:53 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; arm variant v7

```console
$ docker pull monica@sha256:6e242af3931d3c7f32cc7e83e93f3bccde56970aaeae0a7f3e7039c3b66b5557
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163572905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a81a9a8f6c0619889dd8b04563677d4ceba3044a7c710eeaedd24187333b404`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:21:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 08:21:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 08:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:22:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:22:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:27:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 08:27:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 08:27:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 08:27:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 08:27:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 08:27:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 08:27:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:06:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 22:45:30 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 22:45:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 22:45:31 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 22:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 22:45:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:50:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 22:50:24 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:50:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 22:50:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 22:50:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 22:50:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:50:27 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 22:50:28 GMT
EXPOSE 80
# Thu, 01 Jul 2021 22:50:28 GMT
CMD ["apache2-foreground"]
# Fri, 02 Jul 2021 03:22:14 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 02 Jul 2021 03:22:23 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 03:26:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 03:26:40 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 02 Jul 2021 03:26:40 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 02 Jul 2021 03:26:42 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 02 Jul 2021 03:26:44 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 02 Jul 2021 03:26:46 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 02 Jul 2021 03:26:46 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 03:26:47 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 02 Jul 2021 03:26:47 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 02 Jul 2021 03:27:38 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 03:27:40 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 02 Jul 2021 03:27:40 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 02 Jul 2021 03:27:41 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9600bb4c83e3ef3465228eed7d6e9dfed7dc9078d2ab47f0bbdc8ccd6cb2b4`  
		Last Modified: Wed, 23 Jun 2021 11:51:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4b7395146be79190767115c26cc6b70ac8d5af36c4a7acf9de1f34d06b41d7`  
		Last Modified: Wed, 23 Jun 2021 11:52:18 GMT  
		Size: 59.5 MB (59514051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3641f6e3173b95d08e8b4ec00f48cb7e09d9813f88a086a422173594dfc93ddd`  
		Last Modified: Wed, 23 Jun 2021 11:51:40 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7d1aa9268ffe2596e041fe0130bbdc37fb7e587a9b8d7c5346360e2f27b41d`  
		Last Modified: Wed, 23 Jun 2021 11:53:09 GMT  
		Size: 17.5 MB (17481801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56adf5c38075c402f8bf5f30dee3d2dd1d1f5c327b12641f29af33f5ba950a`  
		Last Modified: Wed, 23 Jun 2021 11:52:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bf5eeb5d260e70dda8e6cf6bf12b837eca9e5650117ad4e659861a5ecc31f5`  
		Last Modified: Wed, 23 Jun 2021 11:52:58 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3087c5ce84e1a06e9cd11d8aad1f54513da18c41b3a7fcdcbda61da272e61a02`  
		Last Modified: Thu, 01 Jul 2021 23:43:04 GMT  
		Size: 11.0 MB (11010968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21b01e564716bac9d8e421f0b19ce534686684a40688df70b24c7c1bf70b3b5`  
		Last Modified: Thu, 01 Jul 2021 23:42:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5b4bdde0f6190e859020a734d741ce99aaf74f0c7fdd106151c2a7a016908a`  
		Last Modified: Thu, 01 Jul 2021 23:43:09 GMT  
		Size: 12.5 MB (12503665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22296f5406acd9f11c8588603f978e49d3237f8d99e34187964d5b7a98fae0`  
		Last Modified: Thu, 01 Jul 2021 23:42:59 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab648ea29674e3ccc2dd322af7c825e04d0841efcfb1c889921aaa83f1c0841`  
		Last Modified: Thu, 01 Jul 2021 23:42:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fed51014aca8b1e6807b5e7c470c01ab618a8be1f9bebc13d5763707ddd4fd6`  
		Last Modified: Thu, 01 Jul 2021 23:42:59 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767478f40acdb47c07df4284e72616c71e200c376ca7cb0b405e267d16b9f8df`  
		Last Modified: Fri, 02 Jul 2021 03:39:52 GMT  
		Size: 1.2 MB (1175553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8471703c88a6d23c8efb283d0974a5846ad6540658f158aabc9acda7ff141c2`  
		Last Modified: Fri, 02 Jul 2021 03:39:54 GMT  
		Size: 4.6 MB (4597311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efa62c2e4b3828c6c747caea9166477abdf9dfe771e74551e9acb0babfa7df1`  
		Last Modified: Fri, 02 Jul 2021 03:39:51 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa075c60b748610777a168bd1cb32b529c0e0bb7dab17c6382005cecfbf24f1`  
		Last Modified: Fri, 02 Jul 2021 03:39:50 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ec8cea900dffa93cc7f98bf55ca74a84d8e6276e779e880a7802d35dd49e40`  
		Last Modified: Fri, 02 Jul 2021 03:39:49 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f375c183f353ec1cf9d7bebe35f323380d3f238af49e040d9a6f4ba6d0e6742`  
		Last Modified: Fri, 02 Jul 2021 03:39:49 GMT  
		Size: 8.3 KB (8309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b875b235ba82e387192ec601470e1d640ae8192240aaed3583d038ff7561344`  
		Last Modified: Fri, 02 Jul 2021 03:40:35 GMT  
		Size: 34.5 MB (34526632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d9cea338feee587f34065508876b6067f5e727481f23669b09a2a5822119bf`  
		Last Modified: Fri, 02 Jul 2021 03:39:49 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; arm64 variant v8

```console
$ docker pull monica@sha256:d216dca21f6b3f3ffaae73bffb2155ce3bb479d882d003b0946c516b6f44760d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180599135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc873f04457980db1b0efa91df9dc30da9d0db7cecca8058e0211e436b457f76`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:48:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 08:48:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 08:48:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:48:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:48:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:53:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 08:53:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 08:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 08:53:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 08:53:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:53:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:16:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 21:56:27 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 21:56:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 21:56:28 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 21:56:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 21:56:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:59:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 21:59:50 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:59:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 21:59:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 21:59:51 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 21:59:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:59:52 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 21:59:52 GMT
EXPOSE 80
# Thu, 01 Jul 2021 21:59:52 GMT
CMD ["apache2-foreground"]
# Fri, 02 Jul 2021 00:46:21 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 02 Jul 2021 00:46:25 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 00:48:04 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 00:48:05 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 02 Jul 2021 00:48:05 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 02 Jul 2021 00:48:06 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 02 Jul 2021 00:48:07 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 02 Jul 2021 00:48:08 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 02 Jul 2021 00:48:08 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 00:48:08 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 02 Jul 2021 00:48:09 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 02 Jul 2021 00:48:27 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 00:48:29 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 02 Jul 2021 00:48:29 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 02 Jul 2021 00:48:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce6585fd70baac65871dafb05b7f408940165f163c30d7e0f9ec3518709e908`  
		Last Modified: Wed, 23 Jun 2021 10:25:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab6c01ccebb7fc71b44dfe6966672e34b47ea5e22d53a11e4481e76243cd44b`  
		Last Modified: Wed, 23 Jun 2021 10:25:24 GMT  
		Size: 70.4 MB (70356352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ed9f96098643713fabf62c17f792254db16c6623e3cec0b4a4ea602af2e742`  
		Last Modified: Wed, 23 Jun 2021 10:25:12 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6852e08c882a542c19980b469e16cebe09c20c56cb6a883fe46d7fa71c77a5bf`  
		Last Modified: Wed, 23 Jun 2021 10:26:10 GMT  
		Size: 18.6 MB (18579813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650d5012e5fa16b3bcc69043ccc3b45a8e75bd3651354579204af7abe7ae4eae`  
		Last Modified: Wed, 23 Jun 2021 10:26:01 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390447f485b4746ca973bb40b4a5ef8edc132fc2fd3b4c1e3681b22c5fa1ca47`  
		Last Modified: Wed, 23 Jun 2021 10:26:01 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee51f39f7992261f66c409d0d9c5aabe453af6328e9716b785dc001a7467cfe7`  
		Last Modified: Thu, 01 Jul 2021 22:39:56 GMT  
		Size: 11.0 MB (11011587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6b0c47ed6d56acc1e9258e07589ed29aec712ddc1806e816da90a1ad0d00a5`  
		Last Modified: Thu, 01 Jul 2021 22:39:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2292d6b4a6921e4bbce7cca480263548a2542a01ee0a87f5d49817d765f2b0a`  
		Last Modified: Thu, 01 Jul 2021 22:39:56 GMT  
		Size: 13.9 MB (13926725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d828625d6d523e3cf5c0b2e9b761a6c44c1f865c42c55d7d2f60832e6fa0dd63`  
		Last Modified: Thu, 01 Jul 2021 22:39:53 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb5546393632660201ccea2cb7f1dea76727d3a2f4be4bcbd418d35e991774`  
		Last Modified: Thu, 01 Jul 2021 22:39:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f20f20f9a3ecc7ac38c03c1e4ab4a1685e2a2d659e969a45c0b4e819c504c0`  
		Last Modified: Thu, 01 Jul 2021 22:39:53 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6aaf0d4943756aede82a4ade18c15dde3beab2c0819901909947887a40c33b`  
		Last Modified: Fri, 02 Jul 2021 00:53:53 GMT  
		Size: 1.3 MB (1313696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6011cb5e2262062e3f707559d361e88d219d82cb9fb6c0032bde04728dffa`  
		Last Modified: Fri, 02 Jul 2021 00:53:54 GMT  
		Size: 5.0 MB (4951021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc37a1b9def769b9e82c4d37fc754ee068ab2f7dcde7eaf1a3c1fef2678919b`  
		Last Modified: Fri, 02 Jul 2021 00:53:53 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9025a1cff1795f23c50ab6ed272d2cf781fda33ec1637031fa498be210555c14`  
		Last Modified: Fri, 02 Jul 2021 00:53:50 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557a75dd69116fc3cdcad7621be2f74e83af7e7858b142684047add5bfa22c8b`  
		Last Modified: Fri, 02 Jul 2021 00:53:50 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2835e11b9b06605b8e8152b0d9e3c8a5950ae72d72d523dd0ebed21538715ceb`  
		Last Modified: Fri, 02 Jul 2021 00:53:50 GMT  
		Size: 8.3 KB (8307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e7105846e905598e2330d878fb4821a6990cd50aef9a1288df7b617a4e5146`  
		Last Modified: Fri, 02 Jul 2021 00:54:00 GMT  
		Size: 34.5 MB (34528110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f89b3580f24b9976d0ddf5cbfcf65021caeabbbf1582e7655b4e88d61004b2`  
		Last Modified: Fri, 02 Jul 2021 00:53:51 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; 386

```console
$ docker pull monica@sha256:c774650a7e445d3d0dcf52dcb5a9f72e9cf23f89c194c808adaf52280d334824
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194911496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb4952c74a2dcccbede7447d6eae62119e98926cfd05e98c4220dea9822f8cb`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 09:40:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 09:40:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 09:40:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 09:40:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 09:40:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 09:49:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 09:49:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 09:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 09:49:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 09:49:46 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 09:49:46 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 10:26:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 23:24:58 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 23:24:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 23:24:59 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 23:25:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 23:25:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 23:30:14 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:30:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 23:30:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 23:30:15 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 23:30:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:30:16 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 23:30:16 GMT
EXPOSE 80
# Thu, 01 Jul 2021 23:30:16 GMT
CMD ["apache2-foreground"]
# Fri, 02 Jul 2021 02:50:07 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 02 Jul 2021 02:50:12 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 02:51:58 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 02:51:59 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 02 Jul 2021 02:52:00 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 02 Jul 2021 02:52:01 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 02 Jul 2021 02:52:02 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 02 Jul 2021 02:52:03 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 02 Jul 2021 02:52:03 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 02:52:03 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 02 Jul 2021 02:52:04 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 02 Jul 2021 02:52:27 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 02:52:29 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 02 Jul 2021 02:52:29 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 02 Jul 2021 02:52:30 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851ded1e6779ac12f2623fa13c3d156987e0e3748e10171438e042c4a18cada8`  
		Last Modified: Wed, 23 Jun 2021 12:27:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9108f1298d19c1c39f13396485b32141017e3d97dcc7093d43854940c92b6c`  
		Last Modified: Wed, 23 Jun 2021 12:28:14 GMT  
		Size: 81.2 MB (81230041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a8cc691843125fa492ce4109092746e47e36d222eceef5b59dd10271176374`  
		Last Modified: Wed, 23 Jun 2021 12:27:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce571916f9fd350c507c0b0f4ba7db9c473cb95da721dfeab5acd167c05197`  
		Last Modified: Wed, 23 Jun 2021 12:29:05 GMT  
		Size: 19.1 MB (19115037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abad9c9b3f342c41ff79e0b1832309d795f17e4aaafd51a979891c9c747684c`  
		Last Modified: Wed, 23 Jun 2021 12:28:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecb5db768b6cdd9c3b371c253bc49fc82700b113499943217799b6cf74aab9`  
		Last Modified: Wed, 23 Jun 2021 12:28:58 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c6e5b2eabed94cce778a9e0d0aa4e15d955bdc490973e19f6b37db2ac6acd8`  
		Last Modified: Fri, 02 Jul 2021 00:24:10 GMT  
		Size: 11.0 MB (11012171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa93203bbccc11301ee02e3e88f995960707eb85ff0a8e1c6d0bfc238cc0e36`  
		Last Modified: Fri, 02 Jul 2021 00:24:06 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f65c89965149d1832a4c422423e4dd4962752ebb23096c62e8d98398c039bf`  
		Last Modified: Fri, 02 Jul 2021 00:24:11 GMT  
		Size: 14.8 MB (14794475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e718358c0e49e05142b2f6892ded5a221750a855f305d1522d3a489e190e6497`  
		Last Modified: Fri, 02 Jul 2021 00:24:06 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5f55ea4ed95f01ee0ea25f581d41a238ce6afa909282015b58e533a9891ef0`  
		Last Modified: Fri, 02 Jul 2021 00:24:06 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83493a7fa3e73dc846fbdb7f9d86613857c9c4e4160654ecec6be73705a596`  
		Last Modified: Fri, 02 Jul 2021 00:24:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a957afbb71ebeec7f12665e2116108cf758527fbba33061d9b3db00fa8f727`  
		Last Modified: Fri, 02 Jul 2021 02:58:30 GMT  
		Size: 1.4 MB (1358565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071ea77d3668021ba802e6159f2e50337156e5304f54fd3f9041d334204781ea`  
		Last Modified: Fri, 02 Jul 2021 02:58:30 GMT  
		Size: 5.1 MB (5057469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c3f7a7ca4ee037fbacd31c576ef4d36f9ddf2c6f31f36a34fa039e82747117`  
		Last Modified: Fri, 02 Jul 2021 02:58:29 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4821f7b9742c0d63b4d36850b39f2b831661d83a2d148317d60d10f18c53b40a`  
		Last Modified: Fri, 02 Jul 2021 02:58:26 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee7bc0bf3265a00eeae1b0c95254892332f7f1edf36b3dc014377b2acce39e`  
		Last Modified: Fri, 02 Jul 2021 02:58:26 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c0eab60899b01ff49143e5e1c523b52e5b279e3f35e6f15f3dae867439c60c`  
		Last Modified: Fri, 02 Jul 2021 02:58:26 GMT  
		Size: 8.3 KB (8302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6c24e6f4ea676b592e25fad56690ed4ae04ce7f45a0b5c903e111f7e676436`  
		Last Modified: Fri, 02 Jul 2021 02:58:39 GMT  
		Size: 34.5 MB (34529473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b18b37a99e198e6f35aebe5fcd8e1023b7efff5ec5cd45b2914b4613c7d943d`  
		Last Modified: Fri, 02 Jul 2021 02:58:26 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; mips64le

```console
$ docker pull monica@sha256:65c35cfe648e3ed567a74de174eadc329437f150b27f01042806bd2b8251cf43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171180206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad6e7607b3e41f3bd3aa8af671ddd7b925a9d1afa14043a59aee9dbdc505655c`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:39:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 02:39:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 02:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:40:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 02:40:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 02:52:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 02:52:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 02:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 02:53:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 02:53:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 02:53:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 03:45:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 20:58:31 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 20:58:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 20:58:32 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 20:58:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 20:58:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:10:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 21:10:58 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:11:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 21:11:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 21:11:01 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 21:11:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:11:01 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 21:11:02 GMT
EXPOSE 80
# Thu, 01 Jul 2021 21:11:02 GMT
CMD ["apache2-foreground"]
# Thu, 01 Jul 2021 22:52:59 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 01 Jul 2021 22:53:11 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 01 Jul 2021 22:58:25 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 01 Jul 2021 22:58:27 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 01 Jul 2021 22:58:27 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 01 Jul 2021 22:58:29 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 01 Jul 2021 22:58:32 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 01 Jul 2021 22:58:34 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 01 Jul 2021 22:58:34 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 22:58:34 GMT
ENV MONICA_VERSION=v3.1.3
# Thu, 01 Jul 2021 22:58:35 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Thu, 01 Jul 2021 22:59:38 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 01 Jul 2021 22:59:41 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:59:41 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Thu, 01 Jul 2021 22:59:41 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c90d345f251f9a0ec80cf41b5f35febb67c1c989281d9e68b2aeefee1c00143`  
		Last Modified: Wed, 23 Jun 2021 05:55:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf25841fee636dffd0610ecca37bade0d96a921f21482eda088538659d329a`  
		Last Modified: Wed, 23 Jun 2021 05:55:57 GMT  
		Size: 61.4 MB (61404106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b88a019f1da6587ce2665903b08be861bc197f91d09bfbfb6e62a368de4a231`  
		Last Modified: Wed, 23 Jun 2021 05:55:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208dcf88dd78c21b0c19c351345924790c3caa4bbca1580e2e289d738c874ab`  
		Last Modified: Wed, 23 Jun 2021 05:56:42 GMT  
		Size: 18.6 MB (18611849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe3845bbf14eccd94071a1ab8d234fe05503b03c7d92b53ed1643a1ca33d9a4`  
		Last Modified: Wed, 23 Jun 2021 05:56:29 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec3aa526d170c9dd2f45b8bd19f5f8f080e143f30ba8431c0e6d9105ec4d0c`  
		Last Modified: Wed, 23 Jun 2021 05:56:29 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a8bb414148c8c83b8b4532efd1488cf27b42a9ed7b72c161b991fc8117b58e`  
		Last Modified: Thu, 01 Jul 2021 21:40:46 GMT  
		Size: 11.0 MB (11010175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2af5cf3fda9cd7153a869d6bc884a82599a23b69536c1f4503543a8d43c668`  
		Last Modified: Thu, 01 Jul 2021 21:40:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95521ff0602b1145c87be61feda65abd391b7aeb4879b71a6d37ab8c99dcc01a`  
		Last Modified: Thu, 01 Jul 2021 21:40:52 GMT  
		Size: 13.4 MB (13433092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedfc9afea5673a7384a1c85f51ae76e70c2a0de539660e48e5a3374bbfae16a`  
		Last Modified: Thu, 01 Jul 2021 21:40:40 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30685c27d70bddf3103a0cf60089d71483bb6dbe080832862065c60804f0bffc`  
		Last Modified: Thu, 01 Jul 2021 21:40:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e37ff7e5346b993685514b6d5a606596c32e471446d6e86284a73a03e3f990`  
		Last Modified: Thu, 01 Jul 2021 21:40:40 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbb0db6e047a42a361e49c0af9d0906519a3ba532f8ecf40284deef1b2bb0a5`  
		Last Modified: Thu, 01 Jul 2021 23:06:55 GMT  
		Size: 1.4 MB (1445396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126cdb83296a19949fca9c8929ba7ed57b87dd86f7bee6a267ac6df8f240cbd5`  
		Last Modified: Thu, 01 Jul 2021 23:06:58 GMT  
		Size: 4.9 MB (4920749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6a164cd51cefcf0f6e4ab0edb22180ede26f8ccf0f2992cb3ea92b117a03b8`  
		Last Modified: Thu, 01 Jul 2021 23:06:54 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9091a932f0b08d547ad302f4997490b9f659ee69805d099af7b7dff35c0db9`  
		Last Modified: Thu, 01 Jul 2021 23:06:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c9d1f9c49722f51803bb9c205df9e9cc4eb453df0657d16df5d3cf7e14792a`  
		Last Modified: Thu, 01 Jul 2021 23:06:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bd1f9e77d3552a57f71fd92faa03186b9cd949c46bbd059c9f023d89fafded`  
		Last Modified: Thu, 01 Jul 2021 23:06:51 GMT  
		Size: 8.3 KB (8307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff54e0e4aa246b6d659da31270007ceeefaae10a7aac1288e43362ca9b5ec188`  
		Last Modified: Thu, 01 Jul 2021 23:07:33 GMT  
		Size: 34.5 MB (34525215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfb0a5124cbb47953bb313795b22e4123e17628df6dad69a892c2cc1d7b5d2`  
		Last Modified: Thu, 01 Jul 2021 23:06:51 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; ppc64le

```console
$ docker pull monica@sha256:eefaf9a929e882780605b1e76ce484e70800be3e3c0bb7afb884d215232a89c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.2 MB (200210108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3344ac008119631e8826f5a5497ff751b6881f00db4274b978d1d307e0447af5`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 04:04:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 26 Jun 2021 04:04:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 26 Jun 2021 04:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 04:09:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 04:09:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 04:24:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 26 Jun 2021 04:24:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 26 Jun 2021 04:26:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 26 Jun 2021 04:26:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 26 Jun 2021 04:26:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 26 Jun 2021 04:26:47 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 26 Jun 2021 04:26:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 26 Jun 2021 04:26:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 04:27:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 04:27:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 05:48:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 08 Jul 2021 13:46:45 GMT
ENV PHP_VERSION=8.0.8
# Thu, 08 Jul 2021 13:47:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 08 Jul 2021 13:47:11 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 08 Jul 2021 13:50:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 13:50:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 08 Jul 2021 14:06:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 08 Jul 2021 14:06:56 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 08 Jul 2021 14:07:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 08 Jul 2021 14:07:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 08 Jul 2021 14:07:28 GMT
STOPSIGNAL SIGWINCH
# Thu, 08 Jul 2021 14:07:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 08 Jul 2021 14:07:45 GMT
WORKDIR /var/www/html
# Thu, 08 Jul 2021 14:07:54 GMT
EXPOSE 80
# Thu, 08 Jul 2021 14:08:02 GMT
CMD ["apache2-foreground"]
# Fri, 09 Jul 2021 09:58:43 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 09 Jul 2021 09:59:09 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 10:04:07 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 10:04:24 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 09 Jul 2021 10:04:36 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 09 Jul 2021 10:05:00 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 09 Jul 2021 10:05:21 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 09 Jul 2021 10:05:38 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 09 Jul 2021 10:05:43 GMT
WORKDIR /var/www/html
# Fri, 09 Jul 2021 10:05:52 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 09 Jul 2021 10:05:58 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 09 Jul 2021 10:09:46 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 10:09:51 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 09 Jul 2021 10:09:56 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 09 Jul 2021 10:10:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bede12a66c305ed12d280c6b7a6022061a73d9568433f643b06ec9893f790c0`  
		Last Modified: Sat, 26 Jun 2021 09:01:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b569ead47e80d494e6f64ea9e5b97bcc6a4d42355effc0aedead32f63c7ba733`  
		Last Modified: Sat, 26 Jun 2021 09:03:27 GMT  
		Size: 82.3 MB (82291015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b0e4b30eb84311f540a9331dfc8db99c35e188d1fc36e8862ed80fd320c431`  
		Last Modified: Sat, 26 Jun 2021 09:01:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0be226e932ae202655cabfbdf039de068fd0668bc10270960d28e04010caf9d`  
		Last Modified: Sat, 26 Jun 2021 09:04:48 GMT  
		Size: 19.8 MB (19818544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a6a8c2dc286478f193e642b39db64063501e03463223f793d17bf4b4d548a4`  
		Last Modified: Sat, 26 Jun 2021 09:04:35 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d8e7e98a0047f2938ddec0785e0b8a93b3b086bfd03f29c6d1a903ec5bfd69`  
		Last Modified: Sat, 26 Jun 2021 09:04:35 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1a8d6de82ac0859d58bcb19b80faafda297f1b8f84fc532cd1a2289a479cf2`  
		Last Modified: Thu, 08 Jul 2021 17:06:32 GMT  
		Size: 11.0 MB (11013069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9427c0f92c377c83e746b5ba2c12a2271c9d53f4cf5732ff71406955a99ed058`  
		Last Modified: Thu, 08 Jul 2021 17:06:28 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b521fd330590d7a5bf99af4900490cee04095a6cdfba3215742e80d63141eb`  
		Last Modified: Thu, 08 Jul 2021 17:06:34 GMT  
		Size: 15.2 MB (15213375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730ba984332076a780ce3fecd78b55371dd059fa9721022bc82b6ea755be9ffe`  
		Last Modified: Thu, 08 Jul 2021 17:06:28 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c2419d3c469b5b8cfc4b79dab60a29514319f99c537d4e10d13250a9a9d74c`  
		Last Modified: Thu, 08 Jul 2021 17:06:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d06ad7743bf2c7189d3a454c5cdb51b25e60c8ea66604f0671f74906045fb`  
		Last Modified: Thu, 08 Jul 2021 17:06:28 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301018d34fc6a234b0e366d7aa89f3be36dc0dee3ef3dad0aaae3bdeb8ba4853`  
		Last Modified: Fri, 09 Jul 2021 10:20:56 GMT  
		Size: 1.5 MB (1468914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e847824585c6356a8334baa5ebebcd8e09d54cf4e46aba6c969c3db8d6481a`  
		Last Modified: Fri, 09 Jul 2021 10:20:56 GMT  
		Size: 5.3 MB (5303359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201edf3ea4da0e418872b0400ea50f4c4338581dcae1e73af7a5d10cd8cd3ba`  
		Last Modified: Fri, 09 Jul 2021 10:20:54 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464166d108ecfd05c23d6f3d0381b263d1220f45b07eae33975095c883b83a90`  
		Last Modified: Fri, 09 Jul 2021 10:20:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df053c63562f3ae71b78532678c43e8f4ee1c605f0e097a8d0a44d003883766`  
		Last Modified: Fri, 09 Jul 2021 10:20:51 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d60a40f6ac943dec4e8fe7ad14e39dd6c1cbff9345249e1774c715ac4d84236`  
		Last Modified: Fri, 09 Jul 2021 10:20:51 GMT  
		Size: 8.3 KB (8308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecda9e620d79386373e1f78545b428d6840ff90afd5ac6da27df09ddc7fe70f7`  
		Last Modified: Fri, 09 Jul 2021 10:21:02 GMT  
		Size: 34.5 MB (34531325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cd6fd3258a6710685c16f3c60002236dca208b92dfd4b3d0f8e34ea1a59964`  
		Last Modified: Fri, 09 Jul 2021 10:20:50 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:latest` - linux; s390x

```console
$ docker pull monica@sha256:fb873bc233cc37d7be94ac2a6220533a8af5e184fb37f5aee83f715628e252db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174142413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0080b9ee26b7fdc1869efb7d9f06cbf584f4946734d6990c84ff4f15deae759`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 00:09:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 26 Jun 2021 00:09:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 26 Jun 2021 00:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 00:10:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 00:10:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 00:13:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 26 Jun 2021 00:13:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 26 Jun 2021 00:14:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 26 Jun 2021 00:14:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 26 Jun 2021 00:14:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 26 Jun 2021 00:14:09 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 00:40:37 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 23:51:14 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 23:51:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 23:51:15 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 23:52:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Jul 2021 23:52:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 23:57:51 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:57:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 23:57:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 23:57:54 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Jul 2021 23:57:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:57:55 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 23:57:55 GMT
EXPOSE 80
# Thu, 01 Jul 2021 23:57:56 GMT
CMD ["apache2-foreground"]
# Fri, 02 Jul 2021 08:19:59 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Fri, 02 Jul 2021 08:20:07 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 08:24:56 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 08:24:59 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Fri, 02 Jul 2021 08:25:00 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Fri, 02 Jul 2021 08:25:03 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Fri, 02 Jul 2021 08:25:05 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Fri, 02 Jul 2021 08:25:07 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Fri, 02 Jul 2021 08:25:08 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 08:25:09 GMT
ENV MONICA_VERSION=v3.1.3
# Fri, 02 Jul 2021 08:25:10 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Fri, 02 Jul 2021 08:26:33 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 08:26:48 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Fri, 02 Jul 2021 08:26:49 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Fri, 02 Jul 2021 08:26:50 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61297595675dd5f94c60485ec6670e0d45420c73a569aebae232822f3805f5f4`  
		Last Modified: Sat, 26 Jun 2021 02:18:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab5f68c432394e6815ad9808418b4300224b46b5898a0f90a1fedbfdf9ca7f`  
		Last Modified: Sat, 26 Jun 2021 02:18:46 GMT  
		Size: 64.7 MB (64710315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def165c1dbb7cd43c8e70e00b2ec5aa53eae70056635c2ff93bdaf25ec061ef`  
		Last Modified: Sat, 26 Jun 2021 02:18:36 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b3e7236868c26c00547364caef50791abcea8d5a62d4fac4ff00f1acf28308`  
		Last Modified: Sat, 26 Jun 2021 02:19:14 GMT  
		Size: 18.5 MB (18525085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae502a4e5daabc91e5f674004c64396c939ee72f05af0b913531fd51c79a37e`  
		Last Modified: Sat, 26 Jun 2021 02:19:11 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c27e0c3d22fb08edda2488324e9cbcd02f8ff31f5bad766bdd1470e2ea7048`  
		Last Modified: Sat, 26 Jun 2021 02:19:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771cff9dbb87665b7991a8687f0a57051d6344a696a99b2a46a03da9cdc076f4`  
		Last Modified: Fri, 02 Jul 2021 01:15:32 GMT  
		Size: 11.0 MB (11011392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a168beeba80eca90b5acdbd0560bb8996b287ea402640894e3048062f3c14955`  
		Last Modified: Fri, 02 Jul 2021 01:15:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbcefbef5bba54401f4bfa1311e5448113a2adf2667eabdb04f716e2b15868f`  
		Last Modified: Fri, 02 Jul 2021 01:15:20 GMT  
		Size: 13.4 MB (13361980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b0dbc32ca5304feef35aa8e81886ba42fb79b9c939e4abb65188ba0cc05f1`  
		Last Modified: Fri, 02 Jul 2021 01:15:16 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dc45940630855229af4a807a42cfc7adf18a769274faad981bf937f08f0435`  
		Last Modified: Fri, 02 Jul 2021 01:15:15 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb1724e28adaa2b106f824a7bda83e5782c6797e8f80c781a4c9ed2c0692544`  
		Last Modified: Fri, 02 Jul 2021 01:15:16 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffe29390ab67ca543107e05379904dcece8f116a144bdf2ae8d1ad06b360acf`  
		Last Modified: Fri, 02 Jul 2021 08:35:58 GMT  
		Size: 1.3 MB (1316452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0f034ad71b71c130ca8ebc5896e93d83f9d7bf43e3c736b69a3ef2f11da66`  
		Last Modified: Fri, 02 Jul 2021 08:35:46 GMT  
		Size: 4.9 MB (4911136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356f5f097811a556aee289a55968b1db9c9c9adb0d6c3cd0e4d5037d20bd2c14`  
		Last Modified: Fri, 02 Jul 2021 08:35:46 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f87064d7ce16258f89916195acd0452c15b2451d6b0e170a4932551f3a6777`  
		Last Modified: Fri, 02 Jul 2021 08:35:33 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96dbdfdfc843c17ac48a52620517c216aada159098c01a8920f69f9c8a1387b`  
		Last Modified: Fri, 02 Jul 2021 08:35:37 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213f627c55aeef92324c74c84b4ec2c9643a1015e1fe8e22ddb24777907c5968`  
		Last Modified: Fri, 02 Jul 2021 08:35:33 GMT  
		Size: 8.3 KB (8310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb59d33554a0c102512bef5191e4f0e77cf8b7c989aeb6162e395073e0c96b9`  
		Last Modified: Fri, 02 Jul 2021 08:35:42 GMT  
		Size: 34.5 MB (34528481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16b944ab876e3af7dd3a168be52ff56265507a8a0c56733885bd39514c8f78`  
		Last Modified: Fri, 02 Jul 2021 08:35:37 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
