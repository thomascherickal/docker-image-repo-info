## `drupal:php8.1-apache-buster`

```console
$ docker pull drupal@sha256:5232b2e4e0b0a8818ccfe1d36263596d4fdba29cd201e1424852a47d804d942c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:php8.1-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:5e5997b8c0e06dba90348d31ab658fb7d0eabb6bcf43c6789b7544c8e1295b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169467114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f47f2e11b1b75fb3ea38249c0348d697574acb6ef845c11d198bdce1a902a6b`
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
# Wed, 01 Jun 2022 16:26:09 GMT
ENV DRUPAL_VERSION=9.3.14
# Wed, 01 Jun 2022 16:26:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Jun 2022 16:26:19 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 01 Jun 2022 16:26:20 GMT
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
	-	`sha256:b7189e2cb5f09a2a22b3d02ecf18e7cc1c1c6a47209fbf1f3db26feca45003bb`  
		Last Modified: Wed, 01 Jun 2022 16:41:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7970d9ffae31af993bc7670c51be9a7f34a7e7e01d9fc8d380a3b0a4220a326d`  
		Last Modified: Wed, 01 Jun 2022 16:41:29 GMT  
		Size: 21.2 MB (21182751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:0d877a09bd320be9dce0d7bd5af85c36dba956c043a63a5711f1ea63df322b48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144625623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704c5c333826ddd31c763166a49554dbd7a2790c2d071cf944a676d6c5df6736`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:00:54 GMT
