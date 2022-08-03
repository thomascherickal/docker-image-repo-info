## `drupal:9-apache-bullseye`

```console
$ docker pull drupal@sha256:ef5a344c27ac91822e186f73f8d977038f5c99b844ca61affc7406366402898d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:9-apache-bullseye` - linux; amd64

```console
$ docker pull drupal@sha256:11afa4881f8de498ba8f25e57cf68dad63761dd4ee55df951533b151092b3a60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.9 MB (188862506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccfc0309f60d849f7ca786301621b21e0f10fffefc0d8415787edbce9c744ef7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:17:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 06:17:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:17:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:17:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:17:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:21:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:21:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:21:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:21:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:21:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:21:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:21:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 07:43:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 02 Aug 2022 08:09:21 GMT
ENV PHP_VERSION=8.0.21
# Tue, 02 Aug 2022 08:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.21.tar.xz.asc
# Tue, 02 Aug 2022 08:09:21 GMT
ENV PHP_SHA256=e87a598f157e0cf0606e64382bb91c8b30c47d4a0fc96b2c17ad547a27869b3b
# Tue, 02 Aug 2022 08:09:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 08:09:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 08:12:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 08:12:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 08:12:35 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 08:12:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 08:12:35 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 08:12:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 08:12:36 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 08:12:36 GMT
EXPOSE 80
# Tue, 02 Aug 2022 08:12:36 GMT
CMD ["apache2-foreground"]
# Wed, 03 Aug 2022 08:35:56 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 08:35:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 03 Aug 2022 08:35:56 GMT
COPY file:ebe397bd23f15e762d9b58235d8b4962a65d12542d3be8adc4e774426b23f91d in /usr/local/bin/ 
# Wed, 03 Aug 2022 08:35:57 GMT
ENV DRUPAL_VERSION=9.4.4
# Wed, 03 Aug 2022 08:35:57 GMT
WORKDIR /opt/drupal
# Wed, 03 Aug 2022 08:36:07 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 03 Aug 2022 08:36:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239fd0772e9a466a042a9ded0aad7001614c48ea38eeb017681ad8c4fe5ba0a`  
		Last Modified: Tue, 02 Aug 2022 08:57:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ccb8ba6c06f34bd30d69d2ecfda128114c9cd01f63f5e6933645045523d7dd`  
		Last Modified: Tue, 02 Aug 2022 08:57:23 GMT  
		Size: 91.6 MB (91602719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e907707b68ee157bb766af31f4177f9c15e7ff3d82b9a2b8ccb24bd970356c2d`  
		Last Modified: Tue, 02 Aug 2022 08:57:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f001901b2b663a127bc8095d46923fd8c0e78241abec3192a5ba949e4aefe58c`  
		Last Modified: Tue, 02 Aug 2022 08:57:54 GMT  
		Size: 19.2 MB (19244838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3926f8e80674d42227b4973705a6835950a0dcbb27d9ecfa0a56e8e577a4cf58`  
		Last Modified: Tue, 02 Aug 2022 08:57:50 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc6b8b3381c745df5137a078293a4ef876e87ed4d3c501b034858cfa4a722ca`  
		Last Modified: Tue, 02 Aug 2022 08:57:50 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36061c863b41ad62ca9632f6ee44f59e0161714db3760d40700603214b025f13`  
		Last Modified: Tue, 02 Aug 2022 09:11:03 GMT  
		Size: 11.1 MB (11126526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33d4de3115f677d3cda92a90b1164ba6602a2cd9f4e5485cc803af98dc600c7`  
		Last Modified: Tue, 02 Aug 2022 09:11:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a8c766f28254b084a6ef696de3507c880a5425c7e55a3d30f5b928c756c579`  
		Last Modified: Tue, 02 Aug 2022 09:11:02 GMT  
		Size: 10.8 MB (10777466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc76b6b31a238b6f3876d413b172536e3acbc708334dbc48ab09150bee5ee3d3`  
		Last Modified: Tue, 02 Aug 2022 09:11:00 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ea2aedd6379ab2ad5d02b6a34ad09b382fce3916d37d3f6d6be4843ddc48c3`  
		Last Modified: Tue, 02 Aug 2022 09:11:00 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5ee78bd9a69fa8dd3590074a82f0dfc87bba3e7f3c7834de00c4e3a9f7474f`  
		Last Modified: Tue, 02 Aug 2022 09:11:00 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bbcd6b5b7375a53faf0217601be555ce36c52a5af05854652dcc468e936f48`  
		Last Modified: Wed, 03 Aug 2022 08:58:08 GMT  
		Size: 2.3 MB (2292273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf179ab2488f0cef687ff034b471c0c1d035c009a073c93e6ff9951ef7784fe`  
		Last Modified: Wed, 03 Aug 2022 08:58:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1dcc252df0b5a192c703e164da75c20f1681ca6dadf30a07d058647ec33f2c`  
		Last Modified: Wed, 03 Aug 2022 08:58:08 GMT  
		Size: 670.4 KB (670423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ff2f8f662ed6df973850289bb528a7d0a386d382b9c835d1a23cef8a94f9c8`  
		Last Modified: Wed, 03 Aug 2022 08:58:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9449cebc7fea710c87ebf8b8f918563cdf1d646819dad1dd20be149267acb7`  
		Last Modified: Wed, 03 Aug 2022 08:58:13 GMT  
		Size: 21.8 MB (21775462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache-bullseye` - linux; arm variant v7

```console
$ docker pull drupal@sha256:94bf6c6c9c5e46f737c432d5b829abb9f9a54083f9a4131d7aae4b7bf57be97b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158428788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6d64e94a403f7a5dd6e725f15e8f0e60b4c4f694fd9ae29c7c756bd991040`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:58:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jul 2022 10:58:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jul 2022 10:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:58:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jul 2022 10:58:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jul 2022 11:04:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jul 2022 11:04:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jul 2022 11:04:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jul 2022 11:04:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jul 2022 11:04:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jul 2022 11:04:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 11:04:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 11:04:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jul 2022 12:29:37 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 12 Jul 2022 12:29:37 GMT
ENV PHP_VERSION=8.0.21
# Tue, 12 Jul 2022 12:29:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.21.tar.xz.asc
# Tue, 12 Jul 2022 12:29:38 GMT
ENV PHP_SHA256=e87a598f157e0cf0606e64382bb91c8b30c47d4a0fc96b2c17ad547a27869b3b
# Tue, 12 Jul 2022 12:29:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 12:29:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jul 2022 12:34:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jul 2022 12:34:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 12 Jul 2022 12:34:34 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jul 2022 12:34:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jul 2022 12:34:35 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jul 2022 12:34:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jul 2022 12:34:36 GMT
WORKDIR /var/www/html
# Tue, 12 Jul 2022 12:34:37 GMT
EXPOSE 80
# Tue, 12 Jul 2022 12:34:37 GMT
CMD ["apache2-foreground"]
# Sat, 30 Jul 2022 03:17:02 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Jul 2022 03:17:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 30 Jul 2022 03:17:03 GMT
COPY file:ebe397bd23f15e762d9b58235d8b4962a65d12542d3be8adc4e774426b23f91d in /usr/local/bin/ 
# Sat, 30 Jul 2022 03:17:03 GMT
ENV DRUPAL_VERSION=9.4.4
# Sat, 30 Jul 2022 03:17:03 GMT
WORKDIR /opt/drupal
# Sat, 30 Jul 2022 03:17:14 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 30 Jul 2022 03:17:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5f3d640b5f74b9ffbb83cee99e75da8ead005098ef953e12834df9bc804681`  
		Last Modified: Tue, 12 Jul 2022 14:04:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84040343fb8450c093ced981918f719c1df12981b96bae5ccfa953bc809b2575`  
		Last Modified: Tue, 12 Jul 2022 14:04:43 GMT  
		Size: 69.3 MB (69319177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75045a7aa298bf2d94d58a3852608776599c66243fdda85f6f3a1c3252f8856`  
		Last Modified: Tue, 12 Jul 2022 14:04:00 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06596302e2a8babee61a1ff3b0ba581c3212aa0708c1f8c1bc6bd2780fa0a6e8`  
		Last Modified: Tue, 12 Jul 2022 14:05:32 GMT  
		Size: 18.0 MB (17998326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2476aeffdf7deaaf51b5f4bf51a2637b77a28ebe3e8ba4a57042bf1f920a4bf`  
		Last Modified: Tue, 12 Jul 2022 14:05:22 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df58c7d22f49220b8d24bc1a89df3ef2d57468d2fc3401828ef54f6e38b3f2fb`  
		Last Modified: Tue, 12 Jul 2022 14:05:21 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2743fcfd9e576e0897b6eac0c28cbf3e7776cc75fb6009896ec51c2e2ca34a`  
		Last Modified: Tue, 12 Jul 2022 14:18:26 GMT  
		Size: 11.1 MB (11125105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a85fdfafd12972b03537e9af608108c8230bad5c62d5c6640e086677c2658dd`  
		Last Modified: Tue, 12 Jul 2022 14:18:22 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b838c11391b53ed11179f091a8083d3bef063daee9d1dadc57d2ceceb21a8`  
		Last Modified: Tue, 12 Jul 2022 14:18:28 GMT  
		Size: 9.3 MB (9308340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09390b6406c3deed1f7121f7f92577b576249ca63985f2b94f73609209bed33c`  
		Last Modified: Tue, 12 Jul 2022 14:18:21 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc235ddaa5f2d05f6a8c4dc8afdba224a3d8c1ccd6abd70f82dcfa867e11bb4b`  
		Last Modified: Tue, 12 Jul 2022 14:18:21 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769518bd2b78c334f5fbcfe3805314d3712f94ba8cf865108deb542937aa71d`  
		Last Modified: Tue, 12 Jul 2022 14:18:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1e98643cd9a6fbe326e89f72e05866f85fd92b89ef6800a372b8a1feb0c44c`  
		Last Modified: Sat, 30 Jul 2022 04:03:00 GMT  
		Size: 1.7 MB (1665467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de049b34fe29d80938d48dddcc09b736fe95040e44377243ae06f89f874948`  
		Last Modified: Sat, 30 Jul 2022 04:03:00 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2e0c623346b1d1a7082cd457fd94321cc0abeda49e36f1bab471588579b5d0`  
		Last Modified: Sat, 30 Jul 2022 04:03:00 GMT  
		Size: 670.4 KB (670424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e45f9eafd68fe0b75d73dc40c4ba68b028f08c12d75f92dce5cc6601bea59f`  
		Last Modified: Sat, 30 Jul 2022 04:03:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0595a2c15ec88b19efd5e51aa5a371a7bbcf9d9caee763cae776a285c9235884`  
		Last Modified: Sat, 30 Jul 2022 04:03:12 GMT  
		Size: 21.8 MB (21775325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache-bullseye` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:a467f8d1f6f681f7dc8919862b71076e8308599b74eb3db1a27131c9c93e0a79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.2 MB (181246102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ee5fbdb8d5ce7631df9d5af07d23ec93247c25d9bd35a4254a49787b3171226`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 07:49:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 07:49:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 07:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 07:49:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 07:49:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 07:53:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 07:53:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 07:54:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 07:54:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 07:54:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 07:54:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 07:54:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 07:54:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 09:33:39 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 02 Aug 2022 09:57:15 GMT
ENV PHP_VERSION=8.0.21
# Tue, 02 Aug 2022 09:57:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.21.tar.xz.asc
# Tue, 02 Aug 2022 09:57:17 GMT
ENV PHP_SHA256=e87a598f157e0cf0606e64382bb91c8b30c47d4a0fc96b2c17ad547a27869b3b
# Tue, 02 Aug 2022 09:57:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 09:57:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 09:59:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 10:00:00 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 10:00:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 10:00:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 10:00:02 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 10:00:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 10:00:04 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 10:00:05 GMT
EXPOSE 80
# Tue, 02 Aug 2022 10:00:06 GMT
CMD ["apache2-foreground"]
# Wed, 03 Aug 2022 06:07:27 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 06:07:28 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 03 Aug 2022 06:07:29 GMT
COPY file:ebe397bd23f15e762d9b58235d8b4962a65d12542d3be8adc4e774426b23f91d in /usr/local/bin/ 
# Wed, 03 Aug 2022 06:07:29 GMT
ENV DRUPAL_VERSION=9.4.4
# Wed, 03 Aug 2022 06:07:30 GMT
WORKDIR /opt/drupal
# Wed, 03 Aug 2022 06:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 03 Aug 2022 06:07:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b170f8f8cb6c982bdcd7588f95686d62d8c44754cbb47e86fbc26bc2568b370`  
		Last Modified: Tue, 02 Aug 2022 10:48:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc755ababc1c79d77115a60ea2a1d1e2c46db01a697c4175ef4ea82269c7c493`  
		Last Modified: Tue, 02 Aug 2022 10:49:03 GMT  
		Size: 86.9 MB (86923392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f2dd6f420736507b7bd9b484596e6d336fd3ae3ec500d0727cc53db5edb128`  
		Last Modified: Tue, 02 Aug 2022 10:48:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e764bf237e7d4c20d5b8bb997fe29e000a9fc2a67f70925f9ed526ac8e77bc16`  
		Last Modified: Tue, 02 Aug 2022 10:49:38 GMT  
		Size: 19.0 MB (18950357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27245487be45224e75e536ee5b8467c37afdeeb0aebeb57ffc664d9291e0b7b1`  
		Last Modified: Tue, 02 Aug 2022 10:49:35 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbda14df7c9551bbb70e2b2c4be41650d48539e94084fd48fa7225ad5a8c715b`  
		Last Modified: Tue, 02 Aug 2022 10:49:35 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f8eac84b2d2f18fd6e9cb49308f178d2b1eacd5480b4e166c013eacd2f1c4`  
		Last Modified: Tue, 02 Aug 2022 11:03:52 GMT  
		Size: 10.9 MB (10909356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c1df3819e31f8cf7f7217328ce718ddc94ee4d9edeffa23cd18ef62cc26014`  
		Last Modified: Tue, 02 Aug 2022 11:03:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a0d7fcf5815618e9db25ab004b55d8ac40fc62a43fbd674eeed48c95ac4d2b`  
		Last Modified: Tue, 02 Aug 2022 11:03:51 GMT  
		Size: 10.2 MB (10232908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a94c24c3825bf64e4f4b161db4f94da8f969da2e25b0f190872bfcda635535a`  
		Last Modified: Tue, 02 Aug 2022 11:03:49 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f1a946a268610ea6741620567fb3771c20c2b9a501654852b22cf697e3fd45`  
		Last Modified: Tue, 02 Aug 2022 11:03:50 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2559cd6769f0e7190d5e133d8ffeceda17190bf983d65a6af245849cd7418269`  
		Last Modified: Tue, 02 Aug 2022 11:03:49 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4b51fd60c3bb8eba5f177e1534a56bbc4e935131e6d77beee26f9ec323427`  
		Last Modified: Wed, 03 Aug 2022 06:42:29 GMT  
		Size: 1.7 MB (1721005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80729da86fc99732d9fd6959e67d4ff13d17d336eb8ff700cf87eb301bb610c`  
		Last Modified: Wed, 03 Aug 2022 06:42:28 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc632f49406d0cd4ffcdb510591720b9191dbe22ba08b83d52e8ea452febd479`  
		Last Modified: Wed, 03 Aug 2022 06:42:28 GMT  
		Size: 670.4 KB (670423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391bd40475600fc59b54e36873bba94a104c56ace1ee9fec3d7df7acb8f500a3`  
		Last Modified: Wed, 03 Aug 2022 06:42:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747413939fcfc2697da2c5886c38e9a4493144be8c8c1a8423fe5acf1760fda2`  
		Last Modified: Wed, 03 Aug 2022 06:42:33 GMT  
		Size: 21.8 MB (21778457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache-bullseye` - linux; 386

```console
$ docker pull drupal@sha256:5a7fb79b0f7d3f7c9cd3e0358a2652bf9b047477ecaa639cec27a5ffa4f49f5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191094434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac76f2df09906df254a85c80da797be6980525fa132102e1a7a116c19f7b51ef`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:13:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 06:13:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:14:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:14:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:17:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:17:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:17:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:17:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:17:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:17:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:17:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:17:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 07:34:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 02 Aug 2022 07:59:04 GMT
ENV PHP_VERSION=8.0.21
# Tue, 02 Aug 2022 07:59:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.21.tar.xz.asc
# Tue, 02 Aug 2022 07:59:06 GMT
ENV PHP_SHA256=e87a598f157e0cf0606e64382bb91c8b30c47d4a0fc96b2c17ad547a27869b3b
# Tue, 02 Aug 2022 07:59:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 07:59:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 08:01:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 08:01:57 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 08:01:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 08:01:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 08:01:59 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 08:02:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 08:02:01 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 08:02:02 GMT
EXPOSE 80
# Tue, 02 Aug 2022 08:02:03 GMT
CMD ["apache2-foreground"]
# Tue, 02 Aug 2022 18:21:56 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:21:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Aug 2022 18:21:58 GMT
COPY file:ebe397bd23f15e762d9b58235d8b4962a65d12542d3be8adc4e774426b23f91d in /usr/local/bin/ 
# Tue, 02 Aug 2022 18:21:58 GMT
ENV DRUPAL_VERSION=9.4.4
# Tue, 02 Aug 2022 18:21:59 GMT
WORKDIR /opt/drupal
# Tue, 02 Aug 2022 18:22:12 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 02 Aug 2022 18:22:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f2682e124b981c3172137f1f4738d436f5c2e2b51bee2fc331221a7441f08`  
		Last Modified: Tue, 02 Aug 2022 08:51:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb3789a015578785e35f8858874911ca9555cbce7195247bb1de3be188416d`  
		Last Modified: Tue, 02 Aug 2022 08:51:56 GMT  
		Size: 92.7 MB (92719003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272788775f40887c6bc6477a48f04c27c715c5e28ec9975fa3e5c2d8e03d114`  
		Last Modified: Tue, 02 Aug 2022 08:51:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a96e45383b17f140e7d50214f8915f490e2c28182c6f747df41574d41cb2aa`  
		Last Modified: Tue, 02 Aug 2022 08:52:41 GMT  
		Size: 19.5 MB (19515738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce476d9eecd25024c64cb58d4198e713f6cbaad98e2d6605ab5e698a7b2d25f3`  
		Last Modified: Tue, 02 Aug 2022 08:52:38 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c7167209b98b22bd67fa7a56cc36f68aebc00be06ba07514247eba8dfca5bb`  
		Last Modified: Tue, 02 Aug 2022 08:52:39 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbe226123b370804f16d9f65f0ec5f7d1b98e725cdcb49f92510e3355f4acfd`  
		Last Modified: Tue, 02 Aug 2022 09:08:28 GMT  
		Size: 10.9 MB (10909389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0133297f1b09992be3c524c5cf8749b591480acd5e61300ac98077d693c2ad56`  
		Last Modified: Tue, 02 Aug 2022 09:08:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f084e11b6f21282b5b5a0a53010d2ee5f64e36297c4f31acfc6831dbadfb7d99`  
		Last Modified: Tue, 02 Aug 2022 09:08:26 GMT  
		Size: 11.0 MB (10980969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47d6484e9bf2abafbd25999877d20080e30b1dead736dc0d3cfc68fed4e2af8`  
		Last Modified: Tue, 02 Aug 2022 09:08:24 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af298d66bb18f75d855d02f95c3cc4d8f49090200cef43b00e8ee01969bf6f4`  
		Last Modified: Tue, 02 Aug 2022 09:08:24 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5c0165a6829137f30ff432a8b60e0cb35fe69f395ca68000b3562c74e81e79`  
		Last Modified: Tue, 02 Aug 2022 09:08:24 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16989a5b79e5e74bc6e55941eb9856b593a22d4987ee546d7577d1b9b6098f49`  
		Last Modified: Tue, 02 Aug 2022 18:54:41 GMT  
		Size: 2.1 MB (2140749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:979c7a818de42767631d9521cd0517055094d4537a1e72d3df5020a6ea762cfb`  
		Last Modified: Tue, 02 Aug 2022 18:54:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855545875ce0b6ab78bd881434f442c0ba1214e49ea5433851fcaee717bd456`  
		Last Modified: Tue, 02 Aug 2022 18:54:41 GMT  
		Size: 670.4 KB (670423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4646cdb87cbb95c003f358cf5e8ba90b83540926fb932215c87ede3b03c77c49`  
		Last Modified: Tue, 02 Aug 2022 18:54:40 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298d4db3bb26d82236cb275f3efc6f46b08c87c19b4fd2a82ef88fce03d12013`  
		Last Modified: Tue, 02 Aug 2022 18:54:46 GMT  
		Size: 21.8 MB (21778211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache-bullseye` - linux; ppc64le

```console
$ docker pull drupal@sha256:457fb907e6cc58171231f9fbec94f499995e2227071b18dddfd208a9c71398c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189287341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db29805f3e74c48d8c873a404e20043f97c241645e9b696a787efd46c370a3a4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 08:08:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 08:08:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 08:09:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 08:09:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 08:09:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 08:13:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 08:13:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 08:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 08:14:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 08:14:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 08:14:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 08:14:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 08:14:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 11:26:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 02 Aug 2022 12:27:58 GMT
ENV PHP_VERSION=8.0.21
# Tue, 02 Aug 2022 12:27:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.21.tar.xz.asc
# Tue, 02 Aug 2022 12:27:59 GMT
ENV PHP_SHA256=e87a598f157e0cf0606e64382bb91c8b30c47d4a0fc96b2c17ad547a27869b3b
# Tue, 02 Aug 2022 12:28:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 12:28:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:32:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 12:32:12 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:32:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 12:32:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 12:32:13 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 12:32:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:32:14 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 12:32:15 GMT
EXPOSE 80
# Tue, 02 Aug 2022 12:32:15 GMT
CMD ["apache2-foreground"]
# Wed, 03 Aug 2022 12:11:42 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 12:11:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 03 Aug 2022 12:11:43 GMT
COPY file:ebe397bd23f15e762d9b58235d8b4962a65d12542d3be8adc4e774426b23f91d in /usr/local/bin/ 
# Wed, 03 Aug 2022 12:11:43 GMT
ENV DRUPAL_VERSION=9.4.4
# Wed, 03 Aug 2022 12:11:44 GMT
WORKDIR /opt/drupal
# Wed, 03 Aug 2022 12:12:05 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 03 Aug 2022 12:12:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0285aa4963383d13d0bbd4391c2c89c27f5c3b155f8545b585943c2675443754`  
		Last Modified: Tue, 02 Aug 2022 14:35:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb3928a6cac0d782f32f1ad12098fd762f29199a1e22a3a415ed406e68fe8b1`  
		Last Modified: Tue, 02 Aug 2022 14:36:13 GMT  
		Size: 86.6 MB (86633801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f515d8f42d234a23a1cf5c76b59af7ef62ed2945fe55df61c27720a52d846c3`  
		Last Modified: Tue, 02 Aug 2022 14:35:49 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9977d430a7d4a0fa8e6a301ce4957da20fdde8c06ee787221eeafd96bc0613f`  
		Last Modified: Tue, 02 Aug 2022 14:36:56 GMT  
		Size: 20.5 MB (20464668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf954381069d07e3066970bfa08296a3127fd1d7960d93bcf6634c6239f4497`  
		Last Modified: Tue, 02 Aug 2022 14:36:51 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cfb26b4623c191885277856643865ccc75970061a1a497b47d0e295b57dc82`  
		Last Modified: Tue, 02 Aug 2022 14:36:51 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b31170ff826e867a30be92c07fab09d61b641837ee7857fdd199c7f705d701`  
		Last Modified: Tue, 02 Aug 2022 15:03:55 GMT  
		Size: 11.1 MB (11126344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d72745de14e34086658aafe7f84a552347ce4fe3a3a4515153c12d74b1791c`  
		Last Modified: Tue, 02 Aug 2022 15:03:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11fc2607aed756357224ca2a41a51b38a5b2845be8fee33dc19399d665b5dd8`  
		Last Modified: Tue, 02 Aug 2022 15:03:55 GMT  
		Size: 11.1 MB (11139547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759bbed996ad9cddd5bd3f943662a494096839ae277a880912fd896e54b4702d`  
		Last Modified: Tue, 02 Aug 2022 15:03:52 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba51263d347e8f88189d4d77a01325b3ae606c42c9e08f7c4e6d0718bd9d459`  
		Last Modified: Tue, 02 Aug 2022 15:03:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a311ea0f8afdec41c81340d7cce6cfbb2a6c2a9dcfb0348e7ce9a988c906d743`  
		Last Modified: Tue, 02 Aug 2022 15:03:52 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28856e702077e5eb64c668afa4dc0ab8344bfe2537175a0737fd3728ce4f4b24`  
		Last Modified: Wed, 03 Aug 2022 13:09:34 GMT  
		Size: 2.2 MB (2198360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bb9350ed2465b2dd70ae4e06b02f339e69f5acd844290b59e38d6e0f513dc1`  
		Last Modified: Wed, 03 Aug 2022 13:09:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fb54d3a4711c9426861d42f0f8bbe9eb5ca13f935dc1ba348479f60bef818b`  
		Last Modified: Wed, 03 Aug 2022 13:09:34 GMT  
		Size: 670.4 KB (670417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713bc74cce3837690e3b1d898aea92da1a284d9a77ca73acda560ba681454555`  
		Last Modified: Wed, 03 Aug 2022 13:09:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eee495edcae48734af3ba36ecc6095f42b25bebc603d4ca56e848bad77d37ad`  
		Last Modified: Wed, 03 Aug 2022 13:09:54 GMT  
		Size: 21.8 MB (21775374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache-bullseye` - linux; s390x

```console
$ docker pull drupal@sha256:5dc298f0acf8d7aacb6e93feb0dfbb5128249ee2129441c26fc878d44f2e94ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165745750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf61c444ced2f0437a9e76b5e19373548f49ee87c97c13d34e2c6308aea5404`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:49:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 05:49:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 05:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:50:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 05:50:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 05:52:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 05:52:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 05:52:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 05:52:51 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 05:52:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 05:52:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 05:52:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 05:52:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 06:50:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 02 Aug 2022 07:09:25 GMT
ENV PHP_VERSION=8.0.21
# Tue, 02 Aug 2022 07:09:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.21.tar.xz.asc
# Tue, 02 Aug 2022 07:09:25 GMT
ENV PHP_SHA256=e87a598f157e0cf0606e64382bb91c8b30c47d4a0fc96b2c17ad547a27869b3b
# Tue, 02 Aug 2022 07:09:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 07:09:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:11:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 07:11:31 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:11:32 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 07:11:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 07:11:32 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 07:11:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:11:32 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 07:11:32 GMT
EXPOSE 80
# Tue, 02 Aug 2022 07:11:33 GMT
CMD ["apache2-foreground"]
# Tue, 02 Aug 2022 20:43:43 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:43:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Aug 2022 20:43:44 GMT
COPY file:ebe397bd23f15e762d9b58235d8b4962a65d12542d3be8adc4e774426b23f91d in /usr/local/bin/ 
# Tue, 02 Aug 2022 20:43:45 GMT
ENV DRUPAL_VERSION=9.4.4
# Tue, 02 Aug 2022 20:43:45 GMT
WORKDIR /opt/drupal
# Tue, 02 Aug 2022 20:43:58 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 02 Aug 2022 20:44:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46561d2f153c54f55273fe3fc092fca83e6d854850a9d4a3ab9b42af0c76257e`  
		Last Modified: Tue, 02 Aug 2022 07:53:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a771495920d08239931d9aa71868de6a99ed77a1aeadcd174dd0d4ad5136f9`  
		Last Modified: Tue, 02 Aug 2022 07:54:00 GMT  
		Size: 71.6 MB (71623978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f242cce706d4233daf0790086700a1d7a0a18f95dc4093afcbec90e916aab842`  
		Last Modified: Tue, 02 Aug 2022 07:53:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87237ac2ea4191036a23712eb07ba661360f353a3eff2d72bf0c49fac900bf7f`  
		Last Modified: Tue, 02 Aug 2022 07:54:21 GMT  
		Size: 19.1 MB (19071046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddeaa6d5c75e3375a39a4c316b375e69b8c80780efa6202918f7eda0a92db1f4`  
		Last Modified: Tue, 02 Aug 2022 07:54:18 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3fe210b6f35e1524cb22b2b9e91f39bf0092914b7fa0989b4c2151e0cb4d6`  
		Last Modified: Tue, 02 Aug 2022 07:54:18 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a940d3e3afc693c85ccaa9d4e736a8532fc49a827cb016b2116b9799e0f88d`  
		Last Modified: Tue, 02 Aug 2022 08:03:45 GMT  
		Size: 11.1 MB (11125323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cafcea7256b63c884731545f9b079de2a181221875d4e29c2653b5e3ba821b`  
		Last Modified: Tue, 02 Aug 2022 08:03:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93449a90835a67c852e0496b26478d39eaa3a02b97bef2a2bdd3d9ed670050b5`  
		Last Modified: Tue, 02 Aug 2022 08:03:45 GMT  
		Size: 9.9 MB (9926684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70b407d14fc6800fd64141d5248085648b58da8d4cc23d5558bbbb24b4568cf`  
		Last Modified: Tue, 02 Aug 2022 08:03:43 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa8e625f65a23a680795a4babf45abe9f4ee9689ab6bdce2131056db526d6d8`  
		Last Modified: Tue, 02 Aug 2022 08:03:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b99511beacfbacbf7c8abf343fe08714d5e85dbd8eb7e6a74058e18b71d8a65`  
		Last Modified: Tue, 02 Aug 2022 08:03:43 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526771d86aa026bfd838349e60465e793291cf48771558dd91771eb9694aedba`  
		Last Modified: Tue, 02 Aug 2022 21:15:19 GMT  
		Size: 1.9 MB (1906573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cb473c36d11bdb7d8fe4bcebb31eeec8807c931a777e3b81709711b5cea632`  
		Last Modified: Tue, 02 Aug 2022 21:15:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468eb50307c8733f6c2a18ea35f0262de32e0ad01a8b0abc7b486504e15fcf19`  
		Last Modified: Tue, 02 Aug 2022 21:15:19 GMT  
		Size: 670.4 KB (670422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5cadbc8c366cdc7923b5e1d5afbbc521ee3697b0db5cebac774796913d4601`  
		Last Modified: Tue, 02 Aug 2022 21:15:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396a5bc85d1d0036acd82fadc1d4c717242dce5a8ec545865de1a18da003ea78`  
		Last Modified: Tue, 02 Aug 2022 21:15:22 GMT  
		Size: 21.8 MB (21775414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
