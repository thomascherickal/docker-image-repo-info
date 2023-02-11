## `nextcloud:production-fpm-alpine`

```console
$ docker pull nextcloud@sha256:4fcbd6e369cc87974cedfbc86f655e7a452e30ec0cdb763f5bdf9f19e63b6c53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nextcloud:production-fpm-alpine` - linux; amd64

```console
$ docker pull nextcloud@sha256:dd1731b5e7edaa097faf288761b0a6002c2539ff3d116741dddedc8a17541d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.3 MB (251275446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60010f4ed25b23fcba3a303eef6fa353b3ed5f41e595e588705ece5d50bfc4a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:28:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 10:28:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 10:28:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 10:28:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 10:28:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 10:28:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:28:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:28:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 10:52:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 11 Feb 2023 10:52:24 GMT
ENV PHP_VERSION=8.1.15
# Sat, 11 Feb 2023 10:52:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Sat, 11 Feb 2023 10:52:24 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Sat, 11 Feb 2023 10:52:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 11 Feb 2023 10:52:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 11 Feb 2023 11:00:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 11 Feb 2023 11:00:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 11 Feb 2023 11:00:24 GMT
RUN docker-php-ext-enable sodium
# Sat, 11 Feb 2023 11:00:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 11 Feb 2023 11:00:24 GMT
WORKDIR /var/www/html
# Sat, 11 Feb 2023 11:00:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 11 Feb 2023 11:00:25 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 11:00:25 GMT
EXPOSE 9000
# Sat, 11 Feb 2023 11:00:25 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 16:26:40 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 16:29:17 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 16:29:17 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 16:29:17 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 16:29:18 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 16:29:18 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 16:29:18 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 16:30:07 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 16:30:09 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 16:30:10 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 16:30:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 16:30:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd032c1d9bc64fb28abb14a4f1f7ba3b82f201fe308eb5cb5f9a25ef1c0b524`  
		Last Modified: Sat, 11 Feb 2023 11:21:33 GMT  
		Size: 1.7 MB (1721195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be86720d648286af3b185a53ce7968d957f0370224f1ecbfbe38dc2ab06c6647`  
		Last Modified: Sat, 11 Feb 2023 11:21:33 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03010434aa246ad0ecbd25429ffe16a52c424f962893504bc1303a6e13f33cf8`  
		Last Modified: Sat, 11 Feb 2023 11:21:32 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a183969756c9bd992c1a58619ca7835357c52d0d80fbd719327fa3caa8b06c0c`  
		Last Modified: Sat, 11 Feb 2023 11:23:36 GMT  
		Size: 11.8 MB (11834618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e72bfebf7be190ad1ca2b4b6afd9408ac9031804b5067aa1764798f171adb4`  
		Last Modified: Sat, 11 Feb 2023 11:23:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876873e66e5821a0128b737e7e95f1a6ed4e36a3e5d6bd03106cba1bc0b22d03`  
		Last Modified: Sat, 11 Feb 2023 11:23:53 GMT  
		Size: 12.4 MB (12389311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9120a3e9e05b81f22a780d463b65cff8ffc5d0a83e4d49a69c35a45aced62f03`  
		Last Modified: Sat, 11 Feb 2023 11:23:51 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca6bfa0e951920b3e8e379f93ab4fcbc7a0c15efd71d604263699eb9ad824a`  
		Last Modified: Sat, 11 Feb 2023 11:23:51 GMT  
		Size: 18.9 KB (18881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1172e03e646f0dab33956dfbcacc75472db8bbe7d8fb0f20c89bade5709015c6`  
		Last Modified: Sat, 11 Feb 2023 11:23:51 GMT  
		Size: 8.8 KB (8846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c5704a49a530e52a27c68ca1a80c41d32ae6210f10297815fa7c6f3ebba2f`  
		Last Modified: Sat, 11 Feb 2023 16:32:24 GMT  
		Size: 47.4 MB (47443376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2bae5f53aa08a56e958e3f09eff6a73a8e7ea46ce8fb9bdd9572b192551ea2`  
		Last Modified: Sat, 11 Feb 2023 16:32:16 GMT  
		Size: 9.4 MB (9382854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f95a28b3479c468d9fcbb3d00ceabb41b73f67218419a6f1183ce5ca121626e`  
		Last Modified: Sat, 11 Feb 2023 16:32:14 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117cf4e6c1d6c5670a27cb126ea580467cdc88b5fcd03a95d31ed1a03c33df25`  
		Last Modified: Sat, 11 Feb 2023 16:32:36 GMT  
		Size: 165.7 MB (165658148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f5dbcf7d49ae0b16584ad31a6240fbc47a44d6c203abc7cdd950a1fc72d51`  
		Last Modified: Sat, 11 Feb 2023 16:32:14 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b8573d6deec60e8146d97ca8c2863cf62ab6f4dd1c730de9aae5c7da8cdeea`  
		Last Modified: Sat, 11 Feb 2023 16:32:14 GMT  
		Size: 2.1 KB (2150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; arm variant v6

```console
$ docker pull nextcloud@sha256:778ac65b7cbd92b2fd2610581339ad1b653911f9f7f5787330483643ea959da3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244517597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfdcd30b4fff666108755bd98f9c27de67466b9035bfd5cc2dfccfb2faa22d1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:43:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 02:43:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 02:43:55 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 02:43:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 02:43:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 02:43:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:43:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:43:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 03:04:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 11 Feb 2023 03:04:10 GMT
ENV PHP_VERSION=8.1.15
# Sat, 11 Feb 2023 03:04:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Sat, 11 Feb 2023 03:04:10 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Sat, 11 Feb 2023 03:04:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 11 Feb 2023 03:04:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:10:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 11 Feb 2023 03:10:48 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:10:49 GMT
RUN docker-php-ext-enable sodium
# Sat, 11 Feb 2023 03:10:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 11 Feb 2023 03:10:49 GMT
WORKDIR /var/www/html
# Sat, 11 Feb 2023 03:10:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 11 Feb 2023 03:10:50 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 03:10:50 GMT
EXPOSE 9000
# Sat, 11 Feb 2023 03:10:50 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 09:29:03 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 09:32:37 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 09:32:37 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 09:32:38 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 09:32:40 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 09:32:40 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 09:32:40 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 09:33:45 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 09:33:49 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 09:33:50 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 09:33:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 09:33:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98d69a3110bbb146208acf32322ca523d3a7a82fb1ebec13bdf1c11663752c2`  
		Last Modified: Sat, 11 Feb 2023 03:30:33 GMT  
		Size: 1.7 MB (1708058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e2ec151523e8e0f68ed68cfe154dcb6f507c51d9d2e2802be7f2b1ad7bb63`  
		Last Modified: Sat, 11 Feb 2023 03:30:33 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cd7f6075d4f0919fd580be939f1c9c3c4192315cf366ca66cfd32d2e8b0adb`  
		Last Modified: Sat, 11 Feb 2023 03:30:33 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caea812b6074566d4eee371dc21bcbd4bca7c15e834f3bf516a3cfd8184a15b1`  
		Last Modified: Sat, 11 Feb 2023 03:33:01 GMT  
		Size: 11.8 MB (11834575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8899df8405313ee970120a78001d88a9aef2a89110d7f831a226cd6e6dfa6c6`  
		Last Modified: Sat, 11 Feb 2023 03:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809f0a6baaea6b26750cbd6deaf37851c54beac399188788f5b4ef0f6aa1bfb6`  
		Last Modified: Sat, 11 Feb 2023 03:33:23 GMT  
		Size: 11.2 MB (11248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a5c48a776c6dd4340c00069f090ae86da790ddf6900b934a4ab8a9377221fc`  
		Last Modified: Sat, 11 Feb 2023 03:33:20 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704628cd663177d524275d9af4f497e65838a9d74e1af3ead4859f69d8735ffd`  
		Last Modified: Sat, 11 Feb 2023 03:33:21 GMT  
		Size: 18.7 KB (18674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4671a223ca86d1c0e3b37ce815843379a08ecc46e788393a0e28fbc9ef6e8d`  
		Last Modified: Sat, 11 Feb 2023 03:33:21 GMT  
		Size: 8.8 KB (8844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04be27bb242cc0129e863f61fc2fe978d7faa28b1f99d5fa49cc7db0cf30034`  
		Last Modified: Sat, 11 Feb 2023 09:36:34 GMT  
		Size: 43.1 MB (43076252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ada9bc097d4953f544d00a1fbbdc1b982253b0124851b2bc2600c5d648d2a78`  
		Last Modified: Sat, 11 Feb 2023 09:36:23 GMT  
		Size: 8.3 MB (8337949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb0670611f1ac3c91deaabe381e6557b59fba102faceec97930bcd0824b6bad`  
		Last Modified: Sat, 11 Feb 2023 09:36:21 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2063feabec2125f83fae818946b70bd88b7384f2c1c8def47506903623f2db`  
		Last Modified: Sat, 11 Feb 2023 09:36:59 GMT  
		Size: 165.7 MB (165657462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9429023a455bf5d618bc268421283b86499a35a17629ffd51448367acceed91e`  
		Last Modified: Sat, 11 Feb 2023 09:36:21 GMT  
		Size: 3.2 KB (3241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0485db8d0330fe1fe8e01b5aed3c4ba9c3da88290894705a30be1d633f98ff8`  
		Last Modified: Sat, 11 Feb 2023 09:36:20 GMT  
		Size: 2.1 KB (2149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:10e6ac88974d507a78c7219647bd50bcff6500c1a0c97d88aad675e9cad0f908
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.5 MB (241478925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff632eb5d0d77bf42101fb6572d15e2c966390ed751ff54b0eb97c9ac7cb11d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:06:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 07:06:17 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 07:06:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 07:06:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 07:06:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 07:06:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 07:06:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 07:06:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 07:29:11 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 11 Feb 2023 07:29:11 GMT
ENV PHP_VERSION=8.1.15
# Sat, 11 Feb 2023 07:29:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Sat, 11 Feb 2023 07:29:11 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Sat, 11 Feb 2023 07:29:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 11 Feb 2023 07:29:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:35:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 11 Feb 2023 07:35:50 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:35:51 GMT
RUN docker-php-ext-enable sodium
# Sat, 11 Feb 2023 07:35:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 11 Feb 2023 07:35:51 GMT
WORKDIR /var/www/html
# Sat, 11 Feb 2023 07:35:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 11 Feb 2023 07:35:52 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 07:35:52 GMT
EXPOSE 9000
# Sat, 11 Feb 2023 07:35:52 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 14:13:01 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 14:15:22 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 14:15:22 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 14:15:22 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 14:15:23 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 14:15:23 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 14:15:23 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 14:16:11 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 14:16:12 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 14:16:13 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 14:16:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:16:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaded23bd6949b10651a5c2d72b03222676156780db34e7ffdf0575d7d7869d`  
		Last Modified: Sat, 11 Feb 2023 08:03:21 GMT  
		Size: 1.6 MB (1575433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1542053bf918c55b2d36423810bf4cbf98597767110f87da4072ce927952009`  
		Last Modified: Sat, 11 Feb 2023 08:03:21 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1e3c97c206260f8ea1f680dbad690a61e75f238c938e6b9970737e708ad794`  
		Last Modified: Sat, 11 Feb 2023 08:03:21 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5beb1a397d14131c480726c60c86aaf835756cd93d64177ecdcf43efe044ab`  
		Last Modified: Sat, 11 Feb 2023 08:06:13 GMT  
		Size: 11.8 MB (11834586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0294f686fc538517d1486f5a71a5671c09bfb1def26229ac3049c7959d2ca07`  
		Last Modified: Sat, 11 Feb 2023 08:06:12 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809792a2f79121d453f23c869d3b1c8a6416b50a605a94697e00994fac26f6b0`  
		Last Modified: Sat, 11 Feb 2023 08:06:34 GMT  
		Size: 10.6 MB (10561841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9118a03e72060883849df74e1265b63e6e932145ef87d7274d629e725b4bf39e`  
		Last Modified: Sat, 11 Feb 2023 08:06:32 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cfde24dc8e7592c06e608856716491ce3a6ee7c8c74a4486d2f95177380b53`  
		Last Modified: Sat, 11 Feb 2023 08:06:32 GMT  
		Size: 18.6 KB (18648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e69bda7008f48695bc0a3b317ecad7bab4c59071ec0fa8e5d240db8dad878`  
		Last Modified: Sat, 11 Feb 2023 08:06:32 GMT  
		Size: 8.8 KB (8845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ed433140e2ac07180c84371929525c2aa9e0e66bd37d9f0c5b2a9693e0fee3`  
		Last Modified: Sat, 11 Feb 2023 14:20:30 GMT  
		Size: 41.1 MB (41052921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b3869f37e1cc18affdc4fbe8cd45d9215d7b2dc0640a26da46f623d74c346a`  
		Last Modified: Sat, 11 Feb 2023 14:20:22 GMT  
		Size: 8.3 MB (8338730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a196bc20c4eb0d21fd6f9b7fc6bf9a93135adb4c2d14992f1f9038e269722a73`  
		Last Modified: Sat, 11 Feb 2023 14:20:21 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36185efc7b18e0647d57858fc89d67488603424d26a584bbb4c98751aa0d02e`  
		Last Modified: Sat, 11 Feb 2023 14:20:52 GMT  
		Size: 165.7 MB (165657085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73ee01bcc5267f370f8c510bf9fb5653fcc2ecf4c51b1bd962b82c0585a4448`  
		Last Modified: Sat, 11 Feb 2023 14:20:21 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200666816c20a66c708c5ce6846e1a74a0f4ee76383410ea8ac3266186f9d93a`  
		Last Modified: Sat, 11 Feb 2023 14:20:22 GMT  
		Size: 2.1 KB (2149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:ad0dd306d2b40764fe900c1afe7a5920ae3cd6cc8060f65c8f1a5b45c3dacb78
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249872779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5660558e4619684cfb6778d590ddd8ff2a60090346157e6fab3b9a9632188e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:14:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 02:14:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 02:14:05 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 02:14:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 02:14:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 02:14:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:14:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:14:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 02:37:50 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 11 Feb 2023 02:37:50 GMT
ENV PHP_VERSION=8.1.15
# Sat, 11 Feb 2023 02:37:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Sat, 11 Feb 2023 02:37:50 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Sat, 11 Feb 2023 02:37:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 11 Feb 2023 02:37:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 11 Feb 2023 02:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 11 Feb 2023 02:45:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 11 Feb 2023 02:45:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 11 Feb 2023 02:45:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 11 Feb 2023 02:45:54 GMT
WORKDIR /var/www/html
# Sat, 11 Feb 2023 02:45:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 11 Feb 2023 02:45:55 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 02:45:55 GMT
EXPOSE 9000
# Sat, 11 Feb 2023 02:45:55 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 08:00:21 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 08:03:14 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 08:03:14 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 08:03:14 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 08:03:15 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 08:03:15 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 08:03:15 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 08:03:58 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 08:04:02 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 08:04:02 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 08:04:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 08:04:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24945052da1277802c9acdaf867899c620d73633d9ffdb9141894016d23502a8`  
		Last Modified: Sat, 11 Feb 2023 03:03:59 GMT  
		Size: 1.7 MB (1715610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aab80b0b76f2ca115ba0bf03f9e94151c3b730634d2d9e928f9cda792e65966`  
		Last Modified: Sat, 11 Feb 2023 03:03:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b2459980e300f1a871481cd0f9ef1a474248c2a36c1a7cad8928a45283a0fa`  
		Last Modified: Sat, 11 Feb 2023 03:03:58 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e664129d76bf3d40c568e00cb95273222672a49354d1699b67dd726e04cd5`  
		Last Modified: Sat, 11 Feb 2023 03:06:02 GMT  
		Size: 11.8 MB (11834622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9b2f5a532bda64990dc6143dbb64a640420f65c5ba317641dbaac8714a3a70`  
		Last Modified: Sat, 11 Feb 2023 03:06:01 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53117935469cc45eb611b813e149314bb8a15ecaeadb03de9e364083037e3e34`  
		Last Modified: Sat, 11 Feb 2023 03:06:23 GMT  
		Size: 12.4 MB (12436069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5802be1770d1ee34edc6637952a9490b90aff56cce3be147ae7ad6f408d73d`  
		Last Modified: Sat, 11 Feb 2023 03:06:22 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf51ba8e234b4498de7bdf4b4054e98ece478b3265c0d3006af75c4edb845be`  
		Last Modified: Sat, 11 Feb 2023 03:06:22 GMT  
		Size: 18.7 KB (18670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ec995badbf5da1d0dbe458bc937ef4a87773d9a8bd172b2f27f56a76250b7`  
		Last Modified: Sat, 11 Feb 2023 03:06:22 GMT  
		Size: 8.8 KB (8843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084288884ba9fb7437f450e4ab4fe477f3993d8c040bfd8c84cedffa14714401`  
		Last Modified: Sat, 11 Feb 2023 08:06:12 GMT  
		Size: 45.9 MB (45893599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81339cbf23738b0e9b8f0c6ef34fad32ec5e329972caed0dc268ea41cbbd6407`  
		Last Modified: Sat, 11 Feb 2023 08:06:06 GMT  
		Size: 9.6 MB (9587870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f601821bd3a3a3a675fae2d7f72f43e3375f236b05e43ca6facba42d10c114bb`  
		Last Modified: Sat, 11 Feb 2023 08:06:05 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f0afd9f4c11ba665618252a612ced3cb60f39c233edfd045546d3e7e8d859e`  
		Last Modified: Sat, 11 Feb 2023 08:06:23 GMT  
		Size: 165.7 MB (165657543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca6864390e60f651375968a6caee7262976b9a81c11765865fdf31f232ae65`  
		Last Modified: Sat, 11 Feb 2023 08:06:05 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c2f50ef70dfdb4da3e19cad6dc337dafd2eafcc8e5999097cbc87b4857b738`  
		Last Modified: Sat, 11 Feb 2023 08:06:05 GMT  
		Size: 2.1 KB (2150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; 386

```console
$ docker pull nextcloud@sha256:aaacc6ac8f3589dbb533d1ade44d3c11d1c6e61bc9b1b120914b48acdbf758b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250306991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b1dced67f41270b058912c7d4fc91a80f4caed8010f9351dbad13d7b6371869`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:29 GMT
ADD file:59ac1f8f33f9b9727892b7e45b33f54ef3c20d9d876c49d6a4c057641821d68f in / 
# Fri, 10 Feb 2023 21:24:29 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:15:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 10 Feb 2023 23:15:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 10 Feb 2023 23:15:45 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 23:15:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 10 Feb 2023 23:15:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 10 Feb 2023 23:15:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:15:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:15:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 10 Feb 2023 23:39:44 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 10 Feb 2023 23:39:45 GMT
ENV PHP_VERSION=8.1.15
# Fri, 10 Feb 2023 23:39:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Fri, 10 Feb 2023 23:39:47 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Fri, 10 Feb 2023 23:39:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 10 Feb 2023 23:39:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Feb 2023 23:48:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Feb 2023 23:48:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 10 Feb 2023 23:48:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Feb 2023 23:48:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Feb 2023 23:48:11 GMT
WORKDIR /var/www/html
# Fri, 10 Feb 2023 23:48:12 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 10 Feb 2023 23:48:13 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 23:48:14 GMT
EXPOSE 9000
# Fri, 10 Feb 2023 23:48:15 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 05:17:49 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 05:20:29 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 05:20:29 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 05:20:30 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 05:20:31 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 05:20:32 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 05:20:33 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 05:21:29 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 05:21:30 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 05:21:32 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 05:21:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 05:21:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0987f51cd58a7d03bc7d6ff0a3a0a843c1a3fefcd41e3c8adc3999ddde7441e8`  
		Last Modified: Fri, 10 Feb 2023 21:25:30 GMT  
		Size: 2.8 MB (2810653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62122267ef44a612330b6b1a4a8c97503160a6be006e9379c086fb229519dbc2`  
		Last Modified: Sat, 11 Feb 2023 00:14:28 GMT  
		Size: 1.8 MB (1820370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df37a1ab16734bdad148cabca0143c434769c7b6b386dee1ee9e9ddd57a94e2`  
		Last Modified: Sat, 11 Feb 2023 00:14:27 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b27bfe2f160f32b567c2dbf1cd11c7f543e7b03e63a1bc64a7074bff11ad54`  
		Last Modified: Sat, 11 Feb 2023 00:14:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b03605d66ea7adab1702b528d5c12c8a0f9df458364000e5e94d63339f749`  
		Last Modified: Sat, 11 Feb 2023 00:17:05 GMT  
		Size: 11.8 MB (11834420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d964a21cd6283a88e36978e41c28d2715c43a7a670be666ee9573a09a8163a`  
		Last Modified: Sat, 11 Feb 2023 00:17:04 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a459db94214157111d2cf866fcea15482bd17a07c6dcd3535b9c1a9398cd7b`  
		Last Modified: Sat, 11 Feb 2023 00:17:25 GMT  
		Size: 12.7 MB (12683709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0431baf157baad25e747c94e36eacf056a687877cf5d94cae29d0cc4955d0f`  
		Last Modified: Sat, 11 Feb 2023 00:17:23 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c545a4d27aea33b2653e8edf45c31eba6445c958ba3e986f739613d3249f5563`  
		Last Modified: Sat, 11 Feb 2023 00:17:23 GMT  
		Size: 18.8 KB (18776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4ab914b49c2a17932ab83f09139ed8d932462ddde842bcfd80cb3b48d731ea`  
		Last Modified: Sat, 11 Feb 2023 00:17:23 GMT  
		Size: 8.8 KB (8849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e21c4ba9c61cc0fcab9fd3069218e136f97fa2def5acc632a953b658fa0a0b9`  
		Last Modified: Sat, 11 Feb 2023 05:24:54 GMT  
		Size: 46.0 MB (45989132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bb864214a46cc29c7dedfd37e7ce75d858a6047503850c4bc075baccf52016`  
		Last Modified: Sat, 11 Feb 2023 05:24:47 GMT  
		Size: 9.5 MB (9480510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b64320f658735345201db995a17dd0741897e1e25f4b356e7c4ae0858bcbca`  
		Last Modified: Sat, 11 Feb 2023 05:24:45 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc668bf6bf4cf2a1c54001829a9706294def562e000de5c56f997d6b79ecb90`  
		Last Modified: Sat, 11 Feb 2023 05:25:07 GMT  
		Size: 165.7 MB (165650220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638b9ab8f7527bef99b02366189552b6efe80be0b7f8b14dc4ce39c255d5d687`  
		Last Modified: Sat, 11 Feb 2023 05:24:45 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667aff0de6b819f834568e6ba32be2695207d2ea4d36a2439cc2e6666627745a`  
		Last Modified: Sat, 11 Feb 2023 05:24:45 GMT  
		Size: 2.2 KB (2151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:3537d9ba2eb2a3e4cf73345d0edb2c3040a45fb694ddbf99778aed00956c2674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.6 MB (256628098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bba90a8d1e833a5ddae12472d68f10776363ac040d080878c9732b44f9698fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:21:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 10 Feb 2023 23:21:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 10 Feb 2023 23:21:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 23:21:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 10 Feb 2023 23:21:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 10 Feb 2023 23:21:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:21:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:21:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 10 Feb 2023 23:50:07 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 10 Feb 2023 23:50:08 GMT
ENV PHP_VERSION=8.1.15
# Fri, 10 Feb 2023 23:50:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Fri, 10 Feb 2023 23:50:08 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Fri, 10 Feb 2023 23:50:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 10 Feb 2023 23:50:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 11 Feb 2023 00:00:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 11 Feb 2023 00:00:29 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 11 Feb 2023 00:00:31 GMT
RUN docker-php-ext-enable sodium
# Sat, 11 Feb 2023 00:00:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 11 Feb 2023 00:00:32 GMT
WORKDIR /var/www/html
# Sat, 11 Feb 2023 00:00:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 11 Feb 2023 00:00:34 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 00:00:34 GMT
EXPOSE 9000
# Sat, 11 Feb 2023 00:00:35 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 11:40:58 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 11:44:57 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 11:44:58 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 11:44:59 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 11:45:00 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 11:45:01 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 11:45:01 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 11:46:01 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 11:46:10 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 11:46:12 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 11:46:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 11:46:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77483b79fe489e3d1e457273e36c12fdbbfda2b9134aa1ed6c809edb4bc207c9`  
		Last Modified: Sat, 11 Feb 2023 00:30:19 GMT  
		Size: 1.8 MB (1772435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa4d9c93206a48a73541502538d2448b50970846318272100e6410859ee40e1`  
		Last Modified: Sat, 11 Feb 2023 00:30:19 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44eb343fe0eefc0c427b565973e982dbcf3c0991674564b7317125e6dbcaf69e`  
		Last Modified: Sat, 11 Feb 2023 00:30:19 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468610c0b55d2e3d8cc7df9796241b5fdd2450912bd56e516c1b36217cfd6787`  
		Last Modified: Sat, 11 Feb 2023 00:33:11 GMT  
		Size: 11.8 MB (11834591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b3b6006166a68fa02d3f82ce90a3b1fbfa091fd9fe23f4e71911a7504ce744`  
		Last Modified: Sat, 11 Feb 2023 00:33:10 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed7b0b5210cff5a390a5249ec7b47c4220083388af2cf95282029ba2c6df409`  
		Last Modified: Sat, 11 Feb 2023 00:33:36 GMT  
		Size: 12.8 MB (12821259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7ec0b0a103d9bb08f822d8622630d340987d8987d4e4d0969287faf7a1b635`  
		Last Modified: Sat, 11 Feb 2023 00:33:32 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08547e649635c97eaf133a90dacace89826df384d34f504c04c64224e24cdb66`  
		Last Modified: Sat, 11 Feb 2023 00:33:32 GMT  
		Size: 18.7 KB (18660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3b0dc234dbd234fe8e676cf03ddc49e58c88c198141357eb82a1be9bc7b4c5`  
		Last Modified: Sat, 11 Feb 2023 00:33:32 GMT  
		Size: 8.8 KB (8846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c84425124ac6d7fd08ca27b253f4b362f16e61e8386473070c667dc8b15584`  
		Last Modified: Sat, 11 Feb 2023 11:50:23 GMT  
		Size: 52.5 MB (52495254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de81278dee43af7c96a616b1fcaf65471de7e77adb002b493def5d2d8b8f87ca`  
		Last Modified: Sat, 11 Feb 2023 11:50:10 GMT  
		Size: 9.2 MB (9204324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904bb8e2bb61a3305f7403ee6f9884e98bd91de5c9ba3102ae49bf7721dcaa`  
		Last Modified: Sat, 11 Feb 2023 11:50:07 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef17f0a842d9b756be5ee1ec857bddfb418b70a814f7006dbc5ac349e3861d6d`  
		Last Modified: Sat, 11 Feb 2023 11:50:46 GMT  
		Size: 165.7 MB (165657646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea5c79b64892a17cda4669c3d35d92320b6f3ba522c55601d0edab67f700aa2`  
		Last Modified: Sat, 11 Feb 2023 11:50:07 GMT  
		Size: 3.2 KB (3239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828417ce570d243386b7091f01c0d2cac6a12513fc988319e73d75f7d2f0b99c`  
		Last Modified: Sat, 11 Feb 2023 11:50:07 GMT  
		Size: 2.1 KB (2150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:production-fpm-alpine` - linux; s390x

```console
$ docker pull nextcloud@sha256:bdaa614137e30157e88d9bc0373a9f6855f50c4b8587a0c81610b1e9fdd88cb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.8 MB (239758963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6a40ee8824adb2931752401ad0ecc9b28754997ea6d35b53ce9516bee6ac860`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:49:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 03:49:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 03:49:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 03:49:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 04:09:20 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 11 Feb 2023 04:09:20 GMT
ENV PHP_VERSION=8.1.15
# Sat, 11 Feb 2023 04:09:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Sat, 11 Feb 2023 04:09:21 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Sat, 11 Feb 2023 04:09:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 11 Feb 2023 04:09:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 11 Feb 2023 04:16:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 11 Feb 2023 04:16:01 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 11 Feb 2023 04:16:02 GMT
RUN docker-php-ext-enable sodium
# Sat, 11 Feb 2023 04:16:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 11 Feb 2023 04:16:03 GMT
WORKDIR /var/www/html
# Sat, 11 Feb 2023 04:16:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 11 Feb 2023 04:16:03 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 04:16:03 GMT
EXPOSE 9000
# Sat, 11 Feb 2023 04:16:04 GMT
CMD ["php-fpm"]
# Sat, 11 Feb 2023 11:58:22 GMT
RUN set -ex;         apk add --no-cache         rsync         imagemagick     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sat, 11 Feb 2023 11:59:55 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Sat, 11 Feb 2023 11:59:56 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 11 Feb 2023 11:59:56 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 11 Feb 2023 11:59:57 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=60';     } > "${PHP_INI_DIR}/conf.d/opcache-recommended.ini";         echo 'apc.enable_cli=1' >> "${PHP_INI_DIR}/conf.d/docker-php-ext-apcu.ini";         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > "${PHP_INI_DIR}/conf.d/nextcloud.ini";         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 11 Feb 2023 11:59:57 GMT
VOLUME [/var/www/html]
# Sat, 11 Feb 2023 11:59:57 GMT
ENV NEXTCLOUD_VERSION=25.0.3
# Sat, 11 Feb 2023 12:00:35 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com  --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Sat, 11 Feb 2023 12:00:47 GMT
COPY multi:6a18c1c6e633992cb8206e6acf4353eeb6ef9c184e76ada9420c1bd01fe25af2 in / 
# Sat, 11 Feb 2023 12:00:47 GMT
COPY multi:e04ec17740bba0827b5de2ec99cdb42bece265a39b1dfe4bab140bca83af17d6 in /usr/src/nextcloud/config/ 
# Sat, 11 Feb 2023 12:00:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 12:00:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476a3a3fc00d505f146f9062bf162efa67799d1f39390acbac0a7a316be08a7c`  
		Last Modified: Sat, 11 Feb 2023 04:36:27 GMT  
		Size: 1.8 MB (1776052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548ad0a6b1dee36843d375e2a426690db3337e78377cb2d8863a1848f9439897`  
		Last Modified: Sat, 11 Feb 2023 04:36:27 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdded828c248ae0d95503cd8211f9017f84d334e34aae9ecc47b64fbb554eacb`  
		Last Modified: Sat, 11 Feb 2023 04:36:27 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500359eb67b8dfdbf8ab11bd6faa146feb777bdca174650011fb6f90e63c4137`  
		Last Modified: Sat, 11 Feb 2023 04:38:07 GMT  
		Size: 11.8 MB (11834598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ab86ba811f511a1fd7f9731207c42a5748434247d69d6fe580ceb9ab572d3`  
		Last Modified: Sat, 11 Feb 2023 04:38:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d40e39184434f4728c81f4b96c5508aa521f426d02a836f5327d0b83066937`  
		Last Modified: Sat, 11 Feb 2023 04:38:21 GMT  
		Size: 11.6 MB (11578399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aa1c440748d27124cac58bb4eff5a515869eb624c5562cee69e4dcddd576f0`  
		Last Modified: Sat, 11 Feb 2023 04:38:19 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a696c6d9403ec658905f5e0349d2cc262492e9eaf3d258d86b68c1eee30a370`  
		Last Modified: Sat, 11 Feb 2023 04:38:19 GMT  
		Size: 18.7 KB (18674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23101f86c131a0f3538d43c178f32027fa814fe571bedf8a45e82b040ac179c2`  
		Last Modified: Sat, 11 Feb 2023 04:38:19 GMT  
		Size: 8.8 KB (8844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0fc221db36cc43672ffeec2f9cd713317a38ecb00a8ad97d757c2cf1678ae4`  
		Last Modified: Sat, 11 Feb 2023 12:03:55 GMT  
		Size: 37.7 MB (37739285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459684ebca766a593c95cb91de43bf294474aa383d4ef7cf570e62abeba09ecb`  
		Last Modified: Sat, 11 Feb 2023 12:03:50 GMT  
		Size: 8.6 MB (8550111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ac81c977f658dafbc190a85344f56267273d2ea1d8dfdd0b769a87bcf9f8b4`  
		Last Modified: Sat, 11 Feb 2023 12:03:49 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4557ed178216b26b511f20e82cbfb911dd8b2dddcbfb184721fbe066e33243`  
		Last Modified: Sat, 11 Feb 2023 12:04:07 GMT  
		Size: 165.6 MB (165648964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031ed9d050c8feef582a1a19bddbb4d53c9a2dd4faebfe0da02cc776a1601089`  
		Last Modified: Sat, 11 Feb 2023 12:03:49 GMT  
		Size: 3.2 KB (3241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5411a6427a3f945b7b08f747e7bf9a1a662c939e7d3dce89d7a68ed69c7b62`  
		Last Modified: Sat, 11 Feb 2023 12:03:49 GMT  
		Size: 2.2 KB (2153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
