## `monica:apache`

```console
$ docker pull monica@sha256:df72e4a5cb3d10ba6a6d2715144226b3128d4c5c313ebe80ded64734c81143dc
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

### `monica:apache` - linux; amd64

```console
$ docker pull monica@sha256:bfc968a2e9570d7dc2c8d3a63504d4caab410d84501cce5d9428192c690ca58d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.7 MB (208720562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3438d428af762273cbef40f1a2e63bafa93f2591cbb142d588053053bb6bdfe`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:17:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 16:17:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 16:18:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:18:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 16:18:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 16:27:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 16:27:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 16:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 16:27:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 16:27:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 16:27:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 16:27:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 16:27:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 17:28:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 17:28:11 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 17:28:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 17:28:11 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 17:29:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 17:29:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 17:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 17:34:33 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 17:34:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 17:34:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 17:34:35 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 17:34:35 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 17:34:35 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 17:34:35 GMT
EXPOSE 80
# Wed, 26 Jan 2022 17:34:35 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 22:21:55 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 22:21:59 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 22:23:36 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 22:23:36 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 22:23:37 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 22:23:37 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 22:23:38 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 22:23:39 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 22:23:39 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 20:19:40 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 20:19:40 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 20:20:01 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 20:20:02 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 20:20:02 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 20:20:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1ad84cf10194e2130f05599fcf95721234f2e72aeb9b2c7341719a0a736e41`  
		Last Modified: Wed, 26 Jan 2022 19:09:25 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c937dadeb7e3e4f156ed8bf156bc07d09c18d255475f602ae6e7c94ad0efc5`  
		Last Modified: Wed, 26 Jan 2022 19:09:41 GMT  
		Size: 91.6 MB (91604421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2f1dc96e597c811b3e8c3d0332b71dd64989ff1f972ffbc477edbc479062f7`  
		Last Modified: Wed, 26 Jan 2022 19:09:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c3f82c39d441d1987e11925e9cda5f1f9aba52ad1d3c341e9c4e7f1efe42c0`  
		Last Modified: Wed, 26 Jan 2022 19:10:41 GMT  
		Size: 19.2 MB (19245845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc6462bd8e4fa3a65fff11c70bd270c8f59545a093c6d3124a426036e3880a`  
		Last Modified: Wed, 26 Jan 2022 19:10:37 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c670d99116c951149bb76403284f5a63b99c3788e7088cf4278364322ba777ac`  
		Last Modified: Wed, 26 Jan 2022 19:10:37 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268554d6fe96ca6d3f15fe8bb8d8b9535f72fa692ce8d3b6e52b97c8dbc2ac32`  
		Last Modified: Wed, 26 Jan 2022 19:15:12 GMT  
		Size: 11.1 MB (11104734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c29fa0d4492a1d1c6e04e45856f0c3138e2df424d856ac0540c8716486feb5d`  
		Last Modified: Wed, 26 Jan 2022 19:15:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e23c50a2590dc3a72b6cf20068988bc675d282c34ed233391a2d4aa1798b65`  
		Last Modified: Wed, 26 Jan 2022 19:15:11 GMT  
		Size: 14.6 MB (14554487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ac13c96fc2ac3adcf62d16c8506166abca851d2a86d119a72608ff097c8a74`  
		Last Modified: Wed, 26 Jan 2022 19:15:09 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60a3e623949882b978a6a7c24c0dcb67b37e46f8c74b0c8ba43824671f6677c`  
		Last Modified: Wed, 26 Jan 2022 19:15:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac5dd67fd596bcb535704d416ede31d95ef5fb8a5d2cd7cb3ac2f0f7f6d6542`  
		Last Modified: Wed, 26 Jan 2022 19:15:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00684d043a219a18f920b95d774fc90c62ffc5cdafd1a16ba72e755a5dbc6d7`  
		Last Modified: Thu, 27 Jan 2022 22:29:16 GMT  
		Size: 1.4 MB (1385540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c736169a5a2e6e1d67a29e335c4309107cc98572ef753fd6ee2136d22279c3e`  
		Last Modified: Thu, 27 Jan 2022 22:29:16 GMT  
		Size: 4.1 MB (4102629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e80206a309532768386008b652934ac38dda74956d24119904c67f6dece98`  
		Last Modified: Thu, 27 Jan 2022 22:29:15 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b418facac57f9c5583e50f2b34cb912a3599ed89fc6b22fafb81b2700ba9f902`  
		Last Modified: Thu, 27 Jan 2022 22:29:12 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977900ccc9ef76c1eed1d732c5dda871591fccdd4ab6208c4f4c89683b3b00e1`  
		Last Modified: Thu, 27 Jan 2022 22:29:12 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb99ec632944644266f8fec44684319dad5cd7499ac89546344ec4671cd4f2d1`  
		Last Modified: Thu, 27 Jan 2022 22:29:10 GMT  
		Size: 8.3 KB (8309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2abd9ce60795296c38a6c7990866b019c7ae2c4b870e6cc93955057c305cff`  
		Last Modified: Tue, 08 Feb 2022 20:21:26 GMT  
		Size: 35.3 MB (35339461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af15e87d72f96cc8f8833e6f6d9a6e6aea82e400fa56dd9b87491f4f965b131`  
		Last Modified: Tue, 08 Feb 2022 20:21:18 GMT  
		Size: 2.0 KB (2025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; arm variant v5

```console
$ docker pull monica@sha256:362585751353a801ff539f09621521e160cbcbe1cc01332a33e46eb9fea2c128
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (186019464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05409877c0f12d1d2a1370e71a4cd1c17560b0ca1e3cae4b413aba45b365e93a`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:37:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 08:37:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 08:39:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:39:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 08:39:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 08:47:33 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 08:47:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 08:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 08:48:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 08:48:05 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 08:48:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 08:48:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 08:48:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 09:38:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 09:38:31 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 09:38:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 09:38:32 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 09:39:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 09:39:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:44:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 09:44:15 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:44:16 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 09:44:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 09:44:17 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 09:44:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:44:18 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 09:44:19 GMT
EXPOSE 80
# Wed, 26 Jan 2022 09:44:19 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 10:37:12 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 10:37:23 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:41:49 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:41:50 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 10:41:51 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 10:41:52 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 10:41:54 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 10:41:56 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 10:41:56 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 19:48:38 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 19:48:38 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 19:50:04 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 19:50:06 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 19:50:07 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 19:50:07 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb1b62cf85a0cdb10aa730c066ded667f1569b0ecedb00d54533a75b791ad73`  
		Last Modified: Wed, 26 Jan 2022 11:53:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86f49ee6f19a2b2b1c661de4521936eedeab6cc9330a32e04fb3777e60ea81`  
		Last Modified: Wed, 26 Jan 2022 11:54:20 GMT  
		Size: 73.7 MB (73684264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a675ef1269333a12b19d1dd74f886d890895c70a6d6a0da508ce4f474cb32032`  
		Last Modified: Wed, 26 Jan 2022 11:53:29 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed785b1997759bec54442ac3289fb76160900fbd847882743c84adb52070092`  
		Last Modified: Wed, 26 Jan 2022 11:55:43 GMT  
		Size: 18.5 MB (18534324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fe5aa6ffb62e35d7d17981c75d6f3f7fcc5c89f293f7c066d29d9daf569d5f`  
		Last Modified: Wed, 26 Jan 2022 11:55:32 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a171fa46e8edf4c56b1ca7cbb585afc2a69a3e92f9c6066454da19c4333103`  
		Last Modified: Wed, 26 Jan 2022 11:55:32 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b139781aa1eae25ef5665f9f1594d0657b2ee759b4e91fa22597a394610852`  
		Last Modified: Wed, 26 Jan 2022 12:02:22 GMT  
		Size: 11.1 MB (11103328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8770739f72f64b9b1679a88d001b0bf9f8ea01a3fe0941063868b0fa044917`  
		Last Modified: Wed, 26 Jan 2022 12:02:17 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097fe667b8252950ee2e62f5203c7e194497717d8932ef579598ede6a57d744`  
		Last Modified: Wed, 26 Jan 2022 12:02:28 GMT  
		Size: 13.3 MB (13266148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c65d77bfc35abcfcf0e3dca4fc1b287b46b7263e4e59401ab892c3e692c4b0e`  
		Last Modified: Wed, 26 Jan 2022 12:02:18 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc69ca16fd0b0f1ad132545c7a2fefef9d49f250b78cd069c05e079ce9a4ee1`  
		Last Modified: Wed, 26 Jan 2022 12:02:17 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed4ef46119c5a62fc4b7bb5d7fec2ad0d3c4f98f76610809d2466d55a2bd15`  
		Last Modified: Wed, 26 Jan 2022 12:02:17 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f886519964e729bddfff1ae93aa8f75f0d3d52a840a06aa7849dcb5fede29b`  
		Last Modified: Thu, 27 Jan 2022 10:50:25 GMT  
		Size: 1.3 MB (1340445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac269184a9e0caee99c16afca5d4efaa825e3767878c2d0b64dac5c8a88d06dc`  
		Last Modified: Thu, 27 Jan 2022 10:50:28 GMT  
		Size: 3.8 MB (3826514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e0c3cbfae59aebfc7e96c8526e4026db6d2aca591390bd2762b3fc4dd88c72`  
		Last Modified: Thu, 27 Jan 2022 10:50:25 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a928ed2d4c1a71a5955ebe080de1c77bb997056ef534e9e719535673accfb`  
		Last Modified: Thu, 27 Jan 2022 10:50:23 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c2c346af4cd457b6c3e273353d766f5cf725c93e4d3929e16a6d36f336da87`  
		Last Modified: Thu, 27 Jan 2022 10:50:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc1518795498e5afedd6eaccfb080264642768178f787c0faaf64fd0414647f`  
		Last Modified: Thu, 27 Jan 2022 10:50:23 GMT  
		Size: 8.3 KB (8309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ce2e39bf2845bd931f5f980d9e8851e07f97cf3c3f87761c6d39aca2bd0bc8`  
		Last Modified: Tue, 08 Feb 2022 19:53:21 GMT  
		Size: 35.3 MB (35337596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8224daa75dfaa5fb782603666062cb21d678e65256f194da56a83e9beaad6766`  
		Last Modified: Tue, 08 Feb 2022 19:52:35 GMT  
		Size: 2.0 KB (2025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; arm variant v7

```console
$ docker pull monica@sha256:da483eb40272cb9c8a09e05e8bb5f9b074991f81746619544aa023b9e8aa3d82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177790840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f616d34321329368a4a9f09e17ec5cc1b5687b4a3602c954f20e50caf62015`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:27:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 03:27:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:28:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 03:28:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 03:34:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 03:34:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 03:34:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 03:34:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 03:34:50 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 03:34:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:34:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:34:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 04:20:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 04:20:02 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 04:20:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 04:20:03 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 04:20:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 04:20:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 04:25:30 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:25:32 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 04:25:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 04:25:32 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 04:25:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:25:34 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 04:25:34 GMT
EXPOSE 80
# Wed, 26 Jan 2022 04:25:34 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 13:42:21 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 13:42:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 13:46:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 13:46:42 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 13:46:43 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 13:46:45 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 13:46:46 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 13:46:48 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 13:46:48 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 19:57:58 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 19:57:58 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 19:58:56 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 19:58:59 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 19:58:59 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 19:59:00 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc9a20cd165cc34bba0c0bab277b6fbf5b727eb38c1b902e577a6f91bdd4980`  
		Last Modified: Wed, 26 Jan 2022 06:36:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e7063615e6e2b8aee21d5be918dc091b1ed4a0792197b96205dcb419f7115b`  
		Last Modified: Wed, 26 Jan 2022 06:37:29 GMT  
		Size: 69.3 MB (69315436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed49ea1bd88a9bbfafb4155619fe90383f2f713205f8bb810a75902408f0d1de`  
		Last Modified: Wed, 26 Jan 2022 06:36:46 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22e82e5b1bd524afe0d900329ad1f0e1dcb427a3ff6c5e37accd58d6780ff1b`  
		Last Modified: Wed, 26 Jan 2022 08:19:17 GMT  
		Size: 18.0 MB (17993026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65de72f6bd09c20a231d7a2cf455eed5327c561f4b52e2fb20a6ca99b7c75e`  
		Last Modified: Wed, 26 Jan 2022 08:19:07 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292027d35ecb573bb5871e1fe35b5fdde0c782984668e9658d3e3936dda27b7`  
		Last Modified: Wed, 26 Jan 2022 08:19:07 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9484ea50deaa914efcb8febcbc414a741823e3747c3a7370404242e7ed13d0f1`  
		Last Modified: Wed, 26 Jan 2022 08:26:43 GMT  
		Size: 11.1 MB (11103394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251837a37ce22cb7d139dc1ab84d9306655bb0ef72d69da1f9728046c6fb4a0b`  
		Last Modified: Wed, 26 Jan 2022 08:26:37 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bec6bd95596de62d49944ca8bf483109678a5d4740774c34877128913f83c0`  
		Last Modified: Wed, 26 Jan 2022 08:26:46 GMT  
		Size: 12.6 MB (12560433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b625bcf3a956d50cd34dcc61b8ad962842731dcbe750e25f393b1da5369e20`  
		Last Modified: Wed, 26 Jan 2022 08:26:37 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2f0dd85a955d0873962fe6124bd5e689bdeb4b2c04a3266e2f35e3f197f783`  
		Last Modified: Wed, 26 Jan 2022 08:26:37 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8d61bec84a06663481ce899d0002bbd8f48542d7f6d3f86512c942c8752f6e`  
		Last Modified: Wed, 26 Jan 2022 08:26:37 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5ddbc8d501b38bc8e35240dae3075f6ab3c378564165ee91f4a7a24120577`  
		Last Modified: Thu, 27 Jan 2022 13:56:22 GMT  
		Size: 1.2 MB (1220283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c3b9c616e101b4e5713c759c93fa8b609b274367631b562e0bddaccd639918`  
		Last Modified: Thu, 27 Jan 2022 13:56:24 GMT  
		Size: 3.7 MB (3678494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70788c92a56f07f37e1dc5d947454e102208fc270cee1194a991edebd48a5e3`  
		Last Modified: Thu, 27 Jan 2022 13:56:21 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee72b02e1215e26a81c7c1df94c95cb878cc63d3d3802a0ab9bfa935cec9d82`  
		Last Modified: Thu, 27 Jan 2022 13:56:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d15905a84eae405c0557e9403b2af7a613a05ff6305d677e815dd2b4921cf0`  
		Last Modified: Thu, 27 Jan 2022 13:56:19 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758053e7feb5e3c81a084ff58910e2fe2e50ed592b8e784cc4cdc4ba43ba85d5`  
		Last Modified: Thu, 27 Jan 2022 13:56:20 GMT  
		Size: 8.3 KB (8302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf7b74be686a280dbc9420e49b68659a21276b13ea13ea779aa2ae3d57c7088`  
		Last Modified: Tue, 08 Feb 2022 20:03:42 GMT  
		Size: 35.3 MB (35337629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573a7ec394800b1a22219fc797bc93917a49ee9c5bdc24bb8955896c9f8de364`  
		Last Modified: Tue, 08 Feb 2022 20:02:58 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; arm64 variant v8

```console
$ docker pull monica@sha256:6e262248c502db354b17851b21c817c4614997140ee071ad17d2eb5cf5988691
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.8 MB (200836105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b87e23524126fafa03f444e5210767492571b54501995bf17d943bdaadb41d`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 11:17:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 11:17:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 11:17:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 11:17:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 11:17:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 11:22:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 11:22:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 11:22:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 11:22:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 11:22:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 11:22:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 11:22:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 11:22:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 11:57:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 11:57:31 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 11:57:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 11:57:33 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 11:58:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 11:58:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 12:00:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 12:00:43 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 12:00:43 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 12:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 12:00:45 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 12:00:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 12:00:47 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 12:00:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 12:00:49 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 04:21:39 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 04:21:42 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:23:09 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:23:10 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 04:23:11 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 04:23:13 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 04:23:13 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 04:23:14 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 04:23:15 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 19:41:42 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 19:41:43 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 19:42:04 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 19:42:06 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 19:42:07 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 19:42:08 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ef0b26fc2c1475131c5f8e1123b50ad54fefa37503c1b752e1980bb4680a0e`  
		Last Modified: Wed, 26 Jan 2022 13:08:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d4d2813bc9c42491f9d0e965c03abb0de354bc63e51ed09a38abd4b762bab`  
		Last Modified: Wed, 26 Jan 2022 13:08:49 GMT  
		Size: 86.9 MB (86920605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787dfbf2c706b3ee4bc754f4ea1a11d0a884be30f3f653ad76b9dc923e34f52c`  
		Last Modified: Wed, 26 Jan 2022 13:08:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095f089a21c235c04169396d4d7608e7f28e82b5b1dc25cd8872d7800755ebf0`  
		Last Modified: Wed, 26 Jan 2022 13:09:50 GMT  
		Size: 18.9 MB (18943794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11ff030293344021955561671a15be42d45744c89d32bf65845a99c64cd1c4d`  
		Last Modified: Wed, 26 Jan 2022 13:09:47 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897c0c6da4ac81a2ec7f8edb6a55395db524daf285f38fd862721e8e5169dd3`  
		Last Modified: Wed, 26 Jan 2022 13:09:47 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed34cb1130a59534120cac67a9daf5af4508f5b91b8224dbcaba1213b4faf2c`  
		Last Modified: Wed, 26 Jan 2022 13:14:31 GMT  
		Size: 10.9 MB (10889220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea3f9b85722b721c4c5585da7ac1406d0d001018f368f36b9ce3c84481ded75`  
		Last Modified: Wed, 26 Jan 2022 13:14:27 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b3aaec12db371b9a22c7d972bfb38cd1a671d53a7ca501a041dfd7c6e0e9d`  
		Last Modified: Wed, 26 Jan 2022 13:14:30 GMT  
		Size: 13.9 MB (13944632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09bfa1c045d0f5b6c1098921a1c74aa891539f630144e6b055b616e25755551`  
		Last Modified: Wed, 26 Jan 2022 13:14:28 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b6580cdd47fe53a5b47e0a54b23414e46c293208d6bda15fbea5b204397a9e`  
		Last Modified: Wed, 26 Jan 2022 13:14:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7ab8dd3008354cc4ab51a7c196f61a341669f76f84e69b9850d9c6ab4d58b0`  
		Last Modified: Wed, 26 Jan 2022 13:14:27 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345bb512e2c257d3a1c8c0d6c5a101626967313d7ad9a70f279f1babbaa3c54`  
		Last Modified: Thu, 27 Jan 2022 04:26:39 GMT  
		Size: 1.1 MB (1114039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a722173ddd28cf08df97bcadac5288d9af726f9adc54d40674adfee930721`  
		Last Modified: Thu, 27 Jan 2022 04:26:40 GMT  
		Size: 3.8 MB (3827752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c32d1240f7960fce743226b381c748d695194b02d4192ac88467679f1866fd`  
		Last Modified: Thu, 27 Jan 2022 04:26:39 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f79161cfddf126949448d0cd76b5965004bb8dc3ecd9dec8a5942dfa6fdf509`  
		Last Modified: Thu, 27 Jan 2022 04:26:36 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aad461dc4ba25f9061ae0c73a3711dffc33f31972c8fc4340b2cf1193d3c17`  
		Last Modified: Thu, 27 Jan 2022 04:26:37 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beffcbb16c287629a040cbcfd855dead85f0c47da248d0b7311e8cfedd900161`  
		Last Modified: Thu, 27 Jan 2022 04:26:37 GMT  
		Size: 8.3 KB (8303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3bef7eb15744d864e5fe23c095accaea1942116a821673bebdc302aeb717bc`  
		Last Modified: Tue, 08 Feb 2022 19:43:52 GMT  
		Size: 35.1 MB (35122254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dcb681c9fd1ce2867efdfdd949c22384e4c4258b027ac511260d4c8aa9cd25`  
		Last Modified: Tue, 08 Feb 2022 19:43:43 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; 386

```console
$ docker pull monica@sha256:8326cbd1f4b2a4397188c075a381a061f8bff541fd987a8ba85453f301dd5570
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.7 MB (211658478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f7b2adc4d597167cd72070e0c036d3b82bd2967eb40c24f9f4cd76640b71bf`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 14:14:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 14:14:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 14:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 14:14:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 14:14:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 14:25:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 14:25:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 14:25:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 14:25:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 14:25:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 14:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 14:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 14:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 15:13:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 15:13:30 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 15:13:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 15:13:30 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 15:14:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 15:14:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 15:19:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 15:19:36 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 15:19:37 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 15:19:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 15:19:38 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 15:19:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 15:19:38 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 15:19:38 GMT
EXPOSE 80
# Wed, 26 Jan 2022 15:19:38 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 08:58:55 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 08:59:05 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 09:03:44 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 09:03:46 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 09:03:47 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 09:03:49 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 09:03:51 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 09:03:53 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 09:03:54 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 19:38:40 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 19:38:41 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 19:39:12 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 19:39:14 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 19:39:15 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 19:39:15 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682cda5f75565c6258e6085d20fe17517c28479908d154cff4821d10d2740372`  
		Last Modified: Wed, 26 Jan 2022 17:29:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42ce37ddcafbb43a3972e8a050e538f5b29f470467f9583b9ac7f89c788b90b`  
		Last Modified: Wed, 26 Jan 2022 17:29:59 GMT  
		Size: 92.7 MB (92716286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6499046669fefe00a8c534270eb6528ba2251f36f2953b662450bab9b83a144`  
		Last Modified: Wed, 26 Jan 2022 17:29:35 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151a697a8b09279653f3aeb4c6a9a0a55e45801520e2b655363b8a6e004078c4`  
		Last Modified: Wed, 26 Jan 2022 17:31:38 GMT  
		Size: 19.7 MB (19714643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30b77c2d08d5d90daa6a2c60b0755fea3d43bb3496f54dac08e4376a1b591`  
		Last Modified: Wed, 26 Jan 2022 17:31:28 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e18c6d7ab37bbef7714a6a22e778c1f22b9c57d7ddb71f5b80789f252b2a7b`  
		Last Modified: Wed, 26 Jan 2022 17:31:28 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68b914740cc73840790a6bceef799300bbe67fbe3e949b74b9dbc7dfa6fd666`  
		Last Modified: Wed, 26 Jan 2022 17:38:22 GMT  
		Size: 11.1 MB (11104017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010554e54c66e746fab42ecdc6a7c54d39ae92c5024df46816352e420517514`  
		Last Modified: Wed, 26 Jan 2022 17:38:17 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e656ee6795b65720492af3f9a463f2f132abab7b56d80451f0a609dba5aab87d`  
		Last Modified: Wed, 26 Jan 2022 17:38:25 GMT  
		Size: 14.8 MB (14842025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4d8af2fcaf835f189f92baf067d91c315c027d1ad12fe2d1b9361798b327f`  
		Last Modified: Wed, 26 Jan 2022 17:38:18 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bd914303c39a9592f42e197e812163d3271a5ac28af3a92941fec7502c6912`  
		Last Modified: Wed, 26 Jan 2022 17:38:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f012cfd856255d4493ed45aa614a53cbbfe6ee36c16484d7470af201f5bf305`  
		Last Modified: Wed, 26 Jan 2022 17:38:18 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a143b96049fdb67f7c66257fefb7d73d3d5b6b989b77b3acc06f3be6a3447`  
		Last Modified: Thu, 27 Jan 2022 09:17:59 GMT  
		Size: 1.4 MB (1397611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3d0d60c83e38f76638ac22e456edc63910b6d508fa5377715e57a727c5743e`  
		Last Modified: Thu, 27 Jan 2022 09:18:00 GMT  
		Size: 4.2 MB (4150947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a0c729f79a814f6b4ba1c6a6d9a8af7f6dcdeff040a34a8c468114580d892d`  
		Last Modified: Thu, 27 Jan 2022 09:17:58 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32011452366a896cbba40907bfc750e30ab50ab0e35ccd88a74ccf08242bb209`  
		Last Modified: Thu, 27 Jan 2022 09:17:55 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e90309070246526300b94aaba6d3c0175c678216ca813bb044f0b83e27d1de5`  
		Last Modified: Thu, 27 Jan 2022 09:17:55 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2044a4779c6d45717948c372fe295e03cc796d1fe866d1dfd71ed04ea471663`  
		Last Modified: Thu, 27 Jan 2022 09:17:55 GMT  
		Size: 8.3 KB (8309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5218b61164475a85b33ccbe6cadcaa2b7c1f0aea3e25345a6c12ba69cef970`  
		Last Modified: Tue, 08 Feb 2022 19:41:21 GMT  
		Size: 35.3 MB (35338346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090956125c63ecb37205affca0791aab366309ced13274888b7cf6bb5b4d7f0b`  
		Last Modified: Tue, 08 Feb 2022 19:41:07 GMT  
		Size: 2.0 KB (2030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; mips64le

```console
$ docker pull monica@sha256:ecf2797138ea25122b0258bc464113aea590a9b759d21cbdc1570210a9ccd77e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.2 MB (186200195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d4be13dd75de308f93996cb6beda496b81d66a6b8d209689f41f6d78397990`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 12:25:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 12:25:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 12:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 12:26:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 12:26:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 12:39:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 12:39:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 12:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 12:40:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 12:40:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 12:40:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 12:40:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 12:40:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 14:26:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 14:26:44 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 14:26:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 14:26:45 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 14:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 14:27:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 14:39:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 14:39:49 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 14:39:51 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 14:39:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 14:39:52 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 14:39:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 14:39:53 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 14:39:53 GMT
EXPOSE 80
# Wed, 26 Jan 2022 14:39:53 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 19:07:32 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 19:07:44 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 19:13:01 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 19:13:03 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 19:13:03 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 19:13:05 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 19:13:08 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 19:13:10 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 19:13:10 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 20:07:32 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 20:07:33 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 20:09:10 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 20:09:13 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 20:09:13 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 20:09:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191e94952e609ddcd788e8b84a0c6e52cb8d70b72fc1ecdf09671b8b97c8ae88`  
		Last Modified: Wed, 26 Jan 2022 18:35:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a20e2dcd1bfa855631549301d1b32d7018e8471fd65e4172a12ade76c981de`  
		Last Modified: Wed, 26 Jan 2022 18:36:05 GMT  
		Size: 72.0 MB (72013491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1dc62c31c14b2b41b143b779c94633e090e9b781c749c205f379a4a404e4ef`  
		Last Modified: Wed, 26 Jan 2022 18:35:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa51c2bcf42e9b3ec702bec52c0b36b70bf365f6fa4fa1908b7261a112c1dd2c`  
		Last Modified: Wed, 26 Jan 2022 18:37:13 GMT  
		Size: 19.1 MB (19145545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d0161a75ed794ace7404c46755af243b6f1b5f40277f8e34adb69a84b23cce`  
		Last Modified: Wed, 26 Jan 2022 18:36:59 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7bc9abc811886cd43346551116f915ee9670ac9db88c80df0a08c457f94545`  
		Last Modified: Wed, 26 Jan 2022 18:36:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dac8444db2c0711b15018036608098b8fd3fe656195fcf422a84b6268cc848`  
		Last Modified: Wed, 26 Jan 2022 18:43:32 GMT  
		Size: 11.1 MB (11102680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f338fe91af8a410c7bc27a0ebf869f61011a4f626c058abc3d0f83599edb61`  
		Last Modified: Wed, 26 Jan 2022 18:43:25 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df3157953211247badfc6c2467403fab6446d013cc142b48c3ace05f9770f2`  
		Last Modified: Wed, 26 Jan 2022 18:43:37 GMT  
		Size: 13.5 MB (13488810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9473e1b259d0892412bb02e7b37835c78964e5a0bc6b97269bcd877f36532ea4`  
		Last Modified: Wed, 26 Jan 2022 18:43:25 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a7a670507715bd33428684fccb029434b699a35d2c1c44464d7a2c88adc880`  
		Last Modified: Wed, 26 Jan 2022 18:43:25 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e180f0e671d1ae0ec4185af9acfc7b2dea1361467bb5b3cedb7b1ad09f5cc3f`  
		Last Modified: Wed, 26 Jan 2022 18:43:25 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227c42615a796a6f960a75ea70c15ba60f9e8e861c578c121686ff1819e9a320`  
		Last Modified: Thu, 27 Jan 2022 19:21:39 GMT  
		Size: 1.5 MB (1460224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f54613b06780c3aa3c6c8ad5be1b04c9a5616bb2b5eb19b6395d1873fb13f1`  
		Last Modified: Thu, 27 Jan 2022 19:21:41 GMT  
		Size: 4.0 MB (4003113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904fc7bde2b255859d20ab686d4b28302ea6e90144bdfc5a27ab8ff86d9c27d0`  
		Last Modified: Thu, 27 Jan 2022 19:21:37 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6362d7ac23f722d00d5b1821dd7a21285c055858ef98f3956a291d74f5ed9b1f`  
		Last Modified: Thu, 27 Jan 2022 19:21:35 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3498c57de862bcbf78d6f7afbea3d3ecf1d73a58b6eeafcde902e7b4f60413af`  
		Last Modified: Thu, 27 Jan 2022 19:21:35 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aea8097a79ceb730e7c9b389a0b0f31b88fdbf40ae175a8edf2c36bcb47894`  
		Last Modified: Thu, 27 Jan 2022 19:21:35 GMT  
		Size: 8.3 KB (8309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0189110f2438f478146a755f2ce6bf144a170036c187463ac3c2b95d6d6cb246`  
		Last Modified: Tue, 08 Feb 2022 20:12:09 GMT  
		Size: 35.3 MB (35336427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2cf35a46b855e226bffd7bef74ae50d595de3405c22f48e1fa3c936c53c20f`  
		Last Modified: Tue, 08 Feb 2022 20:11:27 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; ppc64le

```console
$ docker pull monica@sha256:f9e65b297a29d414ebcecfd542748cdea9af1d31865a27286f9fac0c4d425d06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.0 MB (209958471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7066e298d4600d33b3a0f642463f9d6f6ed9bf931e872f8ded501587383a7342`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:29:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 10:29:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 10:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 10:31:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 10:31:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 10:40:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 10:40:14 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 10:41:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 10:41:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 10:41:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 10:41:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 10:41:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 10:41:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 11:37:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 11:37:33 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 11:37:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 11:37:40 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 11:39:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 11:39:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:44:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 11:44:50 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:44:55 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 11:44:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 11:45:00 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 11:45:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:45:03 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 11:45:05 GMT
EXPOSE 80
# Wed, 26 Jan 2022 11:45:10 GMT
CMD ["apache2-foreground"]
# Thu, 27 Jan 2022 12:49:08 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Thu, 27 Jan 2022 12:49:21 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 12:52:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 12:52:11 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Thu, 27 Jan 2022 12:52:14 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Thu, 27 Jan 2022 12:52:18 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Thu, 27 Jan 2022 12:52:24 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Thu, 27 Jan 2022 12:52:30 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Thu, 27 Jan 2022 12:52:33 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 20:17:41 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 20:17:45 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 20:22:47 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 20:22:57 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 20:23:01 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 20:23:06 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6353566d57126497241a2d1359b8e40a4aa82b31a4fb89b70b71f25028296b7d`  
		Last Modified: Wed, 26 Jan 2022 13:46:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1c3a5c5a3593cebdd72b812ae7ebe3522a05b2d5522abf096556c638af718`  
		Last Modified: Wed, 26 Jan 2022 13:47:18 GMT  
		Size: 86.6 MB (86624458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824b5fa25d786f0ce5c69716c3b8b6ed693840142dbc489273cfd54b9bf7cd3`  
		Last Modified: Wed, 26 Jan 2022 13:46:29 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de019d08f1c17354d8643f0d49cdb41e9b7e26614ba5a7436b782ea079171078`  
		Last Modified: Wed, 26 Jan 2022 13:48:35 GMT  
		Size: 20.5 MB (20451239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3fedf8071a108e2c69f4f313a0851b4de8cf56294204dcd4a0600b599ebef5`  
		Last Modified: Wed, 26 Jan 2022 13:48:24 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b34bae6208b08ced06055ea40bc35cd69a6258050e1fa7a2f84b88e95f5b16`  
		Last Modified: Wed, 26 Jan 2022 13:48:23 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551d339d0c9fc85e328fd712d50bdd1fe3918e961f832669c569cdfb99ac3c41`  
		Last Modified: Wed, 26 Jan 2022 13:55:33 GMT  
		Size: 11.1 MB (11105055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ffd966b43add2c05e2cb311e8caffd3051ea56bf42ebf5611720c98d4bd665`  
		Last Modified: Wed, 26 Jan 2022 13:55:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23234abac590e7346f900d6f4902648b23cf56ce1850492e013b443230e498`  
		Last Modified: Wed, 26 Jan 2022 13:55:38 GMT  
		Size: 15.3 MB (15250350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83896cbd86b00bb1e41a1b13be75296264705ae17ea7ca2d8831f51197eba60`  
		Last Modified: Wed, 26 Jan 2022 13:55:28 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa4e525ac3eb21fa21ca2bc3bc5c274d6ac30599ee43c85274bd535ca0fdbe9`  
		Last Modified: Wed, 26 Jan 2022 13:55:29 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5c5c79a49b3bbec94dbda672f26a06afa97dc7942f0d07b78438047d996773`  
		Last Modified: Wed, 26 Jan 2022 13:55:28 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcdb9d4662a376612f8e0e54be27d95e10daedcf18b4421350fe79d080e5035`  
		Last Modified: Thu, 27 Jan 2022 13:00:03 GMT  
		Size: 1.5 MB (1507699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4930066208c2c7c8938625578f422b2052a3ad550c194a8d9dfefc44dea3732d`  
		Last Modified: Thu, 27 Jan 2022 13:00:05 GMT  
		Size: 4.4 MB (4388489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ce1bd39d1f2cfa620225063601ff40aaf7f50b1aa3072ac66b185362bfc0f7`  
		Last Modified: Thu, 27 Jan 2022 13:00:02 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5370b218180a3e7a9a6b0bbc42d2e7ad461fbf7495eb05ed36be05488749f5e`  
		Last Modified: Thu, 27 Jan 2022 12:59:58 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e55988938c1743c1904d639d8d6cdc33c53e4c45c72102cdb82b58674fb5134`  
		Last Modified: Thu, 27 Jan 2022 12:59:59 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81157c4d213a28b9afe171d57a51d9a75a1e7b9d2832b850896690dc757580ef`  
		Last Modified: Thu, 27 Jan 2022 12:59:59 GMT  
		Size: 8.3 KB (8308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e01a024211d9aa45e99df2f4c331f079f0fc544c268de2ba3575e2d07bd1909`  
		Last Modified: Tue, 08 Feb 2022 20:29:50 GMT  
		Size: 35.3 MB (35340925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf47c9e847a92c15229a1835f4581e4e3afe5e291a168e6779c419fe94a47ad`  
		Last Modified: Tue, 08 Feb 2022 20:29:36 GMT  
		Size: 2.0 KB (2031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:apache` - linux; s390x

```console
$ docker pull monica@sha256:a60e95838b7de941092d14a1cbe1cde0d0d8c14c2fb6d4392cd8cfb9fdf73ae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.6 MB (185582811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57958956d2e77a66270f5a77a53e0873e2f0bdc649f5ccdd3efb21cdc749eefe`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:50:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 03:50:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 03:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:50:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 03:50:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 03:53:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 03:53:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 03:54:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 03:54:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 03:54:05 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 03:54:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:54:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:54:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 04:16:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 04:16:49 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 04:16:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 04:16:49 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 04:17:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 04:17:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:19:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 04:19:13 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:19:14 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 04:19:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 04:19:14 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 04:19:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:19:15 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 04:19:15 GMT
EXPOSE 80
# Wed, 26 Jan 2022 04:19:15 GMT
CMD ["apache2-foreground"]
# Wed, 26 Jan 2022 21:02:25 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Wed, 26 Jan 2022 21:02:28 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         bash         busybox-static     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 21:03:24 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libicu-dev         zlib1g-dev         libzip-dev         libpng-dev         libxml2-dev         libfreetype6-dev         libjpeg62-turbo-dev         libgmp-dev         libmemcached-dev         libwebp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     if [ ! -e /usr/include/gmp.h ]; then ln -s /usr/include/$debMultiarch/gmp.h /usr/include/gmp.h; fi;    docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j$(nproc)         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.6;         docker-php-ext-enable         apcu         memcached         redis     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;         ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;             apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 21:03:25 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Wed, 26 Jan 2022 21:03:25 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Wed, 26 Jan 2022 21:03:26 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Wed, 26 Jan 2022 21:03:26 GMT
RUN set -ex;         a2enmod headers rewrite remoteip;     {         echo RemoteIPHeader X-Real-IP;         echo RemoteIPTrustedProxy 10.0.0.0/8;         echo RemoteIPTrustedProxy 172.16.0.0/12;         echo RemoteIPTrustedProxy 192.168.0.0/16;     } > $APACHE_CONFDIR/conf-available/remoteip.conf;     a2enconf remoteip
# Wed, 26 Jan 2022 21:03:27 GMT
RUN set -ex;     APACHE_DOCUMENT_ROOT=/var/www/html/public;     sed -ri -e "s!/var/www/html!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/sites-available/*.conf;     sed -ri -e "s!/var/www/!${APACHE_DOCUMENT_ROOT}!g" $APACHE_CONFDIR/apache2.conf $APACHE_CONFDIR/conf-available/*.conf
# Wed, 26 Jan 2022 21:03:27 GMT
WORKDIR /var/www/html
# Tue, 08 Feb 2022 19:41:39 GMT
ENV MONICA_VERSION=v3.7.0
# Tue, 08 Feb 2022 19:41:39 GMT
LABEL org.opencontainers.image.revision=a07317f309f25772925436346b4ebb23b6e69b43 org.opencontainers.image.version=v3.7.0
# Tue, 08 Feb 2022 19:42:07 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 08 Feb 2022 19:42:11 GMT
COPY multi:72e8bce953fdf60df31c4a1bb50faa001efd8f7eaaf696121cf35f8ea9080af7 in /usr/local/bin/ 
# Tue, 08 Feb 2022 19:42:12 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 08 Feb 2022 19:42:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d388c00adf9d70c76ee6e62579fb6aaaf5de79c35dfdec2f01bac554e92b217f`  
		Last Modified: Wed, 26 Jan 2022 05:19:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7fd053151e2d3345606bec45dc234d4da439d0212c54fea8710ca8886a597`  
		Last Modified: Wed, 26 Jan 2022 05:19:12 GMT  
		Size: 71.6 MB (71617962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180f356f15b9f7b050e52b2895a61c852b462ee0e88317b4be1cb7f38cecaf64`  
		Last Modified: Wed, 26 Jan 2022 05:19:02 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca22c94ed4686fff6967b01a3532b6f257d204c623cbe3f746cda3d935967f`  
		Last Modified: Wed, 26 Jan 2022 05:19:54 GMT  
		Size: 19.1 MB (19051142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdb52d188168f2d90bc652b785b253e9048e6d21349d2c5fad7e83e521926ce`  
		Last Modified: Wed, 26 Jan 2022 05:19:51 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948dab850abfbdec2d682f72caacc990c89f5dac555c959394038b4475c3b99`  
		Last Modified: Wed, 26 Jan 2022 05:19:51 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ed02f7fb7b465085a6b0d89b4362c2cbfa74ed6f35b02e25a54b7cddc998dc`  
		Last Modified: Wed, 26 Jan 2022 05:23:12 GMT  
		Size: 11.1 MB (11103640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9079bfeb043af78d38ef65b07a62836f501c7de8343e6032e8798614a202057`  
		Last Modified: Wed, 26 Jan 2022 05:23:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e5eba859085feee69020d5736d4d631910d4fa15744bebc3014b9393e2a5fc`  
		Last Modified: Wed, 26 Jan 2022 05:23:13 GMT  
		Size: 13.5 MB (13454749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bacc2cdc723c09431c972368137a7b25a54b9ff194c253cb978556a1bb5db9`  
		Last Modified: Wed, 26 Jan 2022 05:23:11 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b93a094cef52ae34a0635b3dfa20006f367ad6579c5025b77c5f6aa7fe71cc8`  
		Last Modified: Wed, 26 Jan 2022 05:23:10 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963c20d69177f2107ee198a999e3dc057564a34ff744e5e54997ab3922f13aa9`  
		Last Modified: Wed, 26 Jan 2022 05:23:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e256a067573ef7a9a5cb95040f5df3229cf51bd926b2ccba0779849b3d788ba`  
		Last Modified: Wed, 26 Jan 2022 21:06:12 GMT  
		Size: 1.3 MB (1349013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68f2f5efaffee2bc35095961abf762dfec34abdbdd9556025ab3a586ff9e94d`  
		Last Modified: Wed, 26 Jan 2022 21:06:13 GMT  
		Size: 4.0 MB (4004447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c6212c5b0a8cc8980aa90937f861af2d4f1df6a07b3e9fd3f6c8c2c2a60dd`  
		Last Modified: Wed, 26 Jan 2022 21:06:12 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f48b97a19b895e6dd0519ad9092fb4589daca6446b79ba7fe1b78d198c848`  
		Last Modified: Wed, 26 Jan 2022 21:06:11 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c86d5cd6090a3bcf7cf800508ca0ae42c1bbfcc5122539e0b65a960a2abe20`  
		Last Modified: Wed, 26 Jan 2022 21:06:11 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00996bc7bd85391332419951951e66f2c096f10f99993a5df42bf5b1bdf0c0`  
		Last Modified: Wed, 26 Jan 2022 21:06:11 GMT  
		Size: 8.3 KB (8302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77327f0752e22f662c3e92962039ec23522367809f72a70f146ca8366304b554`  
		Last Modified: Tue, 08 Feb 2022 19:44:06 GMT  
		Size: 35.3 MB (35337604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39503c3e3d53c22d0bc18c1a6c507a26daace81ddddaba339012cbffd59bc7c1`  
		Last Modified: Tue, 08 Feb 2022 19:43:59 GMT  
		Size: 2.0 KB (2030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
