## `drupal:rc-php8.1-apache-buster`

```console
$ docker pull drupal@sha256:1256f25b6bdbb63946685a1a77fc902519f4178b0b8b33782c394f8a51def874
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
$ docker pull drupal@sha256:4ee7a59f26513220b505e9f90e8cf9ab92246ec160260106099dbb5bc097c7ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167402140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9101c6344a70bb8321adb4da0406bd3054c324f93c5fd1d469ac61bff757d6de`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:22:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:22:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:22:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:22:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:25:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:25:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:26:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:26:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:26:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:26:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:26:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:26:01 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 28 May 2022 08:26:02 GMT
ENV PHP_VERSION=8.1.6
# Sat, 28 May 2022 08:26:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Sat, 28 May 2022 08:26:02 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Sat, 28 May 2022 08:26:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 08:26:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 08:29:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 08:29:16 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 08:29:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 08:29:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 08:29:17 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 08:29:17 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 08:29:17 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 08:29:17 GMT
EXPOSE 80
# Sat, 28 May 2022 08:29:18 GMT
CMD ["apache2-foreground"]
# Sun, 29 May 2022 02:23:53 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 02:23:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 May 2022 02:23:54 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sun, 29 May 2022 02:23:54 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sun, 29 May 2022 02:23:54 GMT
WORKDIR /opt/drupal
# Sun, 29 May 2022 02:24:06 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sun, 29 May 2022 02:24:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6a088e191348700971ea8f879b767e613f6e05daab7f01768f01cf4846251`  
		Last Modified: Sat, 28 May 2022 09:52:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a462c113a353741726781679186a05d2b658daf6565a2fe88063ff67ba8e94`  
		Last Modified: Sat, 28 May 2022 09:52:46 GMT  
		Size: 76.7 MB (76683812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907da9f0848a2079665195ba8b00fe90ae716b11f614966f4a44c617a642db13`  
		Last Modified: Sat, 28 May 2022 09:52:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b87c45cce60ddee6f05a5cfde17a04f218e55757f9d8d6e22b912656bb2d2d4`  
		Last Modified: Sat, 28 May 2022 09:53:17 GMT  
		Size: 18.7 MB (18681673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a79f642355cb4bbcd568eddd81b913c4aa864d7c0a5798bb5306539c161a89`  
		Last Modified: Sat, 28 May 2022 09:53:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed4735df7695496064972f978c886ed72455b8baff4a2f3807aec1a075d6c2a`  
		Last Modified: Sat, 28 May 2022 09:53:14 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83b9c830682f25e9a834ede44d15f326bf080db671464aee6c6ba97b9179a6c`  
		Last Modified: Sat, 28 May 2022 09:53:15 GMT  
		Size: 12.0 MB (12047007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa52b66a4bc592988ec7b81e3f12abfb3bfdf3ea1b3dfef0987bf26a5876971`  
		Last Modified: Sat, 28 May 2022 09:53:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcac24e93f8d83f06af9423a98aa5b1f12084acaf0fb157b31d4ea5eb4e4ae7`  
		Last Modified: Sat, 28 May 2022 09:53:14 GMT  
		Size: 11.0 MB (10981802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ad21f814f172138aea2e3b134854335152134c4e2105c763e912447141a069`  
		Last Modified: Sat, 28 May 2022 09:53:12 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633c228a9682b5f88c2692a46c4eebedc48a0b610f61c1cd015cfdf7f0e95e02`  
		Last Modified: Sat, 28 May 2022 09:53:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02ff3b909f6566f63efa9b3c6973fa78b2850bca64faa6e83572cbc0cf4e12`  
		Last Modified: Sat, 28 May 2022 09:53:12 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1644465d202de55236c78ea4430df329a8fe59e28aec6021fff44d386a1e540`  
		Last Modified: Sun, 29 May 2022 02:42:57 GMT  
		Size: 2.1 MB (2082294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8ad5e19a1d0de49d911829f63a51afcdad62cd1247f46051dc87b01233408a`  
		Last Modified: Sun, 29 May 2022 02:42:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6749a673ca1548baea5ac1c2f1d70082427597ae332124d0dec6c82c0b5b0b`  
		Last Modified: Sun, 29 May 2022 02:42:57 GMT  
		Size: 661.6 KB (661586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b55cc72685fade66d1c9aa5b6f8eb295529dffcc05266ffb1c47ccc76affd3d`  
		Last Modified: Sun, 29 May 2022 02:42:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c2722ae9eb7ff38820fd6e46c9031cc84f68a777b3b743b8ce162fb2db8654`  
		Last Modified: Sun, 29 May 2022 02:43:01 GMT  
		Size: 19.1 MB (19117775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:1b569c26127e84dc8c9d48ea0eebc50fa9c62684349a26e15f06d85a025258ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142561777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ee1d4098bc60691463be732799b2afef2e6a458e94efa489c84c55e15024e1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 13:57:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 13:57:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 13:58:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 13:58:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 13:58:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 14:04:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 14:04:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 14:04:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 14:04:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 14:04:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 14:04:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 14:04:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 14:04:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 14:04:28 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 13 May 2022 22:27:03 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 22:27:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 22:27:04 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 22:27:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 22:27:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 22:32:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 22:32:12 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 22:32:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 22:32:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 22:32:14 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 22:32:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 22:32:15 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 22:32:15 GMT
EXPOSE 80
# Fri, 13 May 2022 22:32:16 GMT
CMD ["apache2-foreground"]
# Sat, 14 May 2022 01:53:05 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 May 2022 01:53:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 01:53:07 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 14 May 2022 01:53:08 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 14 May 2022 01:53:08 GMT
WORKDIR /opt/drupal
# Sat, 14 May 2022 01:53:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 14 May 2022 01:53:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a35ae60a85d449da971bdbc6d59854e609e55d181d0b965377366967883d93c`  
		Last Modified: Wed, 11 May 2022 17:30:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a426817eebdd2c479b3443381e193aa0343bd82393a5cb81e1215846033259`  
		Last Modified: Wed, 11 May 2022 17:31:04 GMT  
		Size: 59.5 MB (59538872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56a72f8dff231737568a93846b1289fa47b78e57a507860cb5b976c74dc372a`  
		Last Modified: Wed, 11 May 2022 17:30:27 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e696ab0db3de95432e0fcd726ce11b2289359e0244d8e788fd4ae9a2bb003541`  
		Last Modified: Wed, 11 May 2022 17:31:36 GMT  
		Size: 17.5 MB (17479793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39532b014cd210856aafc982bcbeea8aa59a3cd56ca0f2a0aae0f202e5b38f4`  
		Last Modified: Wed, 11 May 2022 17:31:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aece9ff7b6f33d2fb5aed0d74af006fc4cb485fc5b32fc2105ade6c433d0d57a`  
		Last Modified: Wed, 11 May 2022 17:31:26 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3317226b0dc4feeb919adc84fa8128daa66e8d1721ec8d8e31417aa839cacbcb`  
		Last Modified: Fri, 13 May 2022 23:38:14 GMT  
		Size: 12.0 MB (12045245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2047bc0ec044ac91423104a5f642465cd96b9bbf8e066623cb0daf644f7879`  
		Last Modified: Fri, 13 May 2022 23:38:09 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff2142e4d3affa337b8cfefd2703ff6360ab18da1d07e7a1ca0172339028eb`  
		Last Modified: Fri, 13 May 2022 23:38:16 GMT  
		Size: 9.5 MB (9484990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0081fbf44185c8114e280dbc536fdf49a3843d7aa2a14aa3a8755b6c852b479`  
		Last Modified: Fri, 13 May 2022 23:38:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f2966e6ba44c4d305238c13cf1a56430c97586272259ae1244325c18b4282d`  
		Last Modified: Fri, 13 May 2022 23:38:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d279fbb440b0873983ed920157d2961eb7cb90e9bc9634d3d13567f34523dac`  
		Last Modified: Fri, 13 May 2022 23:38:09 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e20516132a5d716bf3ba1792a70cc766d608c6383fe291772b8c13fe405fa4`  
		Last Modified: Sat, 14 May 2022 02:36:29 GMT  
		Size: 1.5 MB (1479650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86f37df73fc33f6956b9437645d2eccc0d91b6cf589a94deddd29ee669dc2c8`  
		Last Modified: Sat, 14 May 2022 02:36:28 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31207034118594a4c7f0e6f025fb44084f582e044a643176733e907b174c492f`  
		Last Modified: Sat, 14 May 2022 02:36:28 GMT  
		Size: 661.6 KB (661583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d05a18d9498db085e72a365a6c866ecb3417abd7003d734f655a6c3098759ec`  
		Last Modified: Sat, 14 May 2022 02:36:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc05a135918704ee38359f8a7ec80d4c4ceaf14d639acd1c0547bbd4454aa4`  
		Last Modified: Sat, 14 May 2022 02:36:57 GMT  
		Size: 19.1 MB (19117719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:27f679e16e13aa0e313239e2a73b92db1b72462a2360c8f7dac24a39d7411056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.5 MB (159455552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680a81c2160f458b6a42de165a84d8c507139e91d6fcf812ac3c7c1d2353985d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:57:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 04:57:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 04:57:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 04:58:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 04:58:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 05:02:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 05:02:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 05:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 05:02:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 05:02:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 05:02:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 05:02:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 05:02:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 05:02:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 28 May 2022 05:02:28 GMT
ENV PHP_VERSION=8.1.6
# Sat, 28 May 2022 05:02:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Sat, 28 May 2022 05:02:30 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Sat, 28 May 2022 05:02:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 05:02:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 05:06:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 05:06:28 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 05:06:29 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 05:06:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 05:06:30 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 05:06:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 05:06:32 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 05:06:33 GMT
EXPOSE 80
# Sat, 28 May 2022 05:06:34 GMT
CMD ["apache2-foreground"]
# Sat, 28 May 2022 21:35:18 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 21:35:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 May 2022 21:35:20 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 28 May 2022 21:35:20 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 28 May 2022 21:35:21 GMT
WORKDIR /opt/drupal
# Sat, 28 May 2022 21:35:40 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 May 2022 21:35:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68aac919b6108af15c6a38f8dfdd7a5b5b821982f907d310254e3ac075564696`  
		Last Modified: Sat, 28 May 2022 06:34:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f8864a861353b6c73a2d817649ed4affc75b32e821ebfc95289378d5811b5`  
		Last Modified: Sat, 28 May 2022 06:34:14 GMT  
		Size: 70.4 MB (70364250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379e923dd2ca40e8146b160be28d970495c555641741b4239330dcc0b2d8cb7`  
		Last Modified: Sat, 28 May 2022 06:34:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6797f1c48173de46f2843e5e9ec6c7fc41057f0293ac02a1b90c377c7957447`  
		Last Modified: Sat, 28 May 2022 06:34:50 GMT  
		Size: 18.4 MB (18366721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036b68f3d814289148089cafb122ef60701cd2ef89395c3f2f110eab3a9ea307`  
		Last Modified: Sat, 28 May 2022 06:34:48 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ed79eedde9dc7e6d50b870bba30926812fcce0bb09036eeba182ca58a2601b`  
		Last Modified: Sat, 28 May 2022 06:34:48 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976cc7c7059853bd1f418bd8081e5be88e85037a5c8052d54cc0414b2a64cec`  
		Last Modified: Sat, 28 May 2022 06:34:49 GMT  
		Size: 11.8 MB (11832297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ab35b181252245df2f6348fc2078c6ca9072ea13d8e4e7e31a9776e87b6795`  
		Last Modified: Sat, 28 May 2022 06:34:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72595b105ef7e81d8180cb4c4e1941cbedebffe92f4c0c106cad8f9d8adc67b5`  
		Last Modified: Sat, 28 May 2022 06:34:47 GMT  
		Size: 11.1 MB (11052374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7abfd707a81a9c64bf7aa112dc6b83000a2fb37dd59fb7ef5b67c6bda4487e`  
		Last Modified: Sat, 28 May 2022 06:34:46 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a6f92e34bc5613a8e38262d03276d510df49378bd5e2fa8791b8a68af14fa3`  
		Last Modified: Sat, 28 May 2022 06:34:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e17270f71c1b796fe54e779343dfe13bb05889579f1270bb7667807f17171d1`  
		Last Modified: Sat, 28 May 2022 06:34:46 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17f8b2f3b8d040e26d202e598f2e97a539990982b294f065b5972ed6830cae`  
		Last Modified: Sat, 28 May 2022 22:05:07 GMT  
		Size: 2.1 MB (2139246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad44b086d35b9cd57cd7ed999d1d7e8297e9330358ef140b9b6ac7d91e44f7`  
		Last Modified: Sat, 28 May 2022 22:05:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e83e7787a82bf22147012afdcf40669b4669b33adad8260c099019b30a478d`  
		Last Modified: Sat, 28 May 2022 22:05:07 GMT  
		Size: 661.6 KB (661588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5a26f444f8401f2492dbb94cbf7a16359215a75dd890caf4ac9244ad4ee2e`  
		Last Modified: Sat, 28 May 2022 22:05:07 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c743f3ebe2b4201f108ce7aa59ba573dd103d8265e56dca67e392bfd2a05a08`  
		Last Modified: Sat, 28 May 2022 22:05:12 GMT  
		Size: 19.1 MB (19119144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:9550cc7229c08b5dbdf7fd990d94ffe2775a2d8ad8964231a84713868f29f66b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172689876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38cee1b63c8ef46bb6e0ee6289b789201247783017123bd642d2672350e14cf1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 13:07:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 13:07:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 13:08:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 13:08:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 13:08:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 13:11:29 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 13:11:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 13:11:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 13:11:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 13:11:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 13:11:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 13:11:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 13:11:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 13:11:48 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 28 May 2022 13:11:49 GMT
ENV PHP_VERSION=8.1.6
# Sat, 28 May 2022 13:11:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Sat, 28 May 2022 13:11:51 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Sat, 28 May 2022 13:12:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 13:12:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 13:14:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 13:14:49 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 13:14:49 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 13:14:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 13:14:51 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 13:14:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 13:14:53 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 13:14:54 GMT
EXPOSE 80
# Sat, 28 May 2022 13:14:55 GMT
CMD ["apache2-foreground"]
# Sat, 28 May 2022 16:32:31 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:32:32 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 May 2022 16:32:33 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 28 May 2022 16:32:33 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 28 May 2022 16:32:34 GMT
WORKDIR /opt/drupal
# Sat, 28 May 2022 16:32:47 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 May 2022 16:32:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28d79d5aa87168f78db562f5ed522b4ca6e137827ebc56b5406f690e444f67`  
		Last Modified: Sat, 28 May 2022 14:42:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e29d85026bb424319623b6933a017c153d18ee323a49bb6313614946c6b8cb`  
		Last Modified: Sat, 28 May 2022 14:42:28 GMT  
		Size: 81.2 MB (81228806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc3bb47da6bf11574b5f2d9226625a8e1d353b8d852689a648f93c7d91afd1f`  
		Last Modified: Sat, 28 May 2022 14:42:13 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e097677dd04f52be397348ea16b55bf8d1f362582c5c394215b13ae13c8e00a8`  
		Last Modified: Sat, 28 May 2022 14:43:04 GMT  
		Size: 18.9 MB (18900217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd8f1c5a998c7ff0419974de9ef3de0414b9d2d38e356168b0e3d488b828a61`  
		Last Modified: Sat, 28 May 2022 14:43:02 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a30bca68af6466e92c358a037d8164cc496c1d32f34c6776422ba71a0b1962b`  
		Last Modified: Sat, 28 May 2022 14:43:02 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c996fcc9ae7c33880e70bad3cef450074360210919915d6bbd27e62eaaba3a`  
		Last Modified: Sat, 28 May 2022 14:43:03 GMT  
		Size: 11.8 MB (11832824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e67ca81b2089d490b159a1d4d500772461ac2660c34bcc4c1957e1b90229d60`  
		Last Modified: Sat, 28 May 2022 14:42:59 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bd7bfededdbc8cfcc4f866e0dfec5c994957f217fcdddd19bc2f84a1462a45`  
		Last Modified: Sat, 28 May 2022 14:43:02 GMT  
		Size: 11.2 MB (11201054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bc1f8f3675f7294148ba9538efec2aa40e40e02962964ed539e584515e7305`  
		Last Modified: Sat, 28 May 2022 14:42:59 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edc9744c718c940c7af27f78bba782fd0b5a5c4a5a7ce136b81056a8dcf60f2`  
		Last Modified: Sat, 28 May 2022 14:42:59 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e39da1b30a76e7f1b49ec6bf415ad338757b9eb8fb3f5946625f7cb35390193`  
		Last Modified: Sat, 28 May 2022 14:42:59 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd6fa6ea3b6793c57561b95d0bc02491434a03f44af1419b9eb91db30ac7a9`  
		Last Modified: Sat, 28 May 2022 17:00:51 GMT  
		Size: 1.9 MB (1940697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd7b9ea437532354a4967c23195b379729ca19d70bad566bdf62b7a6111d938`  
		Last Modified: Sat, 28 May 2022 17:00:50 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5a972e9508f7f7f1adc0be901434bb14acd3419b10368c5076918b2b7d9ba3`  
		Last Modified: Sat, 28 May 2022 17:00:51 GMT  
		Size: 661.6 KB (661588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264997db22c3d91743a162e255e79697ecc130906582edf29ace1c4ab7ad343f`  
		Last Modified: Sat, 28 May 2022 17:00:50 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe172e8684cb7662f6c92ae42429a4b5fde411645624fc9a7a3569173dfa91b5`  
		Last Modified: Sat, 28 May 2022 17:00:56 GMT  
		Size: 19.1 MB (19119234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:95a59cb73c4c8ce878ac614ac8b01ff894c6c1c1f43ce7a273ae13b1e5a41656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177830856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea1836fcda8fef5c0cd11cac6fb08f7ce6f3ce56a895bdcc98ce229a49d4e7c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:33:31 GMT
ADD file:57fcc3eadd20c2481e373ef3b56a194006f65b3c7ae29bd1747e625efcd89124 in / 
# Wed, 11 May 2022 01:33:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:16:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 16:16:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 16:19:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:19:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 16:19:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 16:25:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 16:25:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 16:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 16:27:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 16:27:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 16:27:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 16:27:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 16:27:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 16:27:37 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 13 May 2022 22:57:36 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 22:57:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 22:57:49 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 22:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 22:59:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 23:05:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 23:05:31 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 23:05:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 23:05:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 23:05:47 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 23:05:48 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 23:05:51 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 23:05:53 GMT
EXPOSE 80
# Fri, 13 May 2022 23:05:55 GMT
CMD ["apache2-foreground"]
# Sat, 14 May 2022 01:02:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 May 2022 01:02:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 01:02:28 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 14 May 2022 01:02:37 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 14 May 2022 01:02:43 GMT
WORKDIR /opt/drupal
# Sat, 14 May 2022 01:03:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 14 May 2022 01:03:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:97c4e3bbd0d14c4a194ce9c48b362e1649c341b249c2ad560738b06fe8576dc3`  
		Last Modified: Wed, 11 May 2022 01:44:06 GMT  
		Size: 30.6 MB (30560544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7294fc5b14f6c2a4cfe653cdcf2bc547c17c3054782e9bfe7ee51f153965fd48`  
		Last Modified: Wed, 11 May 2022 20:04:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9f7b323926d8cbf9887c0b380f52ea1d010441e74daec58aaec10ca276e275`  
		Last Modified: Wed, 11 May 2022 20:04:26 GMT  
		Size: 82.3 MB (82293084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f5e905d9e5d088e7c15fe7b7cb57ddade44e1837ba17cea7a66e3342fec270`  
		Last Modified: Wed, 11 May 2022 20:03:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294704cbdfaaae1559b36a39e54c1f4c564a7eb95491414f70189429395438c0`  
		Last Modified: Wed, 11 May 2022 20:04:56 GMT  
		Size: 19.8 MB (19822420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10325b42411155a4580c7c142734a8e12c8da7a6879e9a72d765fd77ce86f8be`  
		Last Modified: Wed, 11 May 2022 20:04:52 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f51ae9bb9e02424dd59d5394b520c0cabeb4c33fe5de0a8a8076e7141e39a0`  
		Last Modified: Wed, 11 May 2022 20:04:51 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28885ee9a7a2c628897ae69289b8df757c149872d5dea6c2bc97922600ab7b63`  
		Last Modified: Sat, 14 May 2022 00:14:34 GMT  
		Size: 12.0 MB (12046973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331515e9d7bded6698657562faa4953ae7184914c67cb55897bd47059c562119`  
		Last Modified: Sat, 14 May 2022 00:14:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6311a165cf6afd961d07e495e82a3668ab12f7df6f61439d4f2034bfd0debbb2`  
		Last Modified: Sat, 14 May 2022 00:14:33 GMT  
		Size: 11.4 MB (11370888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc51e54597cd60245e286b53b425d4a67ea3d3dcaf8f2d37e42a6dc381ee7f4`  
		Last Modified: Sat, 14 May 2022 00:14:30 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f003723a53343da73aa59d6d55fee9f154f0574cf9ecd694c60f6029bcc58cc`  
		Last Modified: Sat, 14 May 2022 00:14:30 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c58dfc6208c60c703aad786fc8196d92979b68252e128a1f0ceb4ff053a5ae`  
		Last Modified: Sat, 14 May 2022 00:14:30 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811b40dac8451c17bf6fc756f25e6acb49af433e55dc95213fc24189ac72881a`  
		Last Modified: Sat, 14 May 2022 01:58:00 GMT  
		Size: 2.0 MB (1952275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae76ad24854e9a9ddf42663897939c058192d644ae26337707d6a0047399d1f`  
		Last Modified: Sat, 14 May 2022 01:57:57 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee83542e953ad9b832312d9f9c046c9d86ecaec9f824ed63990492f60ac60b73`  
		Last Modified: Sat, 14 May 2022 01:57:57 GMT  
		Size: 661.6 KB (661586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842a4402c71eaf4afcd51492d6a3c5ed454a95f2e257617fbecba28047fb0135`  
		Last Modified: Sat, 14 May 2022 01:57:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e411c8d1361651a21b69f36f1072e771a26c04ce2be864c0742d065c79829dfd`  
		Last Modified: Sat, 14 May 2022 02:00:24 GMT  
		Size: 19.1 MB (19117030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:0dc9870c3839287c84d49657c79c0bdbe5b884cefdabbe12c5136d3f2149d268
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152613866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22fa85b34dbcea8f177487af8887e9f95a99a7bfb60d7fc4ec4ebf92e453a82`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:10:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 09:10:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 09:11:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:11:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 09:11:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 09:13:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 09:13:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 09:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 09:13:38 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 09:13:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 09:13:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:13:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:13:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 09:13:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 13 May 2022 23:13:27 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 23:13:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 23:13:27 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 23:13:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 23:13:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 23:16:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 23:16:48 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 23:16:48 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 23:16:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 23:16:49 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 23:16:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 23:16:49 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 23:16:49 GMT
EXPOSE 80
# Fri, 13 May 2022 23:16:50 GMT
CMD ["apache2-foreground"]
# Sat, 14 May 2022 00:39:22 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 May 2022 00:39:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 00:39:24 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 14 May 2022 00:39:25 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 14 May 2022 00:39:26 GMT
WORKDIR /opt/drupal
# Sat, 14 May 2022 00:40:06 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 14 May 2022 00:40:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525bde4054c9188482f1bc960c8dce2d2b7399ff1c138e471f8ac4c20fa099f`  
		Last Modified: Wed, 11 May 2022 10:55:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd52f3187608b40cd9995c5289500f388c8fdfe08afa7eee1db2c9ea311fa9`  
		Last Modified: Wed, 11 May 2022 10:55:45 GMT  
		Size: 64.7 MB (64726188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dbb2648a936aca9898736e993c8703d18a143eea9dce2246bff8004f51403`  
		Last Modified: Wed, 11 May 2022 10:55:36 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0c375bc76707f8b3ace019a60d158339f16e094b895802aaa25705cdc365bf`  
		Last Modified: Wed, 11 May 2022 10:56:01 GMT  
		Size: 18.5 MB (18524918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c874eb0000d2ccec4d06169bac4f570815ebfa97b51a8568ec5c42402c7116`  
		Last Modified: Wed, 11 May 2022 10:55:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34d6cdedd4a4dc9ae548221c1c0efb09765489a176ddc0d0ea3d1ae62270fa`  
		Last Modified: Wed, 11 May 2022 10:55:58 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f16ff964d614ed81a6a68ac5efb268731903c7eed50ad902d203582fc94f4c7`  
		Last Modified: Sat, 14 May 2022 00:08:52 GMT  
		Size: 12.0 MB (12045543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb7b044a701ff88742679af6c5f9bfb8c278124676a73ac399db590d764c72d`  
		Last Modified: Sat, 14 May 2022 00:08:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a31198385bb9a5556483d70a007eda44631707e1171239e6c77ef2735fa788a`  
		Last Modified: Sat, 14 May 2022 00:08:51 GMT  
		Size: 10.1 MB (10091097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e399e99631b80ad54f58d6eea50ede9d20844abc6caeec806c65832def6dbe`  
		Last Modified: Sat, 14 May 2022 00:08:49 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80744839bbe3f1be8ba3868cd4444cc535689fda8e945e3a99e9a2a6c88dfccc`  
		Last Modified: Sat, 14 May 2022 00:08:49 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143a4dc485baeee135a55178bb3a679da8deecbaa2b9aba4c0a50ee336772664`  
		Last Modified: Sat, 14 May 2022 00:08:49 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefcab7873b3028f26c6d077d0506c0b483035706b1fc56adb4722fcc282032f`  
		Last Modified: Sat, 14 May 2022 01:03:27 GMT  
		Size: 1.7 MB (1682073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eec846461933c39825065dbe7780369fcc360082e60c14571b1470ee04dd85`  
		Last Modified: Sat, 14 May 2022 01:03:27 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8eaf6c45c01132b6e32e27c827a126e1000110c4e650c6f949bff447df4cc8`  
		Last Modified: Sat, 14 May 2022 01:03:27 GMT  
		Size: 661.6 KB (661585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00c365e3bf3d31e5461e0bc0dfbccc22f1346836855af88065929d2f169137`  
		Last Modified: Sat, 14 May 2022 01:03:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6266c2b3e7e50dafe89213c7f78e38a17d1477cfa2b370d86f153a4580b245ab`  
		Last Modified: Sat, 14 May 2022 01:03:31 GMT  
		Size: 19.1 MB (19117664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
