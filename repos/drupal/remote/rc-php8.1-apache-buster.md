## `drupal:rc-php8.1-apache-buster`

```console
$ docker pull drupal@sha256:7cea68485ea6d657ddee32fa0afaf76b2a87effc38a8434210b655839ee45c91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:rc-php8.1-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:989645339bdeb90481db0a0206a6d9bfeb0f229085f20e195fe3732a4bd19b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167333202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b97f9c0121126467ac2a33257ebe7606179519362e417c3577418f89d296ea`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:35:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:35:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:35:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:35:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:40:22 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:40:22 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:40:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:40:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:40:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:40:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:40:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 01:40:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 01:40:32 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 01:40:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 01:40:33 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 01:40:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 01:40:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 01:45:10 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:45:11 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 01:45:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 01:45:11 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 01:45:11 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:45:11 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 01:45:12 GMT
EXPOSE 80
# Tue, 29 Mar 2022 01:45:12 GMT
CMD ["apache2-foreground"]
# Wed, 30 Mar 2022 07:05:17 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 07:05:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 30 Mar 2022 07:05:18 GMT
COPY file:608f7625682057a8f327a57b0a8d1d350465d3209e7a8c9e119158b6dc4b876a in /usr/local/bin/ 
# Wed, 30 Mar 2022 07:05:18 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Wed, 30 Mar 2022 07:05:18 GMT
WORKDIR /opt/drupal
# Wed, 30 Mar 2022 07:05:31 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 30 Mar 2022 07:05:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06aaf1ec5387845ddcc94eb153bc3a733901de26614b2282b8a7f9006f45c809`  
		Last Modified: Tue, 29 Mar 2022 04:20:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b2105946cdab4a534c758e56a5a2884049a02ff6a5cb2ff88ad6768f0c9f73`  
		Last Modified: Tue, 29 Mar 2022 04:20:22 GMT  
		Size: 76.7 MB (76682671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a086d354f476ae73a8db2e297ba65be4cab8e3985a8168105138199ce2ac726`  
		Last Modified: Tue, 29 Mar 2022 04:20:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f420c9f1275d15a45565c4c79e99603fb9e903034f242a316b8525a0c49cd1`  
		Last Modified: Tue, 29 Mar 2022 04:20:53 GMT  
		Size: 18.7 MB (18681868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b6465e78bc58a18fd4aa86b74355a2b05e995c2df67eb93960f84062fe0365`  
		Last Modified: Tue, 29 Mar 2022 04:20:50 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8647e55467c1b75861a0b8d66ad70172e8d55215faf077120fee92abee5ab`  
		Last Modified: Tue, 29 Mar 2022 04:20:50 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa297f2602468c6b264430487690fe61ce5234561262fd712703c8d3fd3c92c`  
		Last Modified: Tue, 29 Mar 2022 04:20:51 GMT  
		Size: 12.0 MB (12037623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d279976afeb2b8cc99a57128f5b1f8e2d3bb30997e0a305f66ef4dab060e9da7`  
		Last Modified: Tue, 29 Mar 2022 04:20:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff434c32cd52fcc942dc80a1672c06333123f5b9782f1dbb401f00bf7aab323a`  
		Last Modified: Tue, 29 Mar 2022 04:20:49 GMT  
		Size: 11.0 MB (10978882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2943e6fe0c20a0138f0dd85c79f5d9a7b9e1e7878a93162d795903386dc7f51`  
		Last Modified: Tue, 29 Mar 2022 04:20:47 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340a3224a0dbffa0ef0574a73f823abf034472b1165b6d58202ddd7b76f557a2`  
		Last Modified: Tue, 29 Mar 2022 04:20:47 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab7de5d9cc1e69f042db9e35562d25c2b5641372d1a3381af59c0fb2f3d95a0`  
		Last Modified: Tue, 29 Mar 2022 04:20:47 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50dea439f09b4883c3f4613e0d17d3ff881f2e2f78dd551aee7532d9734462`  
		Last Modified: Wed, 30 Mar 2022 07:32:37 GMT  
		Size: 2.1 MB (2081599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3f50862bdaf3072d53234b338080ddca6313f3c79d755197ebe4c4b6d8b21`  
		Last Modified: Wed, 30 Mar 2022 07:32:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe97b6d0c1df380725392a50cf1bee72912a174768aa351653fdec8fa6eb4b4`  
		Last Modified: Wed, 30 Mar 2022 07:32:37 GMT  
		Size: 575.7 KB (575719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223abc42a10586e047559741fe54159ee9b2e6ad9951a6d9928bcf66b8ae3172`  
		Last Modified: Wed, 30 Mar 2022 07:32:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bc33d2a63855976f44e70bc84c0130677343a29d2abd1a0274b893e64bd8ca`  
		Last Modified: Wed, 30 Mar 2022 07:32:50 GMT  
		Size: 19.1 MB (19136822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:6a0f62e71f542d999ed6e6394b5b447dfb50da466668c9648a1301f7e623de25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142484567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc456ade1d94049d23a675145af0005fb61a20819b09b827b34aa40f2f6165b3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:10:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 07:10:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 07:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:11:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 07:11:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 07:16:28 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 07:16:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 07:16:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 07:16:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 07:16:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 07:16:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 07:16:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 07:16:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 07:16:55 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 07:16:55 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 07:16:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 07:16:56 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 07:17:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 07:17:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:22:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 07:22:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:22:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 07:22:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 07:22:05 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 07:22:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:22:06 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 07:22:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:22:07 GMT
CMD ["apache2-foreground"]
# Tue, 29 Mar 2022 11:12:15 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 11:12:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Mar 2022 11:12:19 GMT
COPY file:608f7625682057a8f327a57b0a8d1d350465d3209e7a8c9e119158b6dc4b876a in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:12:20 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Tue, 29 Mar 2022 11:12:21 GMT
WORKDIR /opt/drupal
# Tue, 29 Mar 2022 11:12:54 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 29 Mar 2022 11:12:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f556041af6c4895a5a79a108ad426f4acd68eccc9bbf408e99eeb772ff938b`  
		Last Modified: Tue, 29 Mar 2022 10:33:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ea667d8c453dd32a011a5ffaeec170d3da0c6fba06e88fbb9cdf2af5f10f3`  
		Last Modified: Tue, 29 Mar 2022 10:33:50 GMT  
		Size: 59.5 MB (59537662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5765fdaa2e37d313b63de452eb17cd046fd31ad02071583cabd29fc756235d24`  
		Last Modified: Tue, 29 Mar 2022 10:33:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8b1927e68778c5beb6d84d5877aeaec3433799a0bcd26b386abb63653da8e0`  
		Last Modified: Tue, 29 Mar 2022 10:34:39 GMT  
		Size: 17.5 MB (17479699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0cce00c9e161592ca1c0b01c5c324c83f28e74644cedb885dcd9f123218380`  
		Last Modified: Tue, 29 Mar 2022 10:34:32 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae5aa384d32114d7c63c8d48ec93877f44d1b64ddfd8dd70010af49afccef9e`  
		Last Modified: Tue, 29 Mar 2022 10:34:32 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a541747cd369333a9b345bb9105037c65067b9cad341292c8ecb6623527c3ec2`  
		Last Modified: Tue, 29 Mar 2022 10:34:35 GMT  
		Size: 12.0 MB (12035824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0034fc7336b78cf2ff15cc8bde18de165cc95687e50363a3d18bfa177350a32b`  
		Last Modified: Tue, 29 Mar 2022 10:34:30 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364898fbc7d996be541007590ac24850ab6f2812562c8b9dcb83c3a97aa8e8fc`  
		Last Modified: Tue, 29 Mar 2022 10:34:35 GMT  
		Size: 9.5 MB (9480464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4d7d4cc4e52e07c3ce3d907eb5b04714c241b7cce9ec2626681d0e9bfa76f4`  
		Last Modified: Tue, 29 Mar 2022 10:34:31 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c1cff1ee5c32305fc400f2768dbc26a2c3db0bbce6e81bc02da9e096153838`  
		Last Modified: Tue, 29 Mar 2022 10:34:30 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8cf3dcc9e9c761dab713c6ddf8b0a14164775b2b02709c306a8b11713c024`  
		Last Modified: Tue, 29 Mar 2022 10:34:30 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ce847b4d9b745fbb7615e9fe23ed6d650c375666f03223a33e8c3dd943304e`  
		Last Modified: Tue, 29 Mar 2022 12:25:31 GMT  
		Size: 1.5 MB (1479438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6f7921a8df6ed0dc9a32715e3a973b45eabd04bc85a742ccea1c7c0ec371b4`  
		Last Modified: Tue, 29 Mar 2022 12:25:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fedb250d8da1adac26191c446c4c23923094b6379813a94d3a066fb5a316fd`  
		Last Modified: Tue, 29 Mar 2022 12:25:30 GMT  
		Size: 575.7 KB (575715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d0c827f0e6178be998f5d8b2099c5bdecdcbc0fbcd6c4113e3954d2929e`  
		Last Modified: Tue, 29 Mar 2022 12:25:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f4aa711b7cbd132bae0dc5ed32d5c330e730b976ee954970fc109331dc93d0`  
		Last Modified: Tue, 29 Mar 2022 12:25:57 GMT  
		Size: 19.1 MB (19136660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:18190614b71f6573a2f1f74dc62531dac185f8b6c57235c08801489f02b16ff9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.4 MB (159376985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dfc5385f3096001a11248bd9475b2afac91ca8fd720138357841b242576681`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:23:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 14:23:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 14:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:24:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 14:24:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 14:29:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 17 Mar 2022 14:29:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 17 Mar 2022 14:29:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 17 Mar 2022 14:29:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 17 Mar 2022 14:29:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 17 Mar 2022 14:29:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:29:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:29:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 14:29:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 18:34:00 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 18:34:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 18:34:01 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 18:35:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 18:35:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 18:39:09 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:39:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 18:39:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 18:39:11 GMT
STOPSIGNAL SIGWINCH
# Fri, 18 Mar 2022 18:39:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:39:13 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 18:39:14 GMT
EXPOSE 80
# Fri, 18 Mar 2022 18:39:15 GMT
CMD ["apache2-foreground"]
# Sat, 19 Mar 2022 18:00:48 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 18:00:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 19 Mar 2022 18:00:50 GMT
COPY file:608f7625682057a8f327a57b0a8d1d350465d3209e7a8c9e119158b6dc4b876a in /usr/local/bin/ 
# Sat, 19 Mar 2022 18:00:50 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Sat, 19 Mar 2022 18:00:51 GMT
WORKDIR /opt/drupal
# Sat, 19 Mar 2022 18:01:11 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 19 Mar 2022 18:01:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b6c2b1e25add7315508df3aedb73d3d05b44920510c571e9746aecc9212808`  
		Last Modified: Thu, 17 Mar 2022 18:15:35 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e868294ede19eddb4934c00c242c3b7fb276b81ef1b28e07cacbda2706c1ad`  
		Last Modified: Thu, 17 Mar 2022 18:15:45 GMT  
		Size: 70.4 MB (70359368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21cecb898c34df71bbb62a78234d013af6c31c04b6d6bf2bcf0c9cf1069d2fc`  
		Last Modified: Thu, 17 Mar 2022 18:15:35 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7dc7a0d2c7c7d1d85e505ab920ac92bac4ee86551e940ebf88521342e26613`  
		Last Modified: Thu, 17 Mar 2022 18:16:10 GMT  
		Size: 18.4 MB (18367359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102fc95735c5442daa329317212569c18ced614a911e1f610f0c26d76af43d91`  
		Last Modified: Thu, 17 Mar 2022 18:16:07 GMT  
		Size: 427.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6ac8701c91de368e0b9e76f1e6c7d6e8924b623aaba0a9b4b1933295eae930`  
		Last Modified: Thu, 17 Mar 2022 18:16:07 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998dfedf16ce07e512e9d9c97550bbd710069e1923f79b1e00029f95b7537e84`  
		Last Modified: Fri, 18 Mar 2022 20:32:18 GMT  
		Size: 11.8 MB (11825144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc05b7376d3b60ac68db256eefa425e51dc25dc509072b12beb68b7a2ec4a2ae`  
		Last Modified: Fri, 18 Mar 2022 20:32:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b0e08b3653f11918f501aedb975079fe98195d81e32084b07c874a2a30ae17`  
		Last Modified: Fri, 18 Mar 2022 20:32:17 GMT  
		Size: 11.0 MB (11047289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aea706ef1a258f6e2a31bb1f5e75395baef5faabd9ecf3f71a7aaaf3c4de6f`  
		Last Modified: Fri, 18 Mar 2022 20:32:14 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f26caf8debdde73d046496526e64ab57bec9b8347f0f218d50183abd581606`  
		Last Modified: Fri, 18 Mar 2022 20:32:15 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa61cf0c186f0c342ddcba00c0de7abf73dfe44ce2f8f1e89a312839ed3799c`  
		Last Modified: Fri, 18 Mar 2022 20:32:14 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8787f0adb842e2faa96409eadc064ca8d77acee15535b13b7e2c4c92ba388cf2`  
		Last Modified: Sat, 19 Mar 2022 18:29:54 GMT  
		Size: 2.1 MB (2137153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987dd343aba42b823acb040d9e11816afc116dd9d22598e69e2daba899387d9`  
		Last Modified: Sat, 19 Mar 2022 18:29:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd2bd4403452c5dd20141623a84b70cd9dc43fe1d167a29f26a2cca9fa627d`  
		Last Modified: Sat, 19 Mar 2022 18:29:54 GMT  
		Size: 575.7 KB (575713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4d50161538aced8f411a81fe3575f2252b00110b6e4fa6adf66c5a241730d3`  
		Last Modified: Sat, 19 Mar 2022 18:29:53 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcda4bfc318332f6366bed2d3471a1e01ca7b4c0944e098282bcb43fa6c89f78`  
		Last Modified: Sat, 19 Mar 2022 18:29:59 GMT  
		Size: 19.1 MB (19135974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:009314a20258c93a5d8a60b2ad959bbe51ababbe97f866a162c478db941abc1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172608811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6656027fbe1fc986fa8593c57e0e1033be502cf478673a5813f72d763c123c58`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:27:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:27:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:27:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:27:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:30:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:30:46 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:30:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:30:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:30:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:31:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:31:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:31:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 01:31:03 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 01:31:04 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 01:31:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 01:31:06 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 01:31:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 01:31:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:34:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 01:34:01 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:34:01 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 01:34:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 01:34:03 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 01:34:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:34:05 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 01:34:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 01:34:07 GMT
CMD ["apache2-foreground"]
# Tue, 29 Mar 2022 18:50:52 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:50:52 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Mar 2022 18:50:54 GMT
COPY file:608f7625682057a8f327a57b0a8d1d350465d3209e7a8c9e119158b6dc4b876a in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:50:54 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Tue, 29 Mar 2022 18:50:55 GMT
WORKDIR /opt/drupal
# Tue, 29 Mar 2022 18:51:07 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 29 Mar 2022 18:51:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26744efb8ac6ac4ea62f65e8c1e5f3f3e1c024b735d801cff58b10f51cc6db89`  
		Last Modified: Tue, 29 Mar 2022 03:22:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb567b8a5ad7879f1c802eb0b8da5a9d7f0f86a22b84dee9802f9de37ce55da`  
		Last Modified: Tue, 29 Mar 2022 03:22:44 GMT  
		Size: 81.2 MB (81226947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d46d3fe970ad3502fc4c87f9ebc9ebca4f9e9e782d28dcd9e5525c81fda84b9`  
		Last Modified: Tue, 29 Mar 2022 03:22:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a319804bcac90248b2a9cce78de210ce748b39f902ee7ddc2ddac1870aa7cc4`  
		Last Modified: Tue, 29 Mar 2022 03:23:23 GMT  
		Size: 18.9 MB (18900587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163dd124b62c20d0c98779fcc0821fb462a7a59369cd1e04a38c62d6d2deb07d`  
		Last Modified: Tue, 29 Mar 2022 03:23:21 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b620e562a127cad3eac00c20dc273ed213cabad897bb3ac5b63ed9edd71a39`  
		Last Modified: Tue, 29 Mar 2022 03:23:20 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2489796904ac3ff71f4813cf5e30384e3d290a450cf7ff47bea87269948d12f6`  
		Last Modified: Tue, 29 Mar 2022 03:23:24 GMT  
		Size: 11.8 MB (11825711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e054de9b3fb06933fae883779bf593183c83e686e36f3631363f88865921cf`  
		Last Modified: Tue, 29 Mar 2022 03:23:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a07808562552aa3574a2aed87515d8d2c773b690789326478ede0269f582c`  
		Last Modified: Tue, 29 Mar 2022 03:23:20 GMT  
		Size: 11.2 MB (11195974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636466cbbf594f3009e2aaa18e17d3f927b7543ec6c7ba5f2129dd2f00aca5f3`  
		Last Modified: Tue, 29 Mar 2022 03:23:18 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f46e568b4bf5b6e44c7b2830cb102cf9b3fe4579a47a37e15eba5abf065e87`  
		Last Modified: Tue, 29 Mar 2022 03:23:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397297a57d9784d256ed25d1c27a1846da61fc22624437242fba5959e44c987`  
		Last Modified: Tue, 29 Mar 2022 03:23:18 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd1df827008a605f58d9fbfdffd2753e43521f4d5c05e3699607e80de394cf`  
		Last Modified: Tue, 29 Mar 2022 19:23:58 GMT  
		Size: 1.9 MB (1940360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8debc7f5f9fc2cefc737f0457d46be79a24d6b6f2f750f92b31df908e606e08`  
		Last Modified: Tue, 29 Mar 2022 19:23:58 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36de334e4bacfed64f07cb5f72729235bc36837b0074283814bc2c6cc3a5d1bd`  
		Last Modified: Tue, 29 Mar 2022 19:23:58 GMT  
		Size: 575.7 KB (575715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf2c60f1e9d67e6112b9616bd60d29ab1ffdd409970808473e865f2c12ceb83`  
		Last Modified: Tue, 29 Mar 2022 19:23:58 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e70229e4a715c1e3091be91040c6e6629fb0b4f895620e8bb51e5632dee10d`  
		Last Modified: Tue, 29 Mar 2022 19:24:04 GMT  
		Size: 19.1 MB (19136373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:c8cfd23d012a62f04c3937d82471191d2d04386d4f52381a554674e45cebfd62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177748776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b03876d661ec3536ece5e7d89592dbaa0eee32f4d2426c39b666ff1f1934ec`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 17 Mar 2022 11:19:08 GMT
ADD file:0af430b7759619d4d40ea316f823599879e4f3e0dfc8877bdee731020fb2620d in / 
# Thu, 17 Mar 2022 11:19:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 13:05:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 18 Mar 2022 13:06:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 18 Mar 2022 13:09:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 13:09:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 18 Mar 2022 13:10:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 18 Mar 2022 13:21:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 18 Mar 2022 13:21:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 18 Mar 2022 13:23:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 18 Mar 2022 13:24:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 18 Mar 2022 13:24:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 18 Mar 2022 13:24:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 13:24:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 13:25:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 13:25:29 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 18 Mar 2022 13:25:48 GMT
ENV PHP_VERSION=8.1.4
# Fri, 18 Mar 2022 13:25:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Fri, 18 Mar 2022 13:26:17 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Fri, 18 Mar 2022 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 13:30:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 13:44:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 13:44:29 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 18 Mar 2022 13:44:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 13:44:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 13:44:57 GMT
STOPSIGNAL SIGWINCH
# Fri, 18 Mar 2022 13:45:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 18 Mar 2022 13:45:09 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 13:45:14 GMT
EXPOSE 80
# Fri, 18 Mar 2022 13:45:19 GMT
CMD ["apache2-foreground"]
# Sat, 19 Mar 2022 21:41:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 21:41:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 19 Mar 2022 21:41:16 GMT
COPY file:608f7625682057a8f327a57b0a8d1d350465d3209e7a8c9e119158b6dc4b876a in /usr/local/bin/ 
# Sat, 19 Mar 2022 21:41:18 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Sat, 19 Mar 2022 21:41:21 GMT
WORKDIR /opt/drupal
# Sat, 19 Mar 2022 21:41:49 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 19 Mar 2022 21:41:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:303d92340e7868a8dc0fdad5d6c67a8a819a74a2bc47038b26339d5be6084bf4`  
		Last Modified: Thu, 17 Mar 2022 11:29:21 GMT  
		Size: 30.6 MB (30562350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95837e03838c8ae24a52d68c38795b37884473b490ea69bc17eafa636b3ba1c9`  
		Last Modified: Fri, 18 Mar 2022 19:08:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87fad4279e4b974d5841af7d823d8e2a8efb34882796087c5921f518b60b4bd`  
		Last Modified: Fri, 18 Mar 2022 19:09:30 GMT  
		Size: 82.3 MB (82292018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b519ad0f798f7ad177060f97cc0a7c3ea13a0f1b9f69fe6f1010362f1cfe0ffc`  
		Last Modified: Fri, 18 Mar 2022 19:08:40 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16506baba4d6bc6441f111b3e31b5b4c21ee01074d090d44a1b9f137535d2ab2`  
		Last Modified: Fri, 18 Mar 2022 19:10:22 GMT  
		Size: 19.8 MB (19822377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949209f454014e2ebd6840becffbf3902d266bbd1e7c4e32ab46ad8ef6e378d9`  
		Last Modified: Fri, 18 Mar 2022 19:10:11 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f228ea7940d9b23508de874041860a1b29d79a1e6513c5aac1d4a412d0d5a66`  
		Last Modified: Fri, 18 Mar 2022 19:10:11 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30107dab713748f8261e91d7d9f382d47cdbcd23bc94000a637cf69ec8312346`  
		Last Modified: Fri, 18 Mar 2022 19:10:13 GMT  
		Size: 12.0 MB (12037767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e18fa0b7c6e4e8261af9abd2f7396c9ee697ae283ff1cd5fb9fefc35fe97af`  
		Last Modified: Fri, 18 Mar 2022 19:10:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e75131733e114c2776c6ac16263287b2ccd0bb5c608abbd380003a8a3037981`  
		Last Modified: Fri, 18 Mar 2022 19:10:17 GMT  
		Size: 11.4 MB (11362927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e5f9ad78f937146b5927330003d80858ce9e6cc0768fc048178793733ca4a6`  
		Last Modified: Fri, 18 Mar 2022 19:10:07 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e845e975f2b7649022aafc0357f096cfc29106a58d5cf8d93c6c11a8e4c194c`  
		Last Modified: Fri, 18 Mar 2022 19:10:07 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec66065f619ddfd0fe60b39c77fbd5a11a114d0877820d90fd97e6bf76ba7496`  
		Last Modified: Fri, 18 Mar 2022 19:10:07 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901ac76ebcdba79dde88e760437e29b172bd30c913f6819f138a482d53010bdb`  
		Last Modified: Sat, 19 Mar 2022 22:51:04 GMT  
		Size: 2.0 MB (1952923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b99c9e3d01529c6fff9ecf2ab860084b898baed20d63534cdbe7ac8016dc`  
		Last Modified: Sat, 19 Mar 2022 22:51:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526a17d84912cfd35fa11c7aa6a72ef93db44507ceedd8137970b8d211550294`  
		Last Modified: Sat, 19 Mar 2022 22:51:03 GMT  
		Size: 575.7 KB (575716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd30a1113759cb32247f453905d71998e3e30ccf91c03aa35b49cb40c385b3d`  
		Last Modified: Sat, 19 Mar 2022 22:51:03 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9297e9c17901ea4d45ab0eb6bec03a894075a58a02d65cd6af4482efbb94d`  
		Last Modified: Sat, 19 Mar 2022 22:52:11 GMT  
		Size: 19.1 MB (19136774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:c49f6e71034cbc8f107a42ed2fac30eae3553fd95c11d8fcce0047f1daae235e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.5 MB (152540625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c777cd321988176744a1148094ae0c37d3b27fd076919e54e5d4031c9e184c48`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:31:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 02:31:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 02:32:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 02:32:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:32:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:35:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 02:35:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 02:35:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 02:35:13 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 02:35:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 02:35:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:35:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:35:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 02:35:15 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 02:35:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 02:35:15 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 02:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 02:35:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:37:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 02:37:52 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:37:52 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 02:37:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 02:37:53 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 02:37:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:37:53 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 02:37:53 GMT
EXPOSE 80
# Tue, 29 Mar 2022 02:37:53 GMT
CMD ["apache2-foreground"]
# Wed, 30 Mar 2022 05:17:08 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:17:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 30 Mar 2022 05:17:09 GMT
COPY file:608f7625682057a8f327a57b0a8d1d350465d3209e7a8c9e119158b6dc4b876a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:17:09 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Wed, 30 Mar 2022 05:17:09 GMT
WORKDIR /opt/drupal
# Wed, 30 Mar 2022 05:17:33 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 30 Mar 2022 05:17:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ca7134221cf66991684a407bf8496ecad583606f019c20f22e07fb5f5be6cd`  
		Last Modified: Tue, 29 Mar 2022 04:49:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e9f0aa2e5f11337fe4d0dbcdf4e8bfe7a05fb6aec754b899a4fa3848463b39`  
		Last Modified: Tue, 29 Mar 2022 04:49:12 GMT  
		Size: 64.7 MB (64725556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee73a65ab7adc7d95bd4a3bd07b1d55d5fea7725c60aa9f1a043d5985fef8ce3`  
		Last Modified: Tue, 29 Mar 2022 04:49:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d43b81220559b5543d6e8c02ad046a1d3e5f6c138f326d593d0bdec9cfc34a1`  
		Last Modified: Tue, 29 Mar 2022 04:54:15 GMT  
		Size: 18.5 MB (18524834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554b8201882e657daf0eb48793dd71f92e8cd739c4ce493dc9f8e147660da90`  
		Last Modified: Tue, 29 Mar 2022 04:54:15 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded5b114dc845253be9e7203ed29a4158c59e7aedebca6727008851d5460472f`  
		Last Modified: Tue, 29 Mar 2022 04:54:11 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023a2bb4aa96d9a553ecae2e43f0e02cb71a1253a044b8be368ae12e2a4388be`  
		Last Modified: Tue, 29 Mar 2022 04:54:15 GMT  
		Size: 12.0 MB (12036141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be27fe9eee80e0214baf2c87c534cadbb784a6b125e8414113340e0f7cb72689`  
		Last Modified: Tue, 29 Mar 2022 04:53:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153561411b3179d048df50a1680879fc785182b33940593513fe6fcc10fc4b6`  
		Last Modified: Tue, 29 Mar 2022 04:53:54 GMT  
		Size: 10.1 MB (10087580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9ed86ef7d881c9dd193ce3f24445eb740f94643679e3e237f2313c9be2cda8`  
		Last Modified: Tue, 29 Mar 2022 04:53:54 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7dbb726d4d8d851fdfb317241359338c050ac146e05afad1f6b8982ed343a`  
		Last Modified: Tue, 29 Mar 2022 04:53:54 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3603c0eaf4fdd63e58e0e45cba79689ffe5e25c6729d32eb8a312ddf1f148fee`  
		Last Modified: Tue, 29 Mar 2022 04:53:54 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60e21e1c4ff639618485ad317a49dc8c107c1f8517c54d4dc89ab3cf475d059`  
		Last Modified: Wed, 30 Mar 2022 05:47:18 GMT  
		Size: 1.7 MB (1681830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaea167709a432ecf1772680111acc76657b7b38a903675c1d4051f238424d7`  
		Last Modified: Wed, 30 Mar 2022 05:47:18 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93fe70389c0d75ac6d3b9c92b401fcc12a09b93b908dfbc3358e602d8394721`  
		Last Modified: Wed, 30 Mar 2022 05:47:18 GMT  
		Size: 575.7 KB (575717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed2b00e584bf3d6236433f49655770847283ae2b34f33da629084077ea3e830`  
		Last Modified: Wed, 30 Mar 2022 05:47:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cd13bd1a033408f2e97f2383b4391354da36d1dd6fb659f89a651345e9ece6`  
		Last Modified: Wed, 30 Mar 2022 05:47:22 GMT  
		Size: 19.1 MB (19137011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
