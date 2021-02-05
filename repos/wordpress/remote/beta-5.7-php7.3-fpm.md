## `wordpress:beta-5.7-php7.3-fpm`

```console
$ docker pull wordpress@sha256:fe45ea46ce6a027ac0f5e77c6ba90f725cbdd8c732b23d00211699fd28359c10
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

### `wordpress:beta-5.7-php7.3-fpm` - linux; amd64

```console
$ docker pull wordpress@sha256:a003a8a8b6e05120afa6e8ede85407032068580e8e6c776861dcff08dae8df0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.7 MB (186659360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c12e763f071ecb4242760f7020bb8d1018c45d52afbbfc84f9b3192f40f23e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:31:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 01:31:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 01:32:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:32:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 01:32:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 01:50:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 01:50:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 01:50:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 01:50:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 02:48:15 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 18:50:58 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 18:50:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 18:50:59 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 18:51:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 18:51:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:59:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:59:28 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:59:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:59:31 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 18:59:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:59:32 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 18:59:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 18:59:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 18:59:35 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 18:59:35 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 23:18:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 23:20:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 23:20:01 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 23:20:02 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 23:26:14 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 23:26:14 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 23:26:14 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 23:26:14 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 23:26:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 23:26:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bab8795938bb41373cc51cd3ccce577cf99b3ddd42d4b109cecc95bc8e1d51`  
		Last Modified: Tue, 12 Jan 2021 03:28:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657d9d2c68b9212bb09c223e67cd72afe8607a1ee7898df13a2f91caf4e5e28d`  
		Last Modified: Tue, 12 Jan 2021 03:29:09 GMT  
		Size: 76.7 MB (76652235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47b5ee58e916d4e3dba85b5821b5c1c348f93da7eaf6d243d5dcdc4a388df32`  
		Last Modified: Tue, 12 Jan 2021 03:28:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2b21c3154cfb9f7c4d526cb389d32671e56b8bc2f5198e14c77f894081fe9a`  
		Last Modified: Thu, 04 Feb 2021 20:49:54 GMT  
		Size: 12.5 MB (12459787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e3d6bc977422f3643d228e877f98b9152f24c1c377952d2a74c7a48c9b9bba`  
		Last Modified: Thu, 04 Feb 2021 20:49:52 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5ad12743a0e4cd8868726e0047aa6f5f62ca960784b5b9afb5a9ceaa1105f9`  
		Last Modified: Thu, 04 Feb 2021 20:49:59 GMT  
		Size: 28.8 MB (28768675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abf637c7b287fd53861206a51cd65a600fe96bccbbc66c528595ebbb4411a2d`  
		Last Modified: Thu, 04 Feb 2021 20:49:51 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb588806620d8da46ef90ae3888ee4bb2f61e208bb67073d35638ec05ed33260`  
		Last Modified: Thu, 04 Feb 2021 20:49:51 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50713eada129dda8aa8121a9f98ef9a34c07eafb6fd442f60e5553680ed1015`  
		Last Modified: Thu, 04 Feb 2021 20:49:51 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb69450cc42a3cd4133dde36d70ece3b2d3af46a62b0af21b6995f80c021c889`  
		Last Modified: Thu, 04 Feb 2021 20:49:52 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eb0a80b23273d67e226d75b86c5e48ab5b5edf84ca23d9f6409b7b1c4ec344`  
		Last Modified: Thu, 04 Feb 2021 23:30:09 GMT  
		Size: 16.8 MB (16847244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56629d3a42ee2f2f8b5cba138b5cd978b120a3699a7cbcd23957818823cc175f`  
		Last Modified: Thu, 04 Feb 2021 23:30:05 GMT  
		Size: 9.3 MB (9259335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a15ef8e26e4971e6437e6692d91bb7dc0c85f29eafc21baae1450f0e865819`  
		Last Modified: Thu, 04 Feb 2021 23:30:00 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711edcee811342dc46a23d9187018cec984fe98a43cad5f67250ad22f0f74ca4`  
		Last Modified: Thu, 04 Feb 2021 23:30:00 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcdb742cc1e6e1d4aff81e0d66a8da710986e693d2a823db2248f38d924fe6d`  
		Last Modified: Thu, 04 Feb 2021 23:32:20 GMT  
		Size: 15.5 MB (15547417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf84a153bc3f97a02b33216f45490429a3c432c8cfe277d9d0324dc77e1c730`  
		Last Modified: Thu, 04 Feb 2021 23:32:16 GMT  
		Size: 2.1 KB (2095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2520dbede39d6cb51e8a62faebfaa8a3bc86da35dbc8fda4b69bcef3bc7cf6e0`  
		Last Modified: Thu, 04 Feb 2021 23:32:16 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:f4cec0d30f05a77020a564e7935d641f53a4ce681a5dbcbf63d99da0f9ff07d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163533556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2d4c16f011bcc1e34c95aed0b27de2dbff7e0297280e7a65d7e34496b5998c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 08:17:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 08:17:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 08:18:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 08:18:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 08:18:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 08:27:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 08:27:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 08:27:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 08:27:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 08:57:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 18:17:24 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 18:17:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 18:17:26 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 18:17:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 18:17:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:21:56 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:21:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:22:02 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 18:22:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:22:05 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 18:22:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 18:22:11 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 18:22:14 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 18:22:17 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 21:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 21:44:15 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 21:44:18 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 21:44:20 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 21:46:12 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 21:46:14 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 21:46:15 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 21:46:15 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 21:46:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 21:46:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875f82a0dbd45f40c3514e20ebda7516bcadfc2e78e321cb713307a0ae63d115`  
		Last Modified: Tue, 12 Jan 2021 09:25:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2713c4ae8eb5d3f30cf7fcc03d75753b0d423dadba590c5b2047530b1a82f3`  
		Last Modified: Tue, 12 Jan 2021 09:25:54 GMT  
		Size: 58.8 MB (58801566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ea6b941c2d5635c446a6acdcc3818ef25ac1fe73f387db4c5ab99300219e1`  
		Last Modified: Tue, 12 Jan 2021 09:25:31 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e5a52dbf5a4ed47229885f7d3453a1b654ccd1a3926c36cae258277b385b97`  
		Last Modified: Thu, 04 Feb 2021 18:49:19 GMT  
		Size: 12.5 MB (12457914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8be911955614966102920321d2f4dcba4f3678305eb8f872cea0cc016c6dea`  
		Last Modified: Thu, 04 Feb 2021 18:49:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2298f01b2067f4a96559710d43574a1f6c21d452f09d0aafbef58dcb39c5816f`  
		Last Modified: Thu, 04 Feb 2021 18:49:14 GMT  
		Size: 27.3 MB (27321585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a635c977953de1868935d4afedffd53f8546bd9acb9c18ac83dfea66fc9fa82b`  
		Last Modified: Thu, 04 Feb 2021 18:49:06 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69355cae302747b046559fe2b921faaf3a1822295ef65a669580093876072ad4`  
		Last Modified: Thu, 04 Feb 2021 18:49:05 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b179e0d805bff7f1d793f1c53f145cc5cfc1f522f2930069ff742dc25561d5`  
		Last Modified: Thu, 04 Feb 2021 18:49:06 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c99a39a5291fc59496449dcc970e949bd45238f86153da9e8d69c5273ce1cd5`  
		Last Modified: Thu, 04 Feb 2021 18:49:05 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9976d4b29e1dd6433b6a5d0a7254cbed6da800ea75b76b991b55f2fdb4d3f3ec`  
		Last Modified: Thu, 04 Feb 2021 21:49:23 GMT  
		Size: 16.4 MB (16407412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8db2d26604e45618b12dc4cc9aab76200a9c3c617314c43e0d8885146489d3`  
		Last Modified: Thu, 04 Feb 2021 21:49:18 GMT  
		Size: 8.1 MB (8129029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9428686ca2c68327780251fbf910ca6d4aad85370dc5a70074eaf10ca72bddb2`  
		Last Modified: Thu, 04 Feb 2021 21:49:16 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92aa9a4a37bdf9b384708385bd258f2c09343cffabaf90d3a41969ffe99ebc45`  
		Last Modified: Thu, 04 Feb 2021 21:49:16 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e52e465072db4f3c89593ddc41dfeabaac2bbe9d2766ac9e880a28951be95`  
		Last Modified: Thu, 04 Feb 2021 21:51:12 GMT  
		Size: 15.5 MB (15547500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1973745b3ca72e4c9950820e247235c817e3854fc6af3a20b1b9c07c40050100`  
		Last Modified: Thu, 04 Feb 2021 21:51:06 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d332043c7cbebc30495fa7d955f7874ed5aa2d740164ba408b7ddc6a459234c`  
		Last Modified: Thu, 04 Feb 2021 21:51:06 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:a12d35e2ed83467bf9abef68ffaccac50f02d2b9eaa843112e41569d3e05e355
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.8 MB (159828669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477eb80c95fed5109f573ec7b0b0ad0d5bf29a863319ffda86c2a3f2de825ea8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:43:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 15:43:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 15:44:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:44:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 15:44:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 15:52:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 15:52:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 15:52:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 15:52:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 16:20:43 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 17:38:43 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 17:38:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 17:38:44 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 17:39:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 17:39:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 17:41:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 17:41:55 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 17:41:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 17:41:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 17:41:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 17:42:00 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 17:42:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 17:42:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 17:42:04 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 17:42:04 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 22:20:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 22:23:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 22:23:16 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 22:23:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 22:31:14 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 22:31:16 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 22:31:16 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 22:31:17 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 22:31:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 22:31:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e8c92106236323b48069345e4cd2a975598cf8e59ed5328bc7ff917437095f`  
		Last Modified: Tue, 12 Jan 2021 16:47:01 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2455a06a5680a8992f82a366764ff612233fc4cc0580977e38b41c68ede8887`  
		Last Modified: Tue, 12 Jan 2021 16:47:18 GMT  
		Size: 59.5 MB (59508577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda08d0c128614f2e4421b636f3c354d88668288eb09d01da892d3eacfb4a20c`  
		Last Modified: Tue, 12 Jan 2021 16:47:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933366778a174e4307023ed1de16f136156d1fc28c9b71abeb2375c5c29c311c`  
		Last Modified: Thu, 04 Feb 2021 18:35:00 GMT  
		Size: 12.5 MB (12457846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ada283dec003d83b83b624fb8f0a5eb444539e67f26c82d3bd7030570b4d51`  
		Last Modified: Thu, 04 Feb 2021 18:34:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81a68467eff3ec2cba63675c11dc60abecb6c3a0252b4f4e7946bd05ff4eb7f`  
		Last Modified: Thu, 04 Feb 2021 18:35:04 GMT  
		Size: 26.3 MB (26321901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93f4f1828dc148b40db61136019b28ebf7965e9d05671ae5c0dc907d456ceae`  
		Last Modified: Thu, 04 Feb 2021 18:34:57 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e70047efb73fe8ecb430bb43aff2eb9eb0b9d79f14035ef4018de17fe9cb3`  
		Last Modified: Thu, 04 Feb 2021 18:34:57 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf70da104ac60065e40370e3411fb9e911f605331d3d44dfcb6e5f588f5f37e`  
		Last Modified: Thu, 04 Feb 2021 18:34:57 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae605d525fabacd989dc818ae81e17d22d5b203495ec52a4d50c62fcf2338ab`  
		Last Modified: Thu, 04 Feb 2021 18:34:57 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f47a1a5677fa07b7ac437311aac01ddff14e91981747f615e623eb5e6c90dc`  
		Last Modified: Thu, 04 Feb 2021 22:35:35 GMT  
		Size: 16.0 MB (15957799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95eebc91bc5122f339a2945eeddd0fe4a4da8ff0548d5d3203137bb276a3a23f`  
		Last Modified: Thu, 04 Feb 2021 22:35:30 GMT  
		Size: 7.3 MB (7302499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9295e0dddfce78fde5344000b533ff13e5b30cfa8594dd8b6c7a5a68a3f4640`  
		Last Modified: Thu, 04 Feb 2021 22:35:28 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de617bc3d0a5fae2a1a335d0e27d5ff284206201bb10f152f345fe16bfe92d1e`  
		Last Modified: Thu, 04 Feb 2021 22:35:28 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea9f2e4922aa8cc45960e612d05ea3f7dbe250c7ce0d6d5cf8678f0fbcf7672`  
		Last Modified: Thu, 04 Feb 2021 22:38:50 GMT  
		Size: 15.5 MB (15547499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5ea6009218ce40c307fd6d35b4799910e8214e26039119f452217f879a47e7`  
		Last Modified: Thu, 04 Feb 2021 22:38:44 GMT  
		Size: 2.1 KB (2093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85dce6c2b6397da4252ceaf7aacb63018de6e68753fad13465c86715efa1b5c`  
		Last Modified: Thu, 04 Feb 2021 22:38:44 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:b3528768491fba98a4e05a241dc824a653998927a827e1798959afe4a2d5fcdb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.1 MB (177135299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ec63593072eba976969cf946c6e3f25eb4c88625cd50e12ed3f514ab7ee61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:57:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 09:57:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 09:57:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:57:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 09:57:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 10:07:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 10:07:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 10:07:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 10:07:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 10:39:47 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 18:39:21 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 18:39:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 18:39:25 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 18:39:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 18:39:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:43:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:43:54 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:43:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:43:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 18:44:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:44:01 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 18:44:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 18:44:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 18:44:05 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 18:44:06 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 21:17:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 21:20:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 21:20:34 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 21:20:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 21:29:45 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 21:29:46 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 21:29:47 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 21:29:48 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 21:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 21:29:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c14cdf3b2bf38116f281b1f08dd94428571f1d8028aca0f4bdd7241578a095`  
		Last Modified: Tue, 12 Jan 2021 11:11:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1153f779dc66475ff6bd2f1bb2ed3481c5577a3e695e2bd3e7db33f9d4a86b28`  
		Last Modified: Tue, 12 Jan 2021 11:12:00 GMT  
		Size: 70.3 MB (70338207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7a48ad69b64a9de956fe744a9589a2555794e40b5b2a847fb0862eeca7438`  
		Last Modified: Tue, 12 Jan 2021 11:11:40 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c335639d0b064bfc98827cfd9bdcdc24c497bc9ac17e30d11c0d51df7e1a33d4`  
		Last Modified: Thu, 04 Feb 2021 19:36:33 GMT  
		Size: 12.5 MB (12458685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04c31e35344fc5202cdfac6830201b1de2f2cb087f46904ee5499b64faede1e`  
		Last Modified: Thu, 04 Feb 2021 19:36:32 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0412cff8cfe3a0e3db75030d2548bfb44a2b4e7658c104bcff292773637d93b6`  
		Last Modified: Thu, 04 Feb 2021 19:36:38 GMT  
		Size: 28.4 MB (28441664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713f29e67f227f922a3d65640af4b67ec16e869fd0ed9ff5b8b6ebbb3833a719`  
		Last Modified: Thu, 04 Feb 2021 19:36:30 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8734087e1f008924759c29bfa0a2a3c73af8be4f717432407da63679812d15`  
		Last Modified: Thu, 04 Feb 2021 19:36:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db8cf2320490a310066974464c8dacb4bd49d4d4434d7d8da71f2afb5486966`  
		Last Modified: Thu, 04 Feb 2021 19:36:30 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2034a9aab4ed267318725ad633f45fa327c2912c7367ad819a94e79f5e72b6c`  
		Last Modified: Thu, 04 Feb 2021 19:36:30 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6ee5a7dde841b948738540f53d6978abcb7aab931531bcb72189ec66bf8ecd`  
		Last Modified: Thu, 04 Feb 2021 21:34:40 GMT  
		Size: 16.8 MB (16794655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808544327e917343c5106f12b9fb50aab30413869ec03ece9b390e6815dd5011`  
		Last Modified: Thu, 04 Feb 2021 21:34:35 GMT  
		Size: 7.7 MB (7673460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bc405bff214b954588a20792e73da33b52006dc38d3e0ae193667e47a353ea`  
		Last Modified: Thu, 04 Feb 2021 21:34:33 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876766b40dfda3c48f9176b59f5d92a438ffa90b6d3c0babc03458ea7036d574`  
		Last Modified: Thu, 04 Feb 2021 21:34:33 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154573e5a88086324d38aecbab755e3aa9e375acfc5a279900027808715188a9`  
		Last Modified: Thu, 04 Feb 2021 21:37:46 GMT  
		Size: 15.5 MB (15547504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c692723ec3aa6ca9e3f34bc387b14f30c3f3f0706ebca53d90c4e90e2b4a8b1`  
		Last Modified: Thu, 04 Feb 2021 21:37:41 GMT  
		Size: 2.1 KB (2094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3828430d9c00170f7e06208a70efb0f02df16f4efd0e4c059288c0c2cc7219fc`  
		Last Modified: Thu, 04 Feb 2021 21:37:41 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; 386

```console
$ docker pull wordpress@sha256:987322472bedc7d83ae7fc997b9137fd929da15e6dd5c078d10e9cf0c102ddd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (192000931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298606271f35478ee92e89f04cf855582313dfa5a11ccafd79aeb6226b072181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:49:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 09:49:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 09:49:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:49:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 09:49:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 10:03:15 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 10:03:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 10:03:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 10:03:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 10:45:06 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 19:28:57 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 19:28:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 19:28:57 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 19:29:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 19:29:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:38:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 19:38:22 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:38:22 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 19:38:23 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 19:38:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 19:38:24 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 19:38:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 19:38:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 19:38:25 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 19:38:25 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 23:58:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 23:59:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 23:59:34 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 23:59:35 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 00:05:12 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 00:05:12 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 00:05:12 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 00:05:12 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 00:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 00:05:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff4a03eef372628e9238ed30c4800e2442e94d5f9888176fcc18ca03ff32d6`  
		Last Modified: Tue, 12 Jan 2021 11:24:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4817302a66115aef63495cbc3fc4afa659ecf7332c18dd1dacd4bf0e04bd9dcb`  
		Last Modified: Tue, 12 Jan 2021 11:25:03 GMT  
		Size: 81.2 MB (81196616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef262fa23965002659eab0f980b5e20db2939288d651a1b6a81c85f44f90f192`  
		Last Modified: Tue, 12 Jan 2021 11:24:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c571302d025fe2fd0c0c8bbdc820a6aae2885b4a166466e738d8cd1e7bbee4f`  
		Last Modified: Thu, 04 Feb 2021 21:20:50 GMT  
		Size: 12.5 MB (12459070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d8a176c363a0d747a84ecaf0af5774cf30e4e989410ab8c7099f4721842006`  
		Last Modified: Thu, 04 Feb 2021 21:20:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ae6b5388c0745bcde13cc19b30c782cdf4bf0badcba600a168582f1a1ab2d`  
		Last Modified: Thu, 04 Feb 2021 21:20:56 GMT  
		Size: 29.3 MB (29318508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5f4cb17de8d347b3ac84aac5bccbd39d4fc430dab84e98d4ca0dcbd2e73a51`  
		Last Modified: Thu, 04 Feb 2021 21:20:47 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf16dd471fcdb29ce1cafcb99c4c5f2353fd610a945d819c821bf97e59572e`  
		Last Modified: Thu, 04 Feb 2021 21:20:47 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c727092bb7b38daa0b3306ef2effd5e9ba63a121288cf28880c047a899dd256f`  
		Last Modified: Thu, 04 Feb 2021 21:20:47 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a58be81f8f0c253970a2a8d6565b5d76d4f01e2ebd616195f09b27dda1be4`  
		Last Modified: Thu, 04 Feb 2021 21:20:47 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9043c94bb250e023c759e643e255caa0ef2a6051a4b1db7b31de67fde07bd6`  
		Last Modified: Fri, 05 Feb 2021 00:08:44 GMT  
		Size: 17.2 MB (17165092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee2ff53a71086a8953c1a9158bc95732042a7f9032d3f82bf5e7d576f43fb68`  
		Last Modified: Fri, 05 Feb 2021 00:08:40 GMT  
		Size: 8.5 MB (8529645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a00ef0f7103b06f3368802ad99f86cc38a8e36d39c8fa7e7a00a7fa433bbb1`  
		Last Modified: Fri, 05 Feb 2021 00:08:38 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d27a2ef26bb75ea42b8b5f904fe8f0c9a1bdf37022741ee25b7993beaa36e2b`  
		Last Modified: Fri, 05 Feb 2021 00:08:37 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226ce7b7b4af4186221b0f6989ba0d9661532884ff0b51064f46fcbd22643b1b`  
		Last Modified: Fri, 05 Feb 2021 00:11:00 GMT  
		Size: 15.5 MB (15547413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0714c8acc9e91c6227122ed9ff0d25396c1dc75aeb6289864b4f5a73ca546`  
		Last Modified: Fri, 05 Feb 2021 00:10:56 GMT  
		Size: 2.1 KB (2095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502e95385310bac397a7ec6eb26d0e2e91142815d52fbabf964af9bc7a5e4c34`  
		Last Modified: Fri, 05 Feb 2021 00:10:56 GMT  
		Size: 1.6 KB (1638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; mips64le

```console
$ docker pull wordpress@sha256:1a22af2e618dcc5c48ae3d1a84db087c3ef3db2a19d2efebe71123ee42300706
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167696017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539f3f45ec38af0f5108f82ac83c5527c7f3e1190a30cbec9f875c7208f4747`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:16:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 03:16:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 03:17:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:17:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 03:17:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 03:42:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 03:42:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 03:42:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 03:42:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 05:11:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 18:08:55 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 18:08:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 18:08:56 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 18:09:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 18:09:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:22:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:22:17 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:22:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:22:21 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 18:22:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:22:21 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 18:22:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 18:22:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 18:22:24 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 18:22:24 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 19:39:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 19:42:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Feb 2021 19:42:43 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 19:42:45 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 19:44:17 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 19:44:18 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 19:44:18 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 19:44:19 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:44:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 19:44:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c492e970ef61753e94d86eff716cb66399cbb6a6759108bd1b7d38b097fc463`  
		Last Modified: Tue, 12 Jan 2021 05:40:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ce2769420a3fc430b336f3a558c2e3596b23cd3570ca7af5944460dcb79c88`  
		Last Modified: Tue, 12 Jan 2021 05:41:14 GMT  
		Size: 61.4 MB (61390093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deff18bb57c1764f805997167faad0d6dc5d5e10f670c16720a2cd911358143`  
		Last Modified: Tue, 12 Jan 2021 05:40:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40035dc4a58938a081b634567694d77ad2a502985a921d064278c950f9441c6d`  
		Last Modified: Thu, 04 Feb 2021 18:42:16 GMT  
		Size: 12.5 MB (12457159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669723f57ca787e37301601a40d13406b7e9769772a5f1a1020f0e4ada62507c`  
		Last Modified: Thu, 04 Feb 2021 18:42:13 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571763fd776590900b308006511567ad5f09d5947ad2f158c9e4843b1e62f8`  
		Last Modified: Thu, 04 Feb 2021 18:42:31 GMT  
		Size: 28.1 MB (28118724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ab89d47e0fee56a77bb86a527b6a76ccd38103056c8e45300eef9198f40941`  
		Last Modified: Thu, 04 Feb 2021 18:42:11 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fa557c5356d6c5187833b770ca61413dcea1e56727d4b3965d76d48f5bd4c8`  
		Last Modified: Thu, 04 Feb 2021 18:42:10 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d82039bf2ae6433bc59c26ff257d3e41ee5b39be9d2ceaecae9cb18048fa70`  
		Last Modified: Thu, 04 Feb 2021 18:42:11 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555c976bf9b13ff3d98f6b6bf435c3ffdc8e93959ad78b3c2cc2ec810c85157`  
		Last Modified: Thu, 04 Feb 2021 18:42:11 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a35a7d4de46a90e30b9d680a864d9713cc508097ed0341eb7a15908275bf8a`  
		Last Modified: Thu, 04 Feb 2021 19:48:58 GMT  
		Size: 16.7 MB (16674621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead6ddfcc001a0f6c6a39bcdcb9da2022920735575b54b141a803f5cb8b3b3ee`  
		Last Modified: Thu, 04 Feb 2021 19:48:47 GMT  
		Size: 7.7 MB (7712708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf9de0393a69fce3544d4ecbe881e01760f8c0defe268e21a260a6829179f6c`  
		Last Modified: Thu, 04 Feb 2021 19:48:41 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dcc95b973bc7f5bb38fb0b3975edae61baa3bd4b4f6ff7d86fb3c60f0bc4d1`  
		Last Modified: Thu, 04 Feb 2021 19:48:41 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1bae26ff190bd286591ec42825f58148da0bd92e1021bd04289ea277240bc0`  
		Last Modified: Thu, 04 Feb 2021 19:52:31 GMT  
		Size: 15.5 MB (15547418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25852ddd4ccee9861360436ee26652a082c7af326ba0348127c1ea12b82acad4`  
		Last Modified: Thu, 04 Feb 2021 19:52:20 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68c109a5cfc4e1b02eb27468659bcef7e8edacbef691e8763197438fbe531cd`  
		Last Modified: Thu, 04 Feb 2021 19:52:20 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; ppc64le

```console
$ docker pull wordpress@sha256:45d589ba2416e38ee730d502bf4e87628922d4dcaf10edfec5116210198ba574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (198025397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cde168f511a2b1740ed26b4dfbce7a69a8b1f139f93886f476632bd717a0476a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 07:42:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 07:42:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 07:46:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 07:46:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 07:46:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 08:05:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 08:05:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 08:06:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 08:06:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 09:07:01 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Jan 2021 09:07:07 GMT
ENV PHP_VERSION=7.3.26
# Tue, 12 Jan 2021 09:07:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Tue, 12 Jan 2021 09:07:13 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Tue, 12 Jan 2021 09:08:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jan 2021 09:08:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jan 2021 09:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:49:06 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:49:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:49:41 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 21 Jan 2021 19:49:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:49:57 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:50:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:50:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:50:28 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:50:33 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 21:54:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 22:05:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 22:06:01 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Jan 2021 22:06:16 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 03 Feb 2021 22:18:57 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 03 Feb 2021 22:19:07 GMT
VOLUME [/var/www/html]
# Wed, 03 Feb 2021 22:19:17 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Wed, 03 Feb 2021 22:19:27 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Wed, 03 Feb 2021 22:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Feb 2021 22:19:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b19aea126b329f3a56cc45ffe95a741105ac95ebba8940d4e59d343307ab`  
		Last Modified: Tue, 12 Jan 2021 09:26:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2915accbe4b788b97c857b0c847ac4ae8151fd5e5f45c5d3f0447c891468aaf2`  
		Last Modified: Tue, 12 Jan 2021 09:26:17 GMT  
		Size: 82.3 MB (82260027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59a0d938c9801c4f31a9b364385a96e2aab022f2d569bd6d64c5d396d30f25`  
		Last Modified: Tue, 12 Jan 2021 09:25:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac2963690c5a91bcde10b50af3efb3e3190b6dfd7010e4670d539300d47dd14`  
		Last Modified: Tue, 12 Jan 2021 09:33:32 GMT  
		Size: 12.5 MB (12459970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeae602a308742f9df0091bdead4783efc67d55d9e3f3ce9b066e5c0da866e7b`  
		Last Modified: Tue, 12 Jan 2021 09:33:32 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f6de3800c89914866ccce5fe15bedd965229694d64020acc6b3a138b9faf5e`  
		Last Modified: Tue, 12 Jan 2021 09:33:33 GMT  
		Size: 30.5 MB (30470182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d3fc42bd673cd4163193850b4d9441e57249db89e12d1da79984fd31787c97`  
		Last Modified: Thu, 21 Jan 2021 20:11:21 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401cbe96fffe1d6cee00c28481cdde1cf042991f2d596e9c121a687c2c81e9d1`  
		Last Modified: Thu, 21 Jan 2021 20:11:23 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa22817f59bbc27dfaa3d671a08f651f9ed994d4764cb1d723e5b4e30f7f6efc`  
		Last Modified: Thu, 21 Jan 2021 20:11:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedc8de1e66744e92f56b24d1cebcd9505d9b2e9eef88f8dba03d511f0a404ef`  
		Last Modified: Thu, 21 Jan 2021 20:11:23 GMT  
		Size: 8.4 KB (8423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0a55ad56cf85d49d487294c5056b49acb2abe86d79450564fe0c7afe7809f4`  
		Last Modified: Thu, 21 Jan 2021 22:38:14 GMT  
		Size: 17.6 MB (17648203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98863cec104570e1bb6c1a16d2bdecdfba1a00f2a1a20dcddee84daab4e25bd`  
		Last Modified: Thu, 21 Jan 2021 22:38:09 GMT  
		Size: 9.1 MB (9090028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4516e90b184aa3f6600bc34c24e785798e4152d4dfb0e0c0b82ccc0085725313`  
		Last Modified: Thu, 21 Jan 2021 22:38:08 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fd0f2664452e866c7d542c439310e45522d306e632a0ceb02feea63add332c`  
		Last Modified: Thu, 21 Jan 2021 22:38:08 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2daa495e6e0249accabf0752262d8281b23b0c424ba146fe97e4a49c588a34`  
		Last Modified: Wed, 03 Feb 2021 22:28:46 GMT  
		Size: 15.5 MB (15547485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454cb5235ac8518552ad3197cbd25dadceb253151eb7276a16045a624e97feb`  
		Last Modified: Wed, 03 Feb 2021 22:28:42 GMT  
		Size: 2.1 KB (2095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396732ecc3619b3b1aa31e120f9cf04bc7672f0c3e1e7168686a579fdac7102`  
		Last Modified: Wed, 03 Feb 2021 22:28:42 GMT  
		Size: 1.6 KB (1638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm` - linux; s390x

```console
$ docker pull wordpress@sha256:681ab3dee067a48397e9b88b6d44bdece6905a3dec8399771a8a4f25e56a7649
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170945647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fff0e19af9b191c99ec97cfbc876a0633da58369aff09381b3935fe957cea98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:08:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 03:08:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 03:09:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:09:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 03:09:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 03:16:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 12 Jan 2021 03:16:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 03:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 03:16:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 03:43:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 19:10:28 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 19:10:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 19:10:29 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 19:11:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Feb 2021 19:11:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:16:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 19:16:08 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:16:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 19:16:11 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 04 Feb 2021 19:16:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 19:16:12 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 19:16:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 19:16:14 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 19:16:15 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 19:16:15 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 04:47:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 04:50:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 05 Feb 2021 04:50:05 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 04:50:06 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 04:57:05 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 04:57:07 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 04:57:07 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 04:57:07 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 04:57:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 04:57:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431047e5ed5c643edfcfd558938d22fb3b8a81d602e482d419ab2a495635c86f`  
		Last Modified: Tue, 12 Jan 2021 03:54:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e023225fac18d7c7a1a8571203b6cf3eacef731b9f052498a931c6e7307fb5c`  
		Last Modified: Tue, 12 Jan 2021 03:54:37 GMT  
		Size: 64.7 MB (64706685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4472bbc450782c5dfc73e56ae04e1325ab78e741bd0ee3acea7c87d570ae33`  
		Last Modified: Tue, 12 Jan 2021 03:54:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0593963eb2ca67513021ffe59090f801ce640c9c134d3a621bff7b88d9cdb5e`  
		Last Modified: Thu, 04 Feb 2021 20:49:47 GMT  
		Size: 12.5 MB (12458144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8731b8cbd67677077fcab6578ec75336c4638a239d967dcb5f533ac7c8894d3`  
		Last Modified: Thu, 04 Feb 2021 20:49:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86256e92df222dae35b718af7eecdcb3ff6f7cd2043fad64707e1747b0debe3`  
		Last Modified: Thu, 04 Feb 2021 20:49:38 GMT  
		Size: 27.9 MB (27906034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d631a24f243306d8da7216bdea7951aad8ec47066e25bd55e9c1cd59686a50`  
		Last Modified: Thu, 04 Feb 2021 20:49:30 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a69f3826aafef041d94ca4525607154a7759708d39c02231ad2ffbc90d684`  
		Last Modified: Thu, 04 Feb 2021 20:49:30 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4c04d477ee64e3349bd17cad642062522bb32d3e7fb9482f91fe75aa5c9eaa`  
		Last Modified: Thu, 04 Feb 2021 20:49:30 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70dafc2b8d4994235b66592033d34b7028b869a7c9cd524e74c3ac2cd6fb5cd`  
		Last Modified: Thu, 04 Feb 2021 20:49:34 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7235f92f4c9b8db62f010e5c12cc7c5bca73002dad3ab919836e5ee1201efbbe`  
		Last Modified: Fri, 05 Feb 2021 05:30:58 GMT  
		Size: 16.8 MB (16768508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfb453143a9bab717ba314294fff185e12ac27c3cb243d367a9158f5d7a7c81`  
		Last Modified: Fri, 05 Feb 2021 05:30:37 GMT  
		Size: 7.8 MB (7818721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e58d741d6df719e067368ab6902db69a391f94cacb844f3d4ecf97167f6f18e`  
		Last Modified: Fri, 05 Feb 2021 05:30:32 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728b075ba0017e7ada89eb1d7d2413d541fd00716d3532b4a82f7f2c014380f5`  
		Last Modified: Fri, 05 Feb 2021 05:30:32 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a706c8c9ec8ee75fd8fbb925a59a400ad27602e8a070b3dbdab663da5221fb`  
		Last Modified: Fri, 05 Feb 2021 06:29:39 GMT  
		Size: 15.5 MB (15547502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660a50a543e963fb02f9496d81cbae0286e6f92f92af4ea18700dae4fa69f8a`  
		Last Modified: Fri, 05 Feb 2021 06:29:39 GMT  
		Size: 2.1 KB (2097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a812d3bdc5a31fcaf84276b53fcac5bd13464400e93fe8aba72ea026f83edce4`  
		Last Modified: Fri, 05 Feb 2021 06:29:39 GMT  
		Size: 1.6 KB (1637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
