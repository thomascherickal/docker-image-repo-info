## `nextcloud:16-fpm-alpine`

```console
$ docker pull nextcloud@sha256:18b295d3936f7a3d01e282482b294f618dc245c50ac15207f0a20657b144e58a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `nextcloud:16-fpm-alpine` - linux; amd64

```console
$ docker pull nextcloud@sha256:09a8f9c630d8ccb765e35e77f07141818f0614826b0e74be4fc31b22c9e5bc5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125249686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590ec2a831a88ec8a333452a72de5b0695a7e577019605d438934adc9579f214`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:18:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:18:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:18:35 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:18:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:18:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 01:56:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 01:56:12 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 01:56:12 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 01:56:12 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 01:56:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 01:56:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 02:03:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 02:03:24 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 02:03:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 02:03:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 02:03:28 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 02:03:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 02:03:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 02:03:30 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 02:03:30 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 05:08:09 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/15 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 24 Mar 2020 05:10:56 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Tue, 24 Mar 2020 05:10:56 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 24 Mar 2020 05:10:57 GMT
VOLUME [/var/www/html]
# Tue, 24 Mar 2020 05:10:57 GMT
ENV NEXTCLOUD_VERSION=16.0.9
# Tue, 24 Mar 2020 05:11:15 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Wed, 01 Apr 2020 06:05:23 GMT
COPY multi:7ff9cff24b6270b00f83a8bfd2c1c1229276cb451cd1a6bd1ec44ef5d1270ba6 in / 
# Wed, 01 Apr 2020 06:05:23 GMT
COPY multi:07fbadbda22b19b1f9b8cfc5e833b697afbaa1e602ffea77b26286f5899f86d6 in /usr/src/nextcloud/config/ 
# Wed, 01 Apr 2020 06:05:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Apr 2020 06:05:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61c449d5d9102f11bc559aba323f82389b7be6118dea453e8273a7f8cc971ea`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 1.4 MB (1354647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fde16e1397a31e46a1030c8f769012ebe10f171fc564c77a692053c845975ff`  
		Last Modified: Tue, 24 Mar 2020 02:42:24 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1096698ab2a54e6370c1f2b9c6bb71ae2bb54e306f246aa436b77e1351ff1cf`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09ee4033d1f636e39d6cd200fa0451906b5417d71fcf17e1dcb97eb8b745e5`  
		Last Modified: Tue, 24 Mar 2020 02:43:49 GMT  
		Size: 12.1 MB (12133350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32670cfc718884cbe40e9158ede48957de177808b6889cf3e0dd3a02e53698cd`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bfbcc96d33915afdf2cc66767bbf705b8c047b08f99347bdd3e943d28fb69a`  
		Last Modified: Tue, 24 Mar 2020 02:43:50 GMT  
		Size: 14.5 MB (14465522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095f83f78721704875575f13144e7b1683c69713e0c00762962a63d0292f3d8d`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6234ddc68641c475c5f736d39fb36a1c925fc59d755593474f87b3846e5c21b`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 16.9 KB (16910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7af26f613dae4046542ee2180cfb8b343d2a3dd00d807b276001131c624877`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f380a9a7210b211cc153f7a85b62e1f8b34cd5560a22bbc018d8b9ab5187dfbc`  
		Last Modified: Tue, 24 Mar 2020 05:16:54 GMT  
		Size: 258.1 KB (258111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff01e771090505f081a4be9e36026cc42855232bee70ff673123532ea7b2aa7`  
		Last Modified: Tue, 24 Mar 2020 05:17:03 GMT  
		Size: 25.6 MB (25603029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38d231fb380403655179b742b8b3300938f4695c4ae436b3d07df2c3cf9da47`  
		Last Modified: Tue, 24 Mar 2020 05:16:53 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576b5cecd1c5214db7536aac649d382cd4635511f64781bfc6c9875f8c20a855`  
		Last Modified: Tue, 24 Mar 2020 05:17:15 GMT  
		Size: 68.6 MB (68598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46e86fceb635ee06f280426a4623df4f926bfea37ee48fb39a0aea3413dfce`  
		Last Modified: Wed, 01 Apr 2020 06:17:28 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e0befc493eb3da5a48a178ae61b56fea3ee7cc7cc4ef138eb8f326d1d650c`  
		Last Modified: Wed, 01 Apr 2020 06:17:28 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:16-fpm-alpine` - linux; arm variant v6

```console
$ docker pull nextcloud@sha256:8b5f3c78a977fbba881ea8ee5ac5c7f8dcd3076bb35f922ad1d520f198e0fe0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123191653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357a5b0f7db616485ede38a98661243ef0ed625274402aab87bb8e3b854da6ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:16:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 02:16:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 02:16:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 02:16:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 02:16:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 02:21:00 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 02:21:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:21:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:21:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 02:33:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 02:33:54 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 02:33:55 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 02:33:56 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 02:33:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 02:34:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 02:37:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 02:37:44 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 02:37:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 02:37:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 02:37:47 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 02:37:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 02:37:50 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 02:37:51 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 02:37:51 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 05:07:25 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/15 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 24 Mar 2020 05:10:40 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Tue, 24 Mar 2020 05:10:42 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 24 Mar 2020 05:10:43 GMT
VOLUME [/var/www/html]
# Tue, 24 Mar 2020 05:10:43 GMT
ENV NEXTCLOUD_VERSION=16.0.9
# Tue, 24 Mar 2020 05:11:16 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 31 Mar 2020 20:55:19 GMT
COPY multi:7ff9cff24b6270b00f83a8bfd2c1c1229276cb451cd1a6bd1ec44ef5d1270ba6 in / 
# Tue, 31 Mar 2020 20:55:22 GMT
COPY multi:07fbadbda22b19b1f9b8cfc5e833b697afbaa1e602ffea77b26286f5899f86d6 in /usr/src/nextcloud/config/ 
# Tue, 31 Mar 2020 20:55:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Mar 2020 20:55:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea08e138832a1357c5a2058da55929de016d0715372ec90df8716d8f08e8aa`  
		Last Modified: Tue, 24 Mar 2020 02:56:26 GMT  
		Size: 1.3 MB (1321096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6155177d2f4f58391e952733581935ca259371ca891a8e72311ff15a4b0caaf9`  
		Last Modified: Tue, 24 Mar 2020 02:56:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64588fb2e6842997faa53e9e5d4ec63be60ac226be4ae2eb5a97bff62263b14e`  
		Last Modified: Tue, 24 Mar 2020 02:56:25 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3586d89254f1b02ce08b4f85dcad2e5681dc6db1966c54c9fbb7240dc4bd01`  
		Last Modified: Tue, 24 Mar 2020 02:58:01 GMT  
		Size: 12.1 MB (12133370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7679b8e7281567c08633df43f610d267cab8d103b1e867940341e0b861a84a47`  
		Last Modified: Tue, 24 Mar 2020 02:57:59 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed716d896a3037f8ca49f16e3baaa358c0b4840ab4d97db27fcacb35b14691c`  
		Last Modified: Tue, 24 Mar 2020 02:58:04 GMT  
		Size: 13.4 MB (13430006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19be938005d675a9dbaadf62127df5fdba1a70a49b859d160ea7e98eb806b55`  
		Last Modified: Tue, 24 Mar 2020 02:57:58 GMT  
		Size: 2.2 KB (2213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2f08373e9ae9bb4f1ef7e8e38df22cc798c18b7ee7303f7c1dc619ee894c38`  
		Last Modified: Tue, 24 Mar 2020 02:57:58 GMT  
		Size: 16.9 KB (16876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ff71767caa409595ce427cb264b71f4725c0ca13b199a247d57fd59a41d198`  
		Last Modified: Tue, 24 Mar 2020 02:57:59 GMT  
		Size: 8.4 KB (8409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c37e330567ab76529024cf870b87350ddd375c79f1edf6d200e227832750a4d`  
		Last Modified: Tue, 24 Mar 2020 05:17:04 GMT  
		Size: 268.6 KB (268579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f109439ba5b8dc1de6c4efd2202f9586db377a4319fc6f483aa996019ca907`  
		Last Modified: Tue, 24 Mar 2020 05:17:09 GMT  
		Size: 24.8 MB (24788257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b152182d7c7eeabf9543fc62eb9115e9fd3e0832ae8f29e7275345c90f043b4`  
		Last Modified: Tue, 24 Mar 2020 05:17:02 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8008c5b191861d509b528157a3f2631c20843dd99768564aa5368e4eb91a42a`  
		Last Modified: Tue, 24 Mar 2020 05:17:28 GMT  
		Size: 68.6 MB (68598097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11da95db92cb7f51f669cc110f114e22d7bbf42ff2d71dd43c7a3b37c08aa5b`  
		Last Modified: Tue, 31 Mar 2020 20:55:58 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be60d5b1099111f5f2e354496d92a26dd856f6692361bab2bf7c6bd23e77d2e`  
		Last Modified: Tue, 31 Mar 2020 20:55:58 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:16-fpm-alpine` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:fea01c811b993bd6318f8ddc94d4fb4e5743b7cc51f876ef5273dffaa368d62f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121357305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2282e4dc17bce74e95ccd6f98e33c0c92487d33eecd05b06ae1bdd76721f9391`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:36:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:36:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:36:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:36:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:36:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:39:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:39:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:39:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:39:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 01:49:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 01:49:09 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 01:49:09 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 01:49:10 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 01:49:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 01:49:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 01:51:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 01:51:48 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 01:51:50 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 01:51:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 01:51:51 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 01:51:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 01:51:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 01:51:55 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 01:51:56 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 03:54:38 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/15 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 24 Mar 2020 03:57:48 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Tue, 24 Mar 2020 03:57:52 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 24 Mar 2020 03:57:53 GMT
VOLUME [/var/www/html]
# Tue, 24 Mar 2020 03:57:54 GMT
ENV NEXTCLOUD_VERSION=16.0.9
# Tue, 24 Mar 2020 03:58:33 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Wed, 01 Apr 2020 05:02:53 GMT
COPY multi:7ff9cff24b6270b00f83a8bfd2c1c1229276cb451cd1a6bd1ec44ef5d1270ba6 in / 
# Wed, 01 Apr 2020 05:02:55 GMT
COPY multi:07fbadbda22b19b1f9b8cfc5e833b697afbaa1e602ffea77b26286f5899f86d6 in /usr/src/nextcloud/config/ 
# Wed, 01 Apr 2020 05:02:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Apr 2020 05:02:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221e0c8c991c3fdd8db1ec76c1a911aa0f946325ec2cf15d22a25693accc6edc`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.2 MB (1227325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeaee6722c9e078934e8f34fe0dc55d3f3c28d742e92ce6b3e86775beaeeb44`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84528978bcc1c0fe1d795bbe412f0a4123fa9119c11c98cd9b1ab8c5db8203f0`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eda6e0d34e828ce8e8dd9efb0c2272f1addf00e813d5faa0e250ac1e56b726a`  
		Last Modified: Tue, 24 Mar 2020 02:08:51 GMT  
		Size: 12.1 MB (12133369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581fd0df565dfdf9fa030d939cc5438a85b6a1aadd9cfb8e17f0cffd8d78a000`  
		Last Modified: Tue, 24 Mar 2020 02:08:47 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f838a6efa2443ba97bb2214f15dc321f29394c259618e664c272cd1e3e8738`  
		Last Modified: Tue, 24 Mar 2020 02:08:51 GMT  
		Size: 12.6 MB (12563182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87befac5eace204a0f989da42597e3ed787680fa956a946afec52808fe9d55a6`  
		Last Modified: Tue, 24 Mar 2020 02:08:48 GMT  
		Size: 2.2 KB (2213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24bc33b4319ab2bdff433bcfc1ebce2a3464819a641eee06e19dd6e50c2dec5`  
		Last Modified: Tue, 24 Mar 2020 02:08:48 GMT  
		Size: 16.9 KB (16865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb66b93ceaaf184b0f0be65fcb63eb8ab5f305046ef5216110e140c4b53d6a`  
		Last Modified: Tue, 24 Mar 2020 02:08:48 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb70d39fb645199f11a87f1fdc1b84b18bb55707db2ff29974d73b0d4a4cddc1`  
		Last Modified: Tue, 24 Mar 2020 04:05:22 GMT  
		Size: 243.1 KB (243093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f2098c895df9b44b9192a93917b112f2fdaa1ae9bc75d02f7ee15939c108e5`  
		Last Modified: Tue, 24 Mar 2020 04:05:26 GMT  
		Size: 24.1 MB (24138014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f558cac800575d3ecf32cacd6eb737cd3fad8f46da7754fcca52e9bbfa21e5`  
		Last Modified: Tue, 24 Mar 2020 04:05:20 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4c9c53499e3f222bc5339f4656c1037212a59cf958548934e94ea012b9968e`  
		Last Modified: Tue, 24 Mar 2020 04:05:44 GMT  
		Size: 68.6 MB (68598162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed284901cd2f04e25c5bf4efbe4b608e4591fa16c71fb9552d1fb051b37edf`  
		Last Modified: Wed, 01 Apr 2020 05:28:02 GMT  
		Size: 2.5 KB (2508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7edf4f8e47c7da0d414e9f8e22ebf396b232084c8a42ad2dc47adc192e24f2`  
		Last Modified: Wed, 01 Apr 2020 05:28:02 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:16-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:f887290fff6dbd4a6ee4a9ebb010f7cd4b025f878a9dddb21590fb679ee2639a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124723964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a022efcf5133c881ffd49d11300e5d6bcb5c22c2fd001c6fdeb769fe377cb0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:21 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:31:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:31:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:31:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:31:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 00:43:23 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 00:43:23 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 00:43:25 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 00:43:26 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 00:43:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 00:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:46:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 00:46:28 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:46:31 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 00:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 00:46:32 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 00:46:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 00:46:35 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 00:46:36 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 00:46:36 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 06:59:20 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/15 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 24 Mar 2020 07:02:36 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Tue, 24 Mar 2020 07:02:39 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 24 Mar 2020 07:02:39 GMT
VOLUME [/var/www/html]
# Tue, 24 Mar 2020 07:02:40 GMT
ENV NEXTCLOUD_VERSION=16.0.9
# Tue, 24 Mar 2020 07:03:11 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Wed, 01 Apr 2020 05:32:04 GMT
COPY multi:7ff9cff24b6270b00f83a8bfd2c1c1229276cb451cd1a6bd1ec44ef5d1270ba6 in / 
# Wed, 01 Apr 2020 05:32:06 GMT
COPY multi:07fbadbda22b19b1f9b8cfc5e833b697afbaa1e602ffea77b26286f5899f86d6 in /usr/src/nextcloud/config/ 
# Wed, 01 Apr 2020 05:32:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Apr 2020 05:32:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee501176ea6c9d16dc12649d7c62f4b6466cc96eaf80bfcea3aa261a052ec099`  
		Last Modified: Tue, 24 Mar 2020 01:03:05 GMT  
		Size: 1.4 MB (1359430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876007701d95df62eb874f76916e4d139709812e5e0be471c4107729808d6af`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ed02bd016dcfb57e62d938f46a81237af426353ef7df647b64c3b3a93276a7`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2cc8840affcbe1779c1af710215aa419bd5623de8e3ce5a27f7812e5bd6f5b`  
		Last Modified: Tue, 24 Mar 2020 01:04:37 GMT  
		Size: 12.1 MB (12133363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc407b68bcf3dd2fd76e069843663d462611cfadc74467b1535df447a95b0e55`  
		Last Modified: Tue, 24 Mar 2020 01:04:33 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab01b4a37f1f8a9b9f356d82f8ee3ee9205b0acce0a23e213e4838eb580060c`  
		Last Modified: Tue, 24 Mar 2020 01:04:39 GMT  
		Size: 14.2 MB (14200626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1063d773aa59567942be63285eb6f4b4ab0b9559ba0ecd953c8cfa77e91f2e30`  
		Last Modified: Tue, 24 Mar 2020 01:04:33 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89b212938840b5a387f36fa9338b4ef45391c796a35993ef22d2016112377e`  
		Last Modified: Tue, 24 Mar 2020 01:04:33 GMT  
		Size: 16.9 KB (16892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4f70c5290d7f704641b7581a0b95a9d6959c50247ad72bc3c91f7d686b5394`  
		Last Modified: Tue, 24 Mar 2020 01:04:34 GMT  
		Size: 8.4 KB (8410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc0a04055e338ef06964be93599a042b67dc3e2fa68d600fc1bc8377e3b5f7`  
		Last Modified: Tue, 24 Mar 2020 07:09:29 GMT  
		Size: 269.0 KB (269007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff1d04df282e8637f814b2f28a7a6cb03a02c6d372aef4482f535f049ad833`  
		Last Modified: Tue, 24 Mar 2020 07:09:35 GMT  
		Size: 25.4 MB (25406592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3596fd8c7716400486f5aa5867b6e08730e1de4fb16b8df14b7c8c43ef6f43cc`  
		Last Modified: Tue, 24 Mar 2020 07:09:28 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483a53d7c4ef2d343d35840b616520c5fdc140a1f35a3a343241f885052fce81`  
		Last Modified: Tue, 24 Mar 2020 07:09:48 GMT  
		Size: 68.6 MB (68598109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd892e724fad17ff4532ed5d1133babddc752c3651cbe1a1d8bd8ac444ecf2df`  
		Last Modified: Wed, 01 Apr 2020 05:54:39 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce2bdf73308d6ab69696968316bb6639370ecb6dfaad4dc9c0b6f89938c38d0`  
		Last Modified: Wed, 01 Apr 2020 05:54:39 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:16-fpm-alpine` - linux; 386

```console
$ docker pull nextcloud@sha256:85e16754c0d146b7a69b4c70a9a777ea62244eefd1229cddff757be64afb6225
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126176142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fe39b9666a461caec58dcdff8f4e824c9d8af63ede56b33e736420186b8cba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:43:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 02:43:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 02:43:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 02:43:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 02:43:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:51:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 03:17:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 03:17:12 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 03:17:12 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 03:17:12 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 03:17:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 03:17:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 03:26:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 03:26:20 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 03:26:21 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 03:26:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 03:26:22 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 03:26:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 03:26:23 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 03:26:23 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 03:26:23 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 06:26:14 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/15 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 24 Mar 2020 06:28:23 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Tue, 24 Mar 2020 06:28:24 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 24 Mar 2020 06:28:24 GMT
VOLUME [/var/www/html]
# Tue, 24 Mar 2020 06:28:25 GMT
ENV NEXTCLOUD_VERSION=16.0.9
# Tue, 24 Mar 2020 06:28:46 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 31 Mar 2020 23:16:23 GMT
COPY multi:7ff9cff24b6270b00f83a8bfd2c1c1229276cb451cd1a6bd1ec44ef5d1270ba6 in / 
# Tue, 31 Mar 2020 23:16:23 GMT
COPY multi:07fbadbda22b19b1f9b8cfc5e833b697afbaa1e602ffea77b26286f5899f86d6 in /usr/src/nextcloud/config/ 
# Tue, 31 Mar 2020 23:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Mar 2020 23:16:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8addccc9b68d6aad59a5f93e0ca1813c5d09a0c7943108d860d8c29f6bebdb5`  
		Last Modified: Tue, 24 Mar 2020 04:03:48 GMT  
		Size: 1.5 MB (1452601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb273244de1495dfb0044080245a9fa0c6f3d8a2ab5f30610237d9a76e66cd4`  
		Last Modified: Tue, 24 Mar 2020 04:03:47 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d6dffa3f09145ac45428f87b062a4603137dadcaa84454812f81f70b71ea07`  
		Last Modified: Tue, 24 Mar 2020 04:03:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f3ad508c3847227ef4b82f8bbd94c5d715596ca74fd0c694964634bba1f1`  
		Last Modified: Tue, 24 Mar 2020 04:05:06 GMT  
		Size: 12.1 MB (12133357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3febefccc338737fbb1701f2246e1f21f7e82322143db1446526b5941e8ebe85`  
		Last Modified: Tue, 24 Mar 2020 04:05:03 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de25fca605611c3f18ff6a13b3eb4338c3193f22f7c5f6d3fe624fcbba32887`  
		Last Modified: Tue, 24 Mar 2020 04:05:04 GMT  
		Size: 14.8 MB (14846208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bdad805a36752f88a09a09511e586e8f9463ead868143b888385253b527203`  
		Last Modified: Tue, 24 Mar 2020 04:05:03 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9cab3415a077e903d51f58b58ef5a4c4018cf91b8bd69c2eb2f1194d2187bd`  
		Last Modified: Tue, 24 Mar 2020 04:05:03 GMT  
		Size: 16.9 KB (16889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac0e0eaa47abc944f1ec4a96f820f2bad2dbbc2a16f278851d5d983e112f1c9`  
		Last Modified: Tue, 24 Mar 2020 04:05:02 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7b75b99e96a4024eeb870fb17e0bdd4bae92b83bf1ae6437a244b39f371d9f`  
		Last Modified: Tue, 24 Mar 2020 06:33:00 GMT  
		Size: 276.9 KB (276900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e04fdfe5843731c0816caddd506f7f675f2f9b4a502c041edad3485538352d`  
		Last Modified: Tue, 24 Mar 2020 06:33:05 GMT  
		Size: 26.0 MB (26029221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f1c933434ad03ed20d11ad9e6933dcc1734b4ee222ebaac7ec6098092d1244`  
		Last Modified: Tue, 24 Mar 2020 06:32:58 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496986801f2036b403dea73d6b0f96d0b8d014c8c0e9870ac9cdbddc5d7fd693`  
		Last Modified: Tue, 24 Mar 2020 06:33:16 GMT  
		Size: 68.6 MB (68598142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf0d76a158db408eec512a2b668b1ff24150b72fd52bdc91c2ee702267b5550`  
		Last Modified: Tue, 31 Mar 2020 23:33:34 GMT  
		Size: 2.5 KB (2510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83116fbe002352c0391f94120a1569ad1803d6e2f3dda9c2e06e4a9f0d1d05f3`  
		Last Modified: Tue, 31 Mar 2020 23:33:35 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:16-fpm-alpine` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:80eb7e5561347f6034d36a0f222644ce305225ea1fb693bc4be4bae57a878d65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126781497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63a76dcb2520398c8097e9e4976d3310cfc2eb12788edc989d8cc126f78a234`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:32:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:32:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:32:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:32:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 00:47:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 00:47:51 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 00:47:54 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 00:47:57 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 00:48:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 00:48:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:52:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 00:52:17 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:52:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 00:52:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 00:52:36 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 00:52:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 00:52:50 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 00:52:56 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 00:53:01 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 04:42:55 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/15 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 24 Mar 2020 04:49:29 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Tue, 24 Mar 2020 04:49:37 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 24 Mar 2020 04:49:39 GMT
VOLUME [/var/www/html]
# Tue, 24 Mar 2020 04:49:43 GMT
ENV NEXTCLOUD_VERSION=16.0.9
# Tue, 24 Mar 2020 04:50:35 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm -r "$GNUPGHOME" nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Wed, 01 Apr 2020 07:00:28 GMT
COPY multi:7ff9cff24b6270b00f83a8bfd2c1c1229276cb451cd1a6bd1ec44ef5d1270ba6 in / 
# Wed, 01 Apr 2020 07:00:31 GMT
COPY multi:07fbadbda22b19b1f9b8cfc5e833b697afbaa1e602ffea77b26286f5899f86d6 in /usr/src/nextcloud/config/ 
# Wed, 01 Apr 2020 07:00:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Apr 2020 07:00:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681c4a6dbdeb5b4877c85db3edbb08e40a877342795a3e7ba7f543a65586c417`  
		Last Modified: Tue, 24 Mar 2020 01:16:24 GMT  
		Size: 1.4 MB (1397873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e23455f025d83291061d4165e722b934e986f58c2b3d71b62a0918166d19db`  
		Last Modified: Tue, 24 Mar 2020 01:16:23 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c3447d90e80a01a72c494bf3563b1379704fcf4fb8b5b207596bbeeac49fc3`  
		Last Modified: Tue, 24 Mar 2020 01:16:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc254a86c9277744e5d5921909889f235e10113bc35de89f269763623419a2c7`  
		Last Modified: Tue, 24 Mar 2020 01:18:50 GMT  
		Size: 12.1 MB (12133377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98942a1122c3eeb1e146b0d5e1292cc308a99df4a2bbef470291b4073d86bc9`  
		Last Modified: Tue, 24 Mar 2020 01:18:46 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f171cdde581ebda3a09092fee88c92865e75df5fe91fa15059f313c520f1c4f6`  
		Last Modified: Tue, 24 Mar 2020 01:18:50 GMT  
		Size: 15.5 MB (15483479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7f27b32f8500e4ec3ba7bf8a7b9d962ead0df603de44068135df4d959a0aac`  
		Last Modified: Tue, 24 Mar 2020 01:18:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaf87e529908aa18bf53d65009afdea973db887e28144ce1221ec5aa70bf7be`  
		Last Modified: Tue, 24 Mar 2020 01:18:45 GMT  
		Size: 16.9 KB (16876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a188be6bc76b4405243d376fc5a21e7065e1988fcafcf0d77d061666431726`  
		Last Modified: Tue, 24 Mar 2020 01:18:45 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f039b182e93bac53db7e22ff601c84006823458fb9090d9d3bc500056808b0`  
		Last Modified: Tue, 24 Mar 2020 04:58:44 GMT  
		Size: 274.3 KB (274290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7b1136c6124ee2d5c27f8697ac68617bec7710f8acf17c34c18559eea714fd`  
		Last Modified: Tue, 24 Mar 2020 04:58:46 GMT  
		Size: 26.0 MB (26040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423ee9d9c5e4990dadce8bcca367de828de20911804d6bc361063ea5f2fef6ae`  
		Last Modified: Tue, 24 Mar 2020 04:58:40 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f639294aa7477f30ec5333e87dd40f69386111c55e7c20ffe2a98a8ac384c`  
		Last Modified: Tue, 24 Mar 2020 04:58:55 GMT  
		Size: 68.6 MB (68597985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0fc97ea47b598116fee5b1794dfaa133cb2a084a87c18f4404be47e2b08238`  
		Last Modified: Wed, 01 Apr 2020 08:06:28 GMT  
		Size: 2.5 KB (2509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48db5eb1aea69bbee817c37085c1e1d8d333dd86d5d746eafc2c98da63f2cce`  
		Last Modified: Wed, 01 Apr 2020 08:06:27 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