ADD file:c89d47099a38749a424760d9c7d3a6e982089455ba9d04140db15ba9eb4cdda1 in / 
# Sat, 28 May 2022 01:00:55 GMT
CMD ["bash"]
# Sun, 29 May 2022 07:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 29 May 2022 07:43:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 29 May 2022 07:44:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 07:44:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 29 May 2022 07:44:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 29 May 2022 07:49:22 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sun, 29 May 2022 07:49:22 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sun, 29 May 2022 07:49:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sun, 29 May 2022 07:49:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sun, 29 May 2022 07:49:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sun, 29 May 2022 07:49:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:49:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:49:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sun, 29 May 2022 07:49:50 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sun, 29 May 2022 07:49:50 GMT
ENV PHP_VERSION=8.1.6
# Sun, 29 May 2022 07:49:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Sun, 29 May 2022 07:49:51 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Sun, 29 May 2022 07:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 29 May 2022 07:50:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 29 May 2022 07:55:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sun, 29 May 2022 07:55:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sun, 29 May 2022 07:55:04 GMT
RUN docker-php-ext-enable sodium
# Sun, 29 May 2022 07:55:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 29 May 2022 07:55:05 GMT
STOPSIGNAL SIGWINCH
# Sun, 29 May 2022 07:55:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sun, 29 May 2022 07:55:06 GMT
WORKDIR /var/www/html
# Sun, 29 May 2022 07:55:06 GMT
EXPOSE 80
# Sun, 29 May 2022 07:55:06 GMT
CMD ["apache2-foreground"]
# Mon, 30 May 2022 01:51:46 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 01:51:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 30 May 2022 01:51:48 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Mon, 30 May 2022 01:57:40 GMT
ENV DRUPAL_VERSION=9.3.13
# Mon, 30 May 2022 01:57:41 GMT
WORKDIR /opt/drupal
# Mon, 30 May 2022 01:58:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 30 May 2022 01:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:e41117292dc8c199b63ae1ec4485358841dbcba68dcbd13f379b66182efe832e`  
		Last Modified: Sat, 28 May 2022 01:16:58 GMT  
		Size: 22.7 MB (22748097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4476e641ba5bca06ca3265e32cd0e1d705a51bf83a8c8dc1d493afda403c490e`  
		Last Modified: Sun, 29 May 2022 10:35:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa8991dfd48a27c38c8bf96a41c5315afb02bbefbc492591cedb2b0ca4187cf`  
		Last Modified: Sun, 29 May 2022 10:35:58 GMT  
		Size: 59.5 MB (59539326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542fc0e311febcb4d1efa92aaef3e0faf6a8f512c1c2d7f3bbd6195d2f9691d8`  
		Last Modified: Sun, 29 May 2022 10:35:21 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae82f69c820b6eb99785ebf2b913a97cf79a9f19efb019aaae07e53eee80079`  
		Last Modified: Sun, 29 May 2022 10:36:45 GMT  
		Size: 17.5 MB (17479645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dae0a9f43ae99f5829b6551447188749f28ec361eb841ae12dd13fbbb62c7b`  
		Last Modified: Sun, 29 May 2022 10:36:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6e72a516f31a4ca72b8bf8e925dd1b6a527241f42afd484cd7a3134f101673`  
		Last Modified: Sun, 29 May 2022 10:36:36 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7720ed1a31973c55d1beeb820e70957037c678a9b1023f8a06cad957361a7c`  
		Last Modified: Sun, 29 May 2022 10:36:39 GMT  
		Size: 12.0 MB (12045259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9057d1b99d6372e3dd0bfb24196b209d4872db678ceff43c89f201bbe5f3eeca`  
		Last Modified: Sun, 29 May 2022 10:36:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf68e6e35ce35e4251307bc696ba34354d2345cdff6c66e8b764377e81eb29`  
		Last Modified: Sun, 29 May 2022 10:36:41 GMT  
		Size: 9.5 MB (9484989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99149b77b45559c046df4d1320f60712890ea221275e8447294eace5e85e11f`  
		Last Modified: Sun, 29 May 2022 10:36:34 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7b91adc36ace7b2851e8ea805045a70d2288e4f0f0b7ddaaf8714d2a9b54f8`  
		Last Modified: Sun, 29 May 2022 10:36:34 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c57b0305a06dbdacfa2acadeccd4072a0afd7b117b337885f51f3ea45ecf4f`  
		Last Modified: Sun, 29 May 2022 10:36:34 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23246345216032c3c8f47e391192bfdf0be92c1ffea68c9651b5ebc522bc833d`  
		Last Modified: Mon, 30 May 2022 02:54:11 GMT  
		Size: 1.5 MB (1479671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f917480fbe164f78586a07979bbbf66096cd35de4750d29932940b659f11a818`  
		Last Modified: Mon, 30 May 2022 02:54:10 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05f7be8835355a027d99e2a07b56d4922e98020f4a63f90a0d6bfe9c8938ea9`  
		Last Modified: Mon, 30 May 2022 02:54:11 GMT  
		Size: 661.6 KB (661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8cbc0fbf7da261f647524cb68ba3a5e66fa3c5496d31048677bd3825df4ef1`  
		Last Modified: Mon, 30 May 2022 02:58:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0838cbb80bc409d7ea02e8db5c97e29780659bd5e58070e8c0a1778153afb1d`  
		Last Modified: Mon, 30 May 2022 02:58:58 GMT  
		Size: 21.2 MB (21180990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:0fa8c1b5c71f4f33bcc6a4909418e53bdfbf905556d23f721fe3d7e3342623f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.5 MB (161520595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1aad9e0b2949e4c0a1f6c6d92c56bf16a2d3b2973a5ae76a347828eb2839aa7`
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
# Wed, 01 Jun 2022 16:46:03 GMT
ENV DRUPAL_VERSION=9.3.14
# Wed, 01 Jun 2022 16:46:04 GMT
WORKDIR /opt/drupal
# Wed, 01 Jun 2022 16:46:27 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 01 Jun 2022 16:46:29 GMT
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
	-	`sha256:8bf2fd989ba5b3015074cbb8b432ae55c07938d64e7392774d99896c80847878`  
		Last Modified: Wed, 01 Jun 2022 17:14:14 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9541c7d8d602a85dcbcce50da5b4c8355ec2f63281c094ee6b7d0ce90add6`  
		Last Modified: Wed, 01 Jun 2022 17:14:20 GMT  
		Size: 21.2 MB (21184186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:4b99e571c7c489b1a2b6bdedfa3657c02cc019b51a37c6f28f7e2ffb2860116b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.8 MB (174754638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794f664e32bd707fcdfa92b0a398b5e1e08d9a2bfb2a15e5a9254cf58fa86ace`
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
# Wed, 01 Jun 2022 16:42:23 GMT
ENV DRUPAL_VERSION=9.3.14
# Wed, 01 Jun 2022 16:42:24 GMT
WORKDIR /opt/drupal
# Wed, 01 Jun 2022 16:42:35 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 01 Jun 2022 16:42:37 GMT
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
	-	`sha256:3b1dbda5e51f6582dbcdfe4957326d4513039f01b5f1ac0e3e831410e848f7b9`  
		Last Modified: Wed, 01 Jun 2022 17:06:57 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1953968983f4860065e8448487a25151cc194db4e8bd0573a8f90f49671b06c6`  
		Last Modified: Wed, 01 Jun 2022 17:07:03 GMT  
		Size: 21.2 MB (21183995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:c3062afcdddd4909537c5b51bbd1257bc5779313738d9b6dadfac831590e2987
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179896924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4448004393fd84be4ab45a41ddfe406d7aba110c4a1e5f49aa1f3fd581c287cc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:23:57 GMT
ADD file:a8c6c897bc64da424049ad04a354d123b0622abda1a56b2725f72de5e4569df8 in / 
# Sat, 28 May 2022 01:24:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:55:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 07:55:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 07:58:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:58:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 07:58:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:05:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:05:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:07:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:07:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:07:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:07:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:07:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:07:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:07:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 28 May 2022 08:07:41 GMT
ENV PHP_VERSION=8.1.6
# Sat, 28 May 2022 08:07:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Sat, 28 May 2022 08:07:46 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Sat, 28 May 2022 08:08:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 08:08:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 08:15:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 08:15:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 08:15:15 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 08:15:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 08:15:17 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 08:15:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 08:15:20 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 08:15:22 GMT
EXPOSE 80
# Sat, 28 May 2022 08:15:25 GMT
CMD ["apache2-foreground"]
# Sun, 29 May 2022 13:01:46 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 13:01:52 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 May 2022 13:01:54 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Wed, 01 Jun 2022 16:22:30 GMT
ENV DRUPAL_VERSION=9.3.14
# Wed, 01 Jun 2022 16:22:35 GMT
WORKDIR /opt/drupal
# Wed, 01 Jun 2022 16:23:05 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 01 Jun 2022 16:23:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:087d40850259bdcd3bee3d5d30d5a2070216727f72c1c9731b514ac3dbf7573e`  
		Last Modified: Sat, 28 May 2022 01:33:30 GMT  
		Size: 30.6 MB (30560238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d86fe312fce5ddf948836fc12f6fc994c03a729e5a25d28588b796d9138571b`  
		Last Modified: Sat, 28 May 2022 11:02:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b42b949e272aa3848050bdb1864a51f94c20b3e267c220203986b6a291111c2`  
		Last Modified: Sat, 28 May 2022 11:02:54 GMT  
		Size: 82.3 MB (82294045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145c718a2732fe16f955570b7ef33cc3abc0c7376a6cd5a7d1371e691110c5dd`  
		Last Modified: Sat, 28 May 2022 11:02:38 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de7b72834bca91dae4299fb53c2ebfffaee448b3e964b20302b00103f813813`  
		Last Modified: Sat, 28 May 2022 11:03:33 GMT  
		Size: 19.8 MB (19822182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c592357329b1e15a1380b75d751bfab1cba35cb59882c3f372bc82851e9b0b`  
		Last Modified: Sat, 28 May 2022 11:03:30 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c219fd80a36121e5106274fa7efdf299e1e63ea06c0228fe634768fa7f66aa`  
		Last Modified: Sat, 28 May 2022 11:03:30 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1624cde6f17feef6432f1a8499dec7a331fd6cefb622017b89cf73ca46fe7`  
		Last Modified: Sat, 28 May 2022 11:03:31 GMT  
		Size: 12.0 MB (12047006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1449d8136ed573919312f393ee14db094547c1c0a9da78b3ee2b88cbc11c9368`  
		Last Modified: Sat, 28 May 2022 11:03:27 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6079b5f5dbda42fda80372112890e527e88a5f707abd760f6f8e3d02e1322d5`  
		Last Modified: Sat, 28 May 2022 11:03:30 GMT  
		Size: 11.4 MB (11370921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7277544e8598dc863900fb9f57c4a5fe5831be355444e1ee4c3d743bb0fbcf76`  
		Last Modified: Sat, 28 May 2022 11:03:27 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e462074e41abf6d33fd93bef9fc6537cb97242d7e720cd9f00baa3ef15784`  
		Last Modified: Sat, 28 May 2022 11:03:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318e7fe365542a2041d06484c103457f7ff0c495b97b14b0def3b828baa7ef30`  
		Last Modified: Sat, 28 May 2022 11:03:27 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a936b8a96e2683c8cbcf38577bfccbe7561914e08c8986e9e9fe0f39931bf1d`  
		Last Modified: Sun, 29 May 2022 14:02:29 GMT  
		Size: 2.0 MB (1952192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6ff4d2a9719cc7672938aa67d52ef4cc792075f2ce505847538346ae7abfc3`  
		Last Modified: Sun, 29 May 2022 14:02:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6022dfb28a488eb528baf1aee477ef06f775c0c3e1352313f23433fc2b5de5`  
		Last Modified: Sun, 29 May 2022 14:02:27 GMT  
		Size: 661.6 KB (661588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d853db263dae87a219288f7c49e4a510c0b946d31ab3fbba4549d89065a95db1`  
		Last Modified: Wed, 01 Jun 2022 17:06:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4dde06017747bb10de54392e735cea6b91a0e001f3b5b387b311e7432de8b`  
		Last Modified: Wed, 01 Jun 2022 17:08:08 GMT  
		Size: 21.2 MB (21182694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:e0e699ee646268a88906e6b3688de707d4c29ace2a5c423a36e54dc66da64317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154679492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c0ef5364dca7c76c38da19156addb1bfeb6f0070082eb83c20e348a0f02f91e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:43:43 GMT
ADD file:eb7d389650b193828480416ddc8257a8dc05bcaba9be79ef2b931e7bbae39bdc in / 
# Sat, 28 May 2022 00:43:45 GMT
CMD ["bash"]
# Sat, 28 May 2022 16:33:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 16:33:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 16:33:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:33:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 16:34:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 16:38:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 16:38:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 16:39:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 16:39:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 16:39:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 16:39:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 16:39:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 16:39:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 16:39:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 28 May 2022 16:39:19 GMT
ENV PHP_VERSION=8.1.6
# Sat, 28 May 2022 16:39:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Sat, 28 May 2022 16:39:20 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Sat, 28 May 2022 16:39:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 16:39:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 16:44:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 16:44:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 16:44:04 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 16:44:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 16:44:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 16:44:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 16:44:06 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 16:44:07 GMT
EXPOSE 80
# Sat, 28 May 2022 16:44:07 GMT
CMD ["apache2-foreground"]
# Sun, 29 May 2022 04:56:04 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 04:56:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 May 2022 04:56:07 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sun, 29 May 2022 05:00:03 GMT
ENV DRUPAL_VERSION=9.3.13
# Sun, 29 May 2022 05:00:03 GMT
WORKDIR /opt/drupal
# Sun, 29 May 2022 05:00:24 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sun, 29 May 2022 05:00:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:94516ab12915ac684a13a2161b8bcaa315b01708a424f29d321971d81ac29a93`  
		Last Modified: Sat, 28 May 2022 00:50:20 GMT  
		Size: 25.8 MB (25758660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a8e809a0c370559278cdde33a8bc08cb6a236d4df2e86b10b7370ec8265428`  
		Last Modified: Sat, 28 May 2022 19:07:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613c3194900e73643d6e79d94846fac4e534dec9c9fcbbb601b3104056c5ab4a`  
		Last Modified: Sat, 28 May 2022 19:07:20 GMT  
		Size: 64.7 MB (64727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd635e75cb9e80cc24362d5658349e6f06fa380380e88bfb940b3ade0cdf11f`  
		Last Modified: Sat, 28 May 2022 19:07:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dd05fb0afea924f5a61201524a81183cbb36fe2e22393a42976c73cd717f51`  
		Last Modified: Sat, 28 May 2022 19:07:48 GMT  
		Size: 18.5 MB (18525128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60db603f3495c85baa87c988a884417becacc39419261ea009e3c2170c07b59`  
		Last Modified: Sat, 28 May 2022 19:07:46 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f54672a1d959f0f343f5424eaf503f6d331caca7152c72e8dddcb5d1d9d445`  
		Last Modified: Sat, 28 May 2022 19:07:46 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90d291005e4106ef910c768cc0bc25650e38b207978d04d56c49cca75860b59`  
		Last Modified: Sat, 28 May 2022 19:07:46 GMT  
		Size: 12.0 MB (12045699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51766717bb2751a25979d9bdae3a4c32675875c005f379484bff3c0fde38818`  
		Last Modified: Sat, 28 May 2022 19:07:44 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebad3e49e27482652c3761c3d4ebb3e7361403685c7dc22ded622ebf5b44554`  
		Last Modified: Sat, 28 May 2022 19:07:46 GMT  
		Size: 10.1 MB (10091263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f92e6be3d357d100ac0d93206cbf4ac38550c669cd98532f60931e0ab3fd9b`  
		Last Modified: Sat, 28 May 2022 19:07:44 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84890ef91253040470b6e06a72f0e373d6da41cb71d2cf1c81e2aa80df1ab79`  
		Last Modified: Sat, 28 May 2022 19:07:44 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a086ef7a602403a9e6459e97a30e40a6a28ffff264931953197bbcc57b2fc18`  
		Last Modified: Sat, 28 May 2022 19:07:44 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a2fc0be1d1e28bebeff6e9af11a5c8e018f047d93a07b64536e1ec19d8b4bf`  
		Last Modified: Sun, 29 May 2022 05:31:33 GMT  
		Size: 1.7 MB (1682263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee4cc3cf13cfc36af0d17c1834154bd1d97063907ad35e9804d509af64a000`  
		Last Modified: Sun, 29 May 2022 05:31:33 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d677803b38b4af585a8d9cf9838277defcb582aa22966df884b8f146c8b3f29f`  
		Last Modified: Sun, 29 May 2022 05:31:33 GMT  
		Size: 661.6 KB (661586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870212e2aa2bf2c715a239e2a95a5c764cd8994595f44e4cae8c27f9c5d60426`  
		Last Modified: Sun, 29 May 2022 05:33:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0628c89ab1de28371d9bf88d51e4cc4a9eb256c29a785fdbcc27713aab0f6b78`  
		Last Modified: Sun, 29 May 2022 05:33:09 GMT  
		Size: 21.2 MB (21181318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
