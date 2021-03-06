## `nextcloud:production-fpm-alpine`

```console
$ docker pull nextcloud@sha256:1663fb2e140190f030f968f104db2e000de598b36df2c5c24fc4715a92130fc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nextcloud:production-fpm-alpine` - linux; amd64

```console
$ docker pull nextcloud@sha256:7ab6054936c6e8bbb31e0c79383a21239e632415b0b4911398a8b6e21bea59e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170209791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f3fe889eb3e570f7c1fef9bc114a2370085239f09c7181619642a8ab39efaf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 00:07:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 18 Feb 2021 00:07:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 18 Feb 2021 00:07:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 18 Feb 2021 00:07:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 18 Feb 2021 00:07:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 18 Feb 2021 00:21:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 18 Feb 2021 00:21:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 18 Feb 2021 00:21:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 18 Feb 2021 00:21:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 18 Feb 2021 00:46:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Feb 2021 00:46:56 GMT
ENV PHP_VERSION=7.4.15
# Thu, 18 Feb 2021 00:46:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 18 Feb 2021 00:46:56 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 18 Feb 2021 00:47:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Feb 2021 00:47:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:58:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Feb 2021 00:58:48 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:58:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Feb 2021 00:58:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Feb 2021 00:58:50 GMT
WORKDIR /var/www/html
# Thu, 18 Feb 2021 00:58:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Feb 2021 00:58:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Feb 2021 00:58:52 GMT
EXPOSE 9000
# Thu, 18 Feb 2021 00:58:52 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 07:53:11 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 07:55:42 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 22:18:31 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 22:18:31 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 22:18:32 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 22:18:32 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 22:22:51 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 22:23:30 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 22:23:32 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 22:23:33 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 22:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 22:23:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccf1c569cdbc9b110a3d500f1a3b660e3328f6b495c85cff29741b7dadcd0c4`  
		Last Modified: Thu, 18 Feb 2021 01:49:12 GMT  
		Size: 1.7 MB (1694702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec65deac30f6e14c8114b155c148f1863f824128d44e27874ac1a2e44a58823c`  
		Last Modified: Thu, 18 Feb 2021 01:49:11 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a32b6dca15d3cebbf4a92912832ba0d9fc60af0448a820ff80e146aa8b4cb13`  
		Last Modified: Thu, 18 Feb 2021 01:49:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210ab7e083dfa73a5ff97a1ad5d4ac5bb691cdba87b4747204101352ea375f13`  
		Last Modified: Thu, 18 Feb 2021 01:50:47 GMT  
		Size: 10.4 MB (10351764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f82cc40c2995041ef861350da160861d048210fa56e1f7c8d0a0382fb5a2bf6`  
		Last Modified: Thu, 18 Feb 2021 01:50:45 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4079d2a57bece3b766bc5ce64c27490021eedb0f6d96c40c8728a29a0c5734c`  
		Last Modified: Thu, 18 Feb 2021 01:50:50 GMT  
		Size: 14.3 MB (14316876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1a72718b07dd449891333db817c5aa41fbce51046d289bd602e08968673bb1`  
		Last Modified: Thu, 18 Feb 2021 01:50:45 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0c57e5b65ad1e5cd730eb8adcc957087a99412feb95d288348d3d3c7104d3e`  
		Last Modified: Thu, 18 Feb 2021 01:50:45 GMT  
		Size: 17.5 KB (17515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8750b2caef12ba765ee3d6b4743a2608eb6934a34f0535d941b6ca2ca57f7b`  
		Last Modified: Thu, 18 Feb 2021 01:50:45 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a4a9b458ace91833b9d5d6f907e00c827bb0f8758a5e8692570f824d96b525`  
		Last Modified: Thu, 18 Feb 2021 07:58:49 GMT  
		Size: 657.4 KB (657370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eadcfe0ce6c7d23b787bfda20b9816cda88735218761dbedec2ccbbe937627`  
		Last Modified: Thu, 18 Feb 2021 07:58:52 GMT  
		Size: 25.4 MB (25357410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25604e8df3a64f4b93dd398b6bc07d6398412dab3d906dcc6d1dd7ae30afe142`  
		Last Modified: Fri, 19 Feb 2021 22:30:54 GMT  
		Size: 565.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b786178666d7010edf7723e2bb823b7cbd4225489c4d7026bc5e4095d379ce77`  
		Last Modified: Fri, 19 Feb 2021 22:34:53 GMT  
		Size: 115.0 MB (114984850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ffc76bfdb6747151d627df1bb5f889be9ff2ce3759df43b817180d4fd0b79`  
		Last Modified: Fri, 19 Feb 2021 22:34:24 GMT  
		Size: 2.5 KB (2529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d38b9ddf66953724c1fcf847e9126be1bc9f45c892c62286b7cb5b4cafa1f3a`  
		Last Modified: Fri, 19 Feb 2021 22:34:24 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; arm variant v6

```console
$ docker pull nextcloud@sha256:9949955cf015bcbe93be53e4abe89445e5b3461a0e54f8483f9b61a13adfb779
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168059015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3568f053020ecaae51364d3fb61323ca74300bcad66a89c9a4366e97d54453`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:17:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 17 Feb 2021 22:17:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 17 Feb 2021 22:17:15 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 17 Feb 2021 22:17:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Feb 2021 22:17:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Feb 2021 22:20:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 17 Feb 2021 22:20:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 22:20:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 22:20:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Feb 2021 22:28:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 17 Feb 2021 22:28:42 GMT
ENV PHP_VERSION=7.4.15
# Wed, 17 Feb 2021 22:28:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Wed, 17 Feb 2021 22:28:43 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Wed, 17 Feb 2021 22:28:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 17 Feb 2021 22:28:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 17 Feb 2021 22:34:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 17 Feb 2021 22:34:22 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 17 Feb 2021 22:34:25 GMT
RUN docker-php-ext-enable sodium
# Wed, 17 Feb 2021 22:34:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 17 Feb 2021 22:34:27 GMT
WORKDIR /var/www/html
# Wed, 17 Feb 2021 22:34:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 17 Feb 2021 22:34:30 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Feb 2021 22:34:30 GMT
EXPOSE 9000
# Wed, 17 Feb 2021 22:34:31 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 02:38:18 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 02:42:12 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 20:02:18 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:02:19 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:02:23 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:02:24 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:05:06 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:06:06 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 20:06:09 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:06:12 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:06:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:06:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a33e390360f607fe5a7fe0a0203b7347693b0d8cab270352594a3700e1a1d0`  
		Last Modified: Wed, 17 Feb 2021 22:57:10 GMT  
		Size: 1.7 MB (1684729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d1bbb88bd210deaf33702df9d6fa7f35e72f23dfbb55196147ab537320e9f3`  
		Last Modified: Wed, 17 Feb 2021 22:57:09 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b99fbc527c373db47c36282e5bbd82010870902db2af45982bbb8d700375a32`  
		Last Modified: Wed, 17 Feb 2021 22:57:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc98fe1c24d3e1ca723fb3f4bed6da828637b898bc3d9468bb2fe46e1fc8436`  
		Last Modified: Wed, 17 Feb 2021 22:58:37 GMT  
		Size: 10.4 MB (10351758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dc0e55372eac2ea79f505d45612af664d8843231485fd782aae22070be2c6`  
		Last Modified: Wed, 17 Feb 2021 22:58:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11322b4673f5859cc9d9f14f1714b76fc5a54598bfbae9d8c35064e9b85f67e0`  
		Last Modified: Wed, 17 Feb 2021 22:58:39 GMT  
		Size: 13.3 MB (13309645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20fae0fe8d81eb020214e2e1cd8b8dbbf515c74ea3a8a10c5e5742bc0f46741`  
		Last Modified: Wed, 17 Feb 2021 22:58:33 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65939c05e9dfa96e3bcd3faea952171300f05d287335a1438a917d29e263ab`  
		Last Modified: Wed, 17 Feb 2021 22:58:33 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b317f5717ed617999a21085988c4f63159150b90f4c364c2a24320a415321781`  
		Last Modified: Wed, 17 Feb 2021 22:58:33 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a75987c0e1f131941d955e8bad3974407bb384c5d0459d6b7f3fac04e02777`  
		Last Modified: Thu, 18 Feb 2021 02:46:19 GMT  
		Size: 620.0 KB (619981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ce3e197181e89f5cd0c69926c9bf12edc624517c7db8af8bd1bb81d7d7260e`  
		Last Modified: Thu, 18 Feb 2021 02:46:25 GMT  
		Size: 24.5 MB (24450742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5358211183de5b0e5f2f55733d62423bd3be78b99f5bea9e0eb265a9f9e26ff`  
		Last Modified: Fri, 19 Feb 2021 20:09:36 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef9fc8881cb6c3545ed9865ef83ce89ee982d4e370f8439882bf0ff98e38ae8`  
		Last Modified: Fri, 19 Feb 2021 20:11:41 GMT  
		Size: 115.0 MB (114984852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa577adcc6c26ececd18905b5d7602ed47f649b1f0ab807f630e8f4abda72151`  
		Last Modified: Fri, 19 Feb 2021 20:11:00 GMT  
		Size: 2.5 KB (2529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cdfc8e2d099b17aa8969e0a63514239850f06a6ca420353e06f49e65e13aea`  
		Last Modified: Fri, 19 Feb 2021 20:11:00 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:0520c0de4dbd714c043369629e5e83eba6f0da574fc477d8c0b03ddd6df45aa4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.4 MB (166400234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d5abd4151096395de3e1d3f1f199bdcd2062d5584c321b8507102ef9a2a865`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:56:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 17 Feb 2021 22:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 17 Feb 2021 22:57:04 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 17 Feb 2021 22:57:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Feb 2021 22:57:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Feb 2021 23:02:51 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 17 Feb 2021 23:02:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 23:02:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 23:02:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Feb 2021 23:10:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 17 Feb 2021 23:10:45 GMT
ENV PHP_VERSION=7.4.15
# Wed, 17 Feb 2021 23:10:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Wed, 17 Feb 2021 23:10:47 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Wed, 17 Feb 2021 23:10:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 17 Feb 2021 23:10:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 17 Feb 2021 23:14:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 17 Feb 2021 23:14:17 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 17 Feb 2021 23:14:20 GMT
RUN docker-php-ext-enable sodium
# Wed, 17 Feb 2021 23:14:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 17 Feb 2021 23:14:24 GMT
WORKDIR /var/www/html
# Wed, 17 Feb 2021 23:14:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 17 Feb 2021 23:14:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Feb 2021 23:14:29 GMT
EXPOSE 9000
# Wed, 17 Feb 2021 23:14:29 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 03:21:12 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 03:24:54 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 21:04:24 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 21:04:25 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 21:04:27 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 21:04:28 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 21:11:59 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 21:12:55 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 21:12:57 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 21:13:01 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 21:13:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 21:13:05 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf491575714634902d01e3e48f3b92702cb2e4c42056aa5421058d2a2cbfd9f6`  
		Last Modified: Wed, 17 Feb 2021 23:33:58 GMT  
		Size: 1.6 MB (1555125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8ae33f1196d3a62a9383b30d3fd81dd4be1bcf1a99a3d928f585b0d85c5408`  
		Last Modified: Wed, 17 Feb 2021 23:33:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16bd16ac2dc3896b7ddf5e8e50bafcc3990d8313dc26634a51beafc97cc6374`  
		Last Modified: Wed, 17 Feb 2021 23:33:58 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ea7cd652a281fd80d484ef1ed7432caedbef26aacbeea707de7e5e96171b60`  
		Last Modified: Wed, 17 Feb 2021 23:35:46 GMT  
		Size: 10.4 MB (10351768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767a935df72db0997004bf0d6ba06f462be7d1353090dd2a3d8c38045e4b9dd2`  
		Last Modified: Wed, 17 Feb 2021 23:35:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da196c37e6c6b71136d89e9988b31f9b60b5a36c935e21c936d8692eebf838a`  
		Last Modified: Wed, 17 Feb 2021 23:35:48 GMT  
		Size: 12.5 MB (12466444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179a06de768532ba9c6f33016c53537f3641cb5659b88b78a1df7dcbdfc78112`  
		Last Modified: Wed, 17 Feb 2021 23:35:44 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d3a95bcccd62c0a0fb00a537a603ad28b1f7d850d7e2ab00852cedfc07c34`  
		Last Modified: Wed, 17 Feb 2021 23:35:44 GMT  
		Size: 17.5 KB (17518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f8d3dde1b702024e029250e6b9405aaa01c40cb57d39d050b101eb29ed5fc`  
		Last Modified: Wed, 17 Feb 2021 23:35:44 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f72e0826dfd44246ae224c61878daa10b70b7e9f0cedffd6b4115a1059a1f32`  
		Last Modified: Thu, 18 Feb 2021 03:30:18 GMT  
		Size: 560.0 KB (560006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74155796a38618da1207e9229b3a08509eb9d57c555cc546544e88ab5f678a72`  
		Last Modified: Thu, 18 Feb 2021 03:30:22 GMT  
		Size: 24.0 MB (24022875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3bbca7fd787e37bd4dec34453658b7fa4b287650a3eba1bf87eea07c26241`  
		Last Modified: Fri, 19 Feb 2021 21:23:54 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceda2770ee9644a14f61dafc412a377a6aed01f1bf57f3812b342582ff1cb06`  
		Last Modified: Fri, 19 Feb 2021 21:29:31 GMT  
		Size: 115.0 MB (114984850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf25a3284e8db9d5b69f85290a73aa34da439b56bac74d09bc9ee2578f4571a1`  
		Last Modified: Fri, 19 Feb 2021 21:28:53 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b53b1b9eb184017477ff8a643dca55e10da6d761779bb7735342fb320b1acb`  
		Last Modified: Fri, 19 Feb 2021 21:28:53 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:477807e5e28746610a3ecce19d666371029f536792941198739f0536407d55fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169617773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d99d41cd48bb5e7feee2709bf19c9d82521b871b03d9240920cc43fcb8918ba9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:42:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 17 Feb 2021 23:42:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 17 Feb 2021 23:42:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 17 Feb 2021 23:42:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Feb 2021 23:42:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Feb 2021 23:47:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 17 Feb 2021 23:47:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 23:47:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 23:47:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Feb 2021 23:57:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 17 Feb 2021 23:57:45 GMT
ENV PHP_VERSION=7.4.15
# Wed, 17 Feb 2021 23:57:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Wed, 17 Feb 2021 23:57:49 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Wed, 17 Feb 2021 23:57:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 17 Feb 2021 23:57:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:02:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Feb 2021 00:02:20 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:02:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Feb 2021 00:02:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Feb 2021 00:02:25 GMT
WORKDIR /var/www/html
# Thu, 18 Feb 2021 00:02:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Feb 2021 00:02:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Feb 2021 00:02:29 GMT
EXPOSE 9000
# Thu, 18 Feb 2021 00:02:30 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 04:20:50 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 04:24:31 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 20:45:05 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:45:06 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:45:08 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:45:09 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:51:41 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:52:26 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 20:52:33 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:52:36 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:52:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:52:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4b642bcaaef409203aaedc803835562ee86d3ea457bf4ccdd22e5d7b2367f1`  
		Last Modified: Thu, 18 Feb 2021 00:23:35 GMT  
		Size: 1.7 MB (1694455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ea39643e14bb66b107bb23b02b8c7a193ed89d38f4ae52b1decbe763fb0db9`  
		Last Modified: Thu, 18 Feb 2021 00:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3455119714d8ce066305d3b121e103a3cf690db26bb556906ba67e7a7c1f559`  
		Last Modified: Thu, 18 Feb 2021 00:23:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f0f505e8d9e25a447ca37f6f1d943270b2c5ec9db527df7be2ac7e9fe2506d`  
		Last Modified: Thu, 18 Feb 2021 00:25:10 GMT  
		Size: 10.4 MB (10351789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8b1939cdc123a434384ecdc6abb9b9e6871d99cd6628e0d2294115dd2b70d3`  
		Last Modified: Thu, 18 Feb 2021 00:25:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6244f613c87bf78863e69b5743b59d211224275ff28778cb3d542c58c60bdfcd`  
		Last Modified: Thu, 18 Feb 2021 00:25:16 GMT  
		Size: 14.1 MB (14089792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2514123300588dddde3f3246c1420af7b976d711f09f56e999dc996cd0ff6f`  
		Last Modified: Thu, 18 Feb 2021 00:25:07 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9083eb6a809619648dd117bcb0c059b115142528cf0718f6e73eca6547a468b`  
		Last Modified: Thu, 18 Feb 2021 00:25:07 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f930032d07466be7897e4ef4aee5c671e567148f86748f041899f6ea6a2d3b13`  
		Last Modified: Thu, 18 Feb 2021 00:25:07 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b839c833fe5f226fcc3e17161e3ca2c73f3aac8a138fa12d10e3dca5cd277a`  
		Last Modified: Thu, 18 Feb 2021 04:28:45 GMT  
		Size: 658.1 KB (658095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d955370f899027f28f80af0a5c0ca7b9a053ef9053fe62e386e955adf101b35`  
		Last Modified: Thu, 18 Feb 2021 04:28:49 GMT  
		Size: 25.1 MB (25091877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833ce94a9a602f6668d068c72e141017356221bf9c79ca413b76f4bc65c2ae5a`  
		Last Modified: Fri, 19 Feb 2021 21:02:55 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396ac4d60a0a802382054042817c2a0087b10051f3e7bd4ddf77111b5b52b3c`  
		Last Modified: Fri, 19 Feb 2021 21:07:48 GMT  
		Size: 115.0 MB (114984902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9b1a252e851eee799f98dd82a01bc3f14e6083be152b799ca578d7d0deaf28`  
		Last Modified: Fri, 19 Feb 2021 21:07:19 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984efec1157c6cb232faca839abff13182e3555a667eb560a08addad6fdc05e4`  
		Last Modified: Fri, 19 Feb 2021 21:07:19 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; 386

```console
$ docker pull nextcloud@sha256:3c87c7880226412bea997a08f77678d77742e74788d1d70ae4a838dfcc21f024
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171060736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515637fdca93e4d3ca5db56408df5fa6220dc244a9155b28a5830e277fa195a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:49:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 17 Feb 2021 23:49:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 17 Feb 2021 23:49:13 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 17 Feb 2021 23:49:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Feb 2021 23:49:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Feb 2021 23:57:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 17 Feb 2021 23:57:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 23:57:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Feb 2021 23:57:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 18 Feb 2021 00:20:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Feb 2021 00:20:08 GMT
ENV PHP_VERSION=7.4.15
# Thu, 18 Feb 2021 00:20:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 18 Feb 2021 00:20:08 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 18 Feb 2021 00:20:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Feb 2021 00:20:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:32:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Feb 2021 00:32:36 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:32:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Feb 2021 00:32:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Feb 2021 00:32:39 GMT
WORKDIR /var/www/html
# Thu, 18 Feb 2021 00:32:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Feb 2021 00:32:41 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Feb 2021 00:32:42 GMT
EXPOSE 9000
# Thu, 18 Feb 2021 00:32:42 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 04:44:46 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 04:47:33 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 21:43:58 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 21:43:58 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 21:43:59 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 21:44:00 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 21:50:47 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 21:51:42 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 21:51:43 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 21:51:45 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 21:51:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 21:51:46 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0deb53f370403cb55f5b50d6db51a7c37e056ab41c21ee510914c61b7d0af707`  
		Last Modified: Thu, 18 Feb 2021 01:28:38 GMT  
		Size: 1.8 MB (1793489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90de99a2e97bfd6926c4c81dc7b6cb82e87ed97cdc9af654ca5971355155874c`  
		Last Modified: Thu, 18 Feb 2021 01:28:37 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74185055e3600ff78e192e1a38fa26c768066e0ea82ceb6305097ed9fb98b34`  
		Last Modified: Thu, 18 Feb 2021 01:28:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0407194512b26806cdd98555712100d31c1cd92487b2eaa73143c4350a202e9b`  
		Last Modified: Thu, 18 Feb 2021 01:30:37 GMT  
		Size: 10.4 MB (10351729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c28636df1516e8a03744fa7907b731111abafc03e86b25416147ccaf7ed3b1`  
		Last Modified: Thu, 18 Feb 2021 01:30:34 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69bc187fe3c0dad941b74b2fbeaee0697425677d319d7511b67ac6e8d6908b6`  
		Last Modified: Thu, 18 Feb 2021 01:30:43 GMT  
		Size: 14.7 MB (14698469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2468a11b8da74b586dd1c7bd51132f8bc6c423d5fb667affaf356bf99078ff`  
		Last Modified: Thu, 18 Feb 2021 01:30:34 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855e0c811c1aa3e471453cd3a10954a0fc39155cb4349a14c3710f81292540f1`  
		Last Modified: Thu, 18 Feb 2021 01:30:34 GMT  
		Size: 17.5 KB (17504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5a784680a66eec6410938c72a3175715bc8907cb1867cf06eb32d70f40304a`  
		Last Modified: Thu, 18 Feb 2021 01:30:34 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6516b7bfa4d929041a0f44ffcd06c6d3332afd71d0e8bf5ce45db7db63575e5c`  
		Last Modified: Thu, 18 Feb 2021 04:51:02 GMT  
		Size: 648.0 KB (647996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9a644d52514764feb724e912689d385eef4676d6ce3952265e5afb767d5d84`  
		Last Modified: Thu, 18 Feb 2021 04:51:08 GMT  
		Size: 25.7 MB (25730986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1afc6b19941dd488e1be782725b14a42bbc064869ce47d53dc57b304d35185`  
		Last Modified: Fri, 19 Feb 2021 22:02:28 GMT  
		Size: 564.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d279d5dfd91669d1947b3dabda76b1514f806490fcd65a5f8308176234bbe1`  
		Last Modified: Fri, 19 Feb 2021 22:08:07 GMT  
		Size: 115.0 MB (114984739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2e4155a6d186ef8bdc86ebe1b70d86e3e3fd6f5999d22d7c97457fd4f9bbea`  
		Last Modified: Fri, 19 Feb 2021 22:07:28 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a52eb150b9c7a1bffb1de544a17949ba977d2e190022d529b3d854ef7cd7f1`  
		Last Modified: Fri, 19 Feb 2021 22:07:28 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:94826e60fe84dd34572935cc432d11e8b7932b01868f9b333b9778e28fcd38b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.7 MB (171709573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b01fc34b8172f1b9009d8ea62b565f3581733350db15f43793afe953386141`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 00:23:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 18 Feb 2021 00:24:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 18 Feb 2021 00:24:44 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 18 Feb 2021 00:24:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 18 Feb 2021 00:25:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 18 Feb 2021 00:32:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 18 Feb 2021 00:32:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 18 Feb 2021 00:32:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 18 Feb 2021 00:32:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 18 Feb 2021 00:47:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Feb 2021 00:47:32 GMT
ENV PHP_VERSION=7.4.15
# Thu, 18 Feb 2021 00:47:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 18 Feb 2021 00:47:46 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 18 Feb 2021 00:48:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Feb 2021 00:48:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:53:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Feb 2021 00:53:20 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 18 Feb 2021 00:53:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Feb 2021 00:53:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Feb 2021 00:53:46 GMT
WORKDIR /var/www/html
# Thu, 18 Feb 2021 00:53:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Feb 2021 00:54:05 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Feb 2021 00:54:10 GMT
EXPOSE 9000
# Thu, 18 Feb 2021 00:54:22 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 06:27:43 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 06:31:08 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 21:53:02 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 21:53:08 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 21:53:22 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 21:53:26 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 22:16:37 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 22:18:57 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 22:19:05 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 22:19:08 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 22:19:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 22:19:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebfde0ed2b25fdf7a28b46b01e73c7891af78bd260ce9c5f46f33a0fd4bba5a`  
		Last Modified: Thu, 18 Feb 2021 01:25:11 GMT  
		Size: 1.7 MB (1741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c587bda2cf37683b8f80371450083e1533df270a51cbe196c845e7ab52f8943`  
		Last Modified: Thu, 18 Feb 2021 01:25:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2faee0918d4167a0323dba5b4244442a3d6cd88d5eacd4a560b72f056274a4`  
		Last Modified: Thu, 18 Feb 2021 01:25:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333dbe0927a80c42a09c27eced48c55de6496609f9753007625e3e4cebda85d3`  
		Last Modified: Thu, 18 Feb 2021 01:27:29 GMT  
		Size: 10.4 MB (10351755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd7ee33527dc95696abb9ad2dd358ba55bb403808771a4246a67353561bc5e2`  
		Last Modified: Thu, 18 Feb 2021 01:27:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d78ad1ca1fd6aa3bcec914ee66da48a0231750112e303adb94ac1774882fe4`  
		Last Modified: Thu, 18 Feb 2021 01:27:29 GMT  
		Size: 15.4 MB (15355606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283e600c287f37c619e6d4d7a82f19aa5eec439126013441af4a8df59963fe0e`  
		Last Modified: Thu, 18 Feb 2021 01:27:25 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044176c25fb405e9f981fc85488f434642eab8a7c799960b47122d69d1088e11`  
		Last Modified: Thu, 18 Feb 2021 01:27:25 GMT  
		Size: 17.5 KB (17524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0be64f7f4ade6f8b6477a3c3c2900b8a26b6c07cb17a6691250e0a2a37438ca`  
		Last Modified: Thu, 18 Feb 2021 01:27:25 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fef3a9215e915d8e26e704b9c08186fa179068901227417ceae761a369ea7c`  
		Last Modified: Thu, 18 Feb 2021 06:39:43 GMT  
		Size: 756.4 KB (756445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e217df5dfb60e7b96b719a00ea68e6a5302c9da4422e99d33ae946946d7e5f3`  
		Last Modified: Thu, 18 Feb 2021 06:39:44 GMT  
		Size: 25.7 MB (25670874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2182191e6b59cb84eaf059fbaf711d106b4b2772f35ac5dc84cd7159f9c37f5b`  
		Last Modified: Fri, 19 Feb 2021 22:46:26 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdc397d2b962cd42d490ab3884046a39ece3c9d1c1cab1a737d20b72f186cf3`  
		Last Modified: Fri, 19 Feb 2021 23:01:37 GMT  
		Size: 115.0 MB (114984869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba5e711cbe9477efb959dd8f3f5d6304eb450e5bb476ad0782f083a288d10fa`  
		Last Modified: Fri, 19 Feb 2021 22:59:31 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e5fcba4bf585364321f260e5a6b866ac3ea9398f88147f131d1c3b70d5e804`  
		Last Modified: Fri, 19 Feb 2021 22:59:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; s390x

```console
$ docker pull nextcloud@sha256:c0f56aae26bc9347153d86fc5b5f2e34aa1d5ffaa5942316742f7251590f832d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.2 MB (169156191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6464f186810c6606398485fd47793c23faa25293807ea47658c310e0dde39f2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 17 Feb 2021 20:41:27 GMT
ADD file:630c66f8d774d75b51e32aff812b438d377ebd3389c4aa6c324fdf8c03b6fa13 in / 
# Wed, 17 Feb 2021 20:41:27 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 00:40:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 18 Feb 2021 00:40:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 18 Feb 2021 00:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 18 Feb 2021 00:40:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 18 Feb 2021 00:40:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 18 Feb 2021 00:46:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 18 Feb 2021 00:46:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 18 Feb 2021 00:46:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 18 Feb 2021 00:46:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 18 Feb 2021 00:56:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Feb 2021 00:56:47 GMT
ENV PHP_VERSION=7.4.15
# Thu, 18 Feb 2021 00:56:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 18 Feb 2021 00:56:48 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 18 Feb 2021 00:56:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Feb 2021 00:56:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Feb 2021 01:02:02 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:02:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Feb 2021 01:02:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Feb 2021 01:02:05 GMT
WORKDIR /var/www/html
# Thu, 18 Feb 2021 01:02:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Feb 2021 01:02:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Feb 2021 01:02:08 GMT
EXPOSE 9000
# Thu, 18 Feb 2021 01:02:09 GMT
CMD ["php-fpm"]
# Thu, 18 Feb 2021 03:02:18 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 18 Feb 2021 03:04:48 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.3;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 19 Feb 2021 20:11:34 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 19 Feb 2021 20:11:34 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 19 Feb 2021 20:11:35 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 19 Feb 2021 20:11:35 GMT
VOLUME [/var/www/html]
# Fri, 19 Feb 2021 20:17:01 GMT
ENV NEXTCLOUD_VERSION=20.0.7
# Fri, 19 Feb 2021 20:17:39 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Fri, 19 Feb 2021 20:17:56 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Fri, 19 Feb 2021 20:17:58 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Fri, 19 Feb 2021 20:17:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Feb 2021 20:17:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ff5e8cb87555e9fa38a441f5cf0414e91353e2cd21cdb48d48b7de5bb39ce674`  
		Last Modified: Wed, 17 Feb 2021 20:41:58 GMT  
		Size: 2.6 MB (2602381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eaf748a32e76be0f1aa6246cb11c8aa5022aa834df364bb87f581198e6376`  
		Last Modified: Thu, 18 Feb 2021 01:26:48 GMT  
		Size: 1.8 MB (1756400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5716be54c61b8e2a38b4d6a0cbece88801726747842f6bd1a50aaf4e8442013f`  
		Last Modified: Thu, 18 Feb 2021 01:26:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aa66a8dad4ec1443c27324fc452b05c4299dbffefcebee55700880033b3ff7`  
		Last Modified: Thu, 18 Feb 2021 01:26:47 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c7dcfcd7af5478eb3b38294f3be2dce058e756e190861907611ac961754715`  
		Last Modified: Thu, 18 Feb 2021 01:28:37 GMT  
		Size: 10.4 MB (10351770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981e48c622f07d957fba5800e1a56c1a262c7a490711fd847a011f542c4feff8`  
		Last Modified: Thu, 18 Feb 2021 01:28:34 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7a1ca6ccf9c03a5e6c87734c3dcab542d2f6002bdab7cb3da73f2a4140d9e1`  
		Last Modified: Thu, 18 Feb 2021 01:28:37 GMT  
		Size: 13.7 MB (13674927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc6fcf7c8fa53efee79a97b58bfcbf0d781e7ad91b4e5c209020679cf7cc25e`  
		Last Modified: Thu, 18 Feb 2021 01:28:35 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21e87df2ecc141e0c021f7d1f757b4993dbb8b4a5c7a94ba7f2a2663cd9bd29`  
		Last Modified: Thu, 18 Feb 2021 01:28:34 GMT  
		Size: 17.5 KB (17520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6d1496f3768ae581da3ebeb2f4b9fcb2d0dc8dc25637afd9602bee4287a89d`  
		Last Modified: Thu, 18 Feb 2021 01:28:35 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9fdc79521b0490c565658c567f2adf3796bb3b232f9acbff3ed4ef5878b79`  
		Last Modified: Thu, 18 Feb 2021 03:09:26 GMT  
		Size: 652.8 KB (652798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeebc9f1b3eb582e327cead2cf9354519bec251c505c7c85610a4c882cc074f`  
		Last Modified: Thu, 18 Feb 2021 03:09:28 GMT  
		Size: 25.1 MB (25097812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d3dca2abd0ea827805b99db4de8e2d0d52cc5938302a54a82a8387de2a0406`  
		Last Modified: Fri, 19 Feb 2021 20:28:15 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f2542cae37535e4322763da1d24e1da15c83f444e2cd7dbaa55cf3719864cb`  
		Last Modified: Fri, 19 Feb 2021 20:31:21 GMT  
		Size: 115.0 MB (114984838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ea51f909e6eccf09bed20274d222900a37cdaa3600fb1e02dec71b46ef6190`  
		Last Modified: Fri, 19 Feb 2021 20:31:02 GMT  
		Size: 2.5 KB (2529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d6ee17273e89434374b8bf76debd23a5e37687ea6649594e985921ec66f426`  
		Last Modified: Fri, 19 Feb 2021 20:31:02 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
