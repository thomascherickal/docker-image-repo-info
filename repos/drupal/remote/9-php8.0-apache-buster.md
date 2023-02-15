## `drupal:9-php8.0-apache-buster`

```console
$ docker pull drupal@sha256:e36c1ab0b10c3416a2b19bd20d5e54d81b022460d8499397336b35eab7956066
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:9-php8.0-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:cd9d78378f577ff7905163a86f41f436f3f730ab21b7913ca5f8002bc7722ad7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90294d35a3fa71bea8738793ecea9033d3abbfd1df76c6eabf69dc8ee695ed4d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:49:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 07:49:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 07:49:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:49:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 07:49:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 07:53:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 07:53:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 07:53:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 07:53:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 07:53:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 07:53:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 07:53:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 07:53:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 08:45:02 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:16:09 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:16:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:16:09 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:16:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 22:16:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:19:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:19:13 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:19:13 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:19:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:19:14 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 22:19:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:19:14 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 22:19:14 GMT
EXPOSE 80
# Tue, 14 Feb 2023 22:19:14 GMT
CMD ["apache2-foreground"]
# Tue, 14 Feb 2023 23:32:53 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 14 Feb 2023 23:32:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 19:43:44 GMT
COPY file:151722a4d2b58546b064de6bf000f03d8e4523c2b44cddc7229b2dce9ac9c49d in /usr/local/bin/ 
# Wed, 15 Feb 2023 19:43:44 GMT
ENV DRUPAL_VERSION=9.5.3
# Wed, 15 Feb 2023 19:43:45 GMT
WORKDIR /opt/drupal
# Wed, 15 Feb 2023 19:43:55 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 15 Feb 2023 19:43:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9563eda87c42a4b9fa8ddab2e79be4418e0e447526bb8239177ada59bf8a357`  
		Last Modified: Thu, 09 Feb 2023 08:59:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8a637b1e9aa1c4bcf8eacb22ef65b17fb87a4f25dcbfd6df48b2ab450756bb`  
		Last Modified: Thu, 09 Feb 2023 08:59:59 GMT  
		Size: 76.7 MB (76688156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca25fc3341de160e527afa62a08d4cb2090ca2cdc40a34b86e99817c3a1dc7c`  
		Last Modified: Thu, 09 Feb 2023 08:59:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9b8d28368ade139c241f2ac0828b0135735aeac716e648d510504d208977c1`  
		Last Modified: Thu, 09 Feb 2023 09:00:33 GMT  
		Size: 18.7 MB (18684914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01585489eea31313c2cc70727ca6b5b1ce690d56ea1bd2a4f6fecb5fd997f10`  
		Last Modified: Thu, 09 Feb 2023 09:00:30 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59db89ad06ab376c68eec6887e6b118bda8c3c2a411e87fe49ea5854dbd77b23`  
		Last Modified: Thu, 09 Feb 2023 09:00:31 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8eb9c9286a240be91b46f5276cb0bdb03cba89d6c6d3481b5680b22187140a1`  
		Last Modified: Tue, 14 Feb 2023 22:52:14 GMT  
		Size: 11.1 MB (11141034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a6daffd93b5a30f8b95d95e35307197c4bd8499226f5ac937b68821edc77bf`  
		Last Modified: Tue, 14 Feb 2023 22:52:12 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfda3d892297e3d504f690cef2d15140cd7aeceac5b75e8ff81d50d215c95f9e`  
		Last Modified: Tue, 14 Feb 2023 22:52:13 GMT  
		Size: 10.7 MB (10726431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4530a307983c2263cf417cf105d4e8b15195a3bdb9f373a8878f7e79442e72`  
		Last Modified: Tue, 14 Feb 2023 22:52:12 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9aeef29cefb0495e900ef90dc8166c8d00d5c120fa016791c629ef84a93fca0`  
		Last Modified: Tue, 14 Feb 2023 22:52:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcac38c19f83759b4425e340a91eb1d2de6509c9752eb7b9ae5ca737632ea3e`  
		Last Modified: Tue, 14 Feb 2023 22:52:12 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1614431de23eada280ff433691a3edb0fa9a7d681f709b332653bf68c614d`  
		Last Modified: Tue, 14 Feb 2023 23:54:54 GMT  
		Size: 2.2 MB (2247796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663c283b507c1a373981532447eeb84855bbb5ec4d710534a29192f37b2fc335`  
		Last Modified: Tue, 14 Feb 2023 23:54:54 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c27375f9f236b176e585347e2cd1c66a8be71d47075b680c3267957e4838cf`  
		Last Modified: Wed, 15 Feb 2023 20:03:44 GMT  
		Size: 697.1 KB (697149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a2d1f7a021cd52c217e7964b22e95f8cb9421c6a61f3298ef2326e12ee08ad`  
		Last Modified: Wed, 15 Feb 2023 20:03:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064de000c551c8c59ce4081a71ddaf4e52eaa2361b0cea69c1aada2b06ba7f5c`  
		Last Modified: Wed, 15 Feb 2023 20:03:49 GMT  
		Size: 22.8 MB (22844887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:875830b91a1b1d483cff0dd07adf52ffdfa90d81d94bf0b1d7bf74593a9a5e98
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.3 MB (145348075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d56c5e1164596758899f9b5eb83dd473aadd18463da2e305a938e137e3bcc8b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:44 GMT
ADD file:a8ec6525d364d668c197a3a8a8122778806534f0c87fa3282ea2ce6529c397fc in / 
# Thu, 09 Feb 2023 06:12:45 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:01:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 09:01:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 09:01:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:01:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 09:01:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 09:05:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 09:05:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 09:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 09:05:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 09:05:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 09:05:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 09:05:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 09:05:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 09:58:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 15 Feb 2023 00:38:25 GMT
ENV PHP_VERSION=8.0.28
# Wed, 15 Feb 2023 00:38:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 15 Feb 2023 00:38:25 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 15 Feb 2023 00:38:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 15 Feb 2023 00:38:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 15 Feb 2023 00:40:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 15 Feb 2023 00:40:58 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 15 Feb 2023 00:40:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 15 Feb 2023 00:40:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 15 Feb 2023 00:40:59 GMT
STOPSIGNAL SIGWINCH
# Wed, 15 Feb 2023 00:40:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 15 Feb 2023 00:40:59 GMT
WORKDIR /var/www/html
# Wed, 15 Feb 2023 00:41:00 GMT
EXPOSE 80
# Wed, 15 Feb 2023 00:41:00 GMT
CMD ["apache2-foreground"]
# Wed, 15 Feb 2023 02:06:47 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Feb 2023 02:06:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 02:06:47 GMT
COPY file:eabda45ae71a4b9525aa8464965ff1caf882c63cab948e2e2ee1aa3eca48001e in /usr/local/bin/ 
# Wed, 15 Feb 2023 02:06:47 GMT
ENV DRUPAL_VERSION=9.5.3
# Wed, 15 Feb 2023 02:06:47 GMT
WORKDIR /opt/drupal
# Wed, 15 Feb 2023 02:07:12 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 15 Feb 2023 02:07:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:af790c31932b6069892469d33f363a5c03459bd259d72ae9e08431e6419ae97e`  
		Last Modified: Thu, 09 Feb 2023 06:20:10 GMT  
		Size: 22.7 MB (22749083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c46739b61e0bd9c549ae9e0acfae73a624a6cd3a91b18a1ffde294637e23f82`  
		Last Modified: Thu, 09 Feb 2023 10:20:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a59fb0f14168096f5ea048b6a311df3bf53ddb46909ee76c7cbff814598183`  
		Last Modified: Thu, 09 Feb 2023 10:20:44 GMT  
		Size: 59.5 MB (59541419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c7942b5cce86955141373bb501b4e616065a5d6bca57fcffa023e7f930dc2f`  
		Last Modified: Thu, 09 Feb 2023 10:20:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332bc604555eba9a948ec449ba8e57c9c193be167559e43e7fba5c8ec7f7f63e`  
		Last Modified: Thu, 09 Feb 2023 10:21:22 GMT  
		Size: 17.5 MB (17481480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf16c291b5b9de3502ea448e0c346adc647e94e9957dc8e4e664ae16cdfa8a0`  
		Last Modified: Thu, 09 Feb 2023 10:21:19 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a17af4a3a86cacd3fbdb67fd61bf1e36493bac024555b54ab3bc500c7094e7e`  
		Last Modified: Thu, 09 Feb 2023 10:21:19 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6650a84ccf77490ce77ff701129a49d650ee9002a5be7bdb527186b5f9c99b68`  
		Last Modified: Wed, 15 Feb 2023 01:20:56 GMT  
		Size: 11.1 MB (11138891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92100e7a00c58d8db833a246ad4b5b2423e9741913d0333e35345172a1dfda2c`  
		Last Modified: Wed, 15 Feb 2023 01:20:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f7d26a787aa7a5f9e9f08ccc1602cbc5390ff2a41854d29cd8d72410976272`  
		Last Modified: Wed, 15 Feb 2023 01:20:55 GMT  
		Size: 9.3 MB (9256563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddeb30e814b9518c50dcfdf373d6a9c1c3c64fa2030c50c58557a5371e0d8581`  
		Last Modified: Wed, 15 Feb 2023 01:20:54 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0209fdecc091c47911d6b08f9e0f8ae2a214f35ad162cd75d150d9f4e0b7ad0e`  
		Last Modified: Wed, 15 Feb 2023 01:20:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3144d6d294072808361f7d7584cbf1df62b82f98549877debb30a0e94fa7bb65`  
		Last Modified: Wed, 15 Feb 2023 01:20:53 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bba0a106ca3d84bfd5d9e6b2e11f5af615679e7d05f5a05f76b5014befaae59`  
		Last Modified: Wed, 15 Feb 2023 02:43:36 GMT  
		Size: 1.6 MB (1633083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b5320276ddc28a6e4148364660c78a5483b5638675ce59af4d26791e16be2c`  
		Last Modified: Wed, 15 Feb 2023 02:43:36 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165faebf64664a2a2f41749c60e0471e284742992489b6865f2ea7b416ca5ba8`  
		Last Modified: Wed, 15 Feb 2023 02:43:36 GMT  
		Size: 697.1 KB (697134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f2873bfca7d03db73aa44cdef4eaec52f7130899eb8e6e4786d5e0d0ea0864`  
		Last Modified: Wed, 15 Feb 2023 02:43:36 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127d3ce202577283b88f65e6712ffd90655f1df970df443c3fef6939198679a2`  
		Last Modified: Wed, 15 Feb 2023 02:43:44 GMT  
		Size: 22.8 MB (22844542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:f17f48cfab18adc396da71ce3f931c61634164787ef85dbaf51413d860a1d98a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.7 MB (161658873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ba45e6dc87797af70d78f2c8c437c3ea3beba442577f9d4c74929128a7edc7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:39:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 05:39:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 05:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:40:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 05:40:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 05:43:05 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 05:43:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 05:43:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 05:43:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 05:43:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 06:27:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:33:25 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:33:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:33:25 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:33:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 22:33:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:35:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:35:32 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:35:32 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:35:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:35:32 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 22:35:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:35:32 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 22:35:32 GMT
EXPOSE 80
# Tue, 14 Feb 2023 22:35:33 GMT
CMD ["apache2-foreground"]
# Tue, 14 Feb 2023 23:50:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 14 Feb 2023 23:50:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 20:02:47 GMT
COPY file:151722a4d2b58546b064de6bf000f03d8e4523c2b44cddc7229b2dce9ac9c49d in /usr/local/bin/ 
# Wed, 15 Feb 2023 20:02:47 GMT
ENV DRUPAL_VERSION=9.5.3
# Wed, 15 Feb 2023 20:02:47 GMT
WORKDIR /opt/drupal
# Wed, 15 Feb 2023 20:03:11 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 15 Feb 2023 20:03:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb59936b35f83df7e783b83adade014dde2600b8c66c7f156646724c0590c7a`  
		Last Modified: Thu, 09 Feb 2023 06:39:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483b7b021f35118cd09f08960f1af17be5a48449550af0f339bed3b0827a9baf`  
		Last Modified: Thu, 09 Feb 2023 06:39:44 GMT  
		Size: 70.4 MB (70362430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c942918fd594cbfd67ad58a43f5f196e39ee36cd9395c7d0b3a87ebfb96e9`  
		Last Modified: Thu, 09 Feb 2023 06:39:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524358ce06edb34679f90c7960a1ae16533f51329eda372d0fef9d3e4b77970c`  
		Last Modified: Thu, 09 Feb 2023 06:40:11 GMT  
		Size: 18.6 MB (18583841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50b57b27c058d020a4257f4c0fc8b20fa0fc5d6ef54d70240156d936d24c797`  
		Last Modified: Thu, 09 Feb 2023 06:40:08 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa49151627f6be68378b677fd0734801eea966b8fff3c12e2f042449b02133`  
		Last Modified: Thu, 09 Feb 2023 06:40:08 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79125cb4669239dc5e042849214d93e8e3db71a9691c20a313214ca397384c5d`  
		Last Modified: Tue, 14 Feb 2023 23:03:27 GMT  
		Size: 11.1 MB (11139763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08950398fdc868a98732c313568df3f064ac9534987b1f8aff4d20c742934a18`  
		Last Modified: Tue, 14 Feb 2023 23:03:25 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5deb9e55e6b274be3406befb283d6f477b77c4b17a98c3e8d273558d94bfba`  
		Last Modified: Tue, 14 Feb 2023 23:03:27 GMT  
		Size: 10.2 MB (10201830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38677f55f2f859aa81f6b1359c90803ae354ffa2956b7ac5a8c60b898ab3c289`  
		Last Modified: Tue, 14 Feb 2023 23:03:25 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6420432a86ae056ed9dd907b44e3352333251bc514660d7ae15e02fb93548b1c`  
		Last Modified: Tue, 14 Feb 2023 23:03:25 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bedf9aadb38fbf1bc89e78f823050ea4b6e4f46d6826c10fa87bc7af6e2255`  
		Last Modified: Tue, 14 Feb 2023 23:03:25 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbacc9351ceba6f3116e9370d755970df9e0fbb26fdd324ebbba0c6383a8c3db`  
		Last Modified: Wed, 15 Feb 2023 00:11:54 GMT  
		Size: 1.9 MB (1900238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae14965dd1581021df562f9864fe4367bd209c3a8809c4245f446769119b433`  
		Last Modified: Wed, 15 Feb 2023 00:11:54 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde7c69b38f0f455c182879bd3667dbd46f63694ee5a5595c42663bed2d187c6`  
		Last Modified: Wed, 15 Feb 2023 20:23:19 GMT  
		Size: 697.1 KB (697143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a13c8fa163d1a8ef29a87d9f93d6b0aa9d93b53ac38f0daaa093cf619148577`  
		Last Modified: Wed, 15 Feb 2023 20:23:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f93af286a01ecdc37b4051ce71e173a6e1a71b082bc8d88f6b1be45973c017`  
		Last Modified: Wed, 15 Feb 2023 20:23:23 GMT  
		Size: 22.8 MB (22844761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:c3ac4f5e1eca25f7377f27048f8fd08ea93ca06693f9dbb1c92be7882f119b3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175445169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f28886d5f8c92eba27f50aa0551892ca4061989b17058a64fe6b1619b4b32f9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 05:13:20 GMT
ADD file:2d19c71df422a9624e6fb34d6f87307703e1eaa800067eb1c594dd2b1778980f in / 
# Thu, 09 Feb 2023 05:13:21 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:48:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 06:48:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 06:48:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:48:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 06:48:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 06:52:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 06:52:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 06:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 06:52:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 06:52:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 06:52:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 06:52:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 06:52:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 07:42:57 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:33:14 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:33:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:33:16 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:33:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 22:33:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:36:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:36:05 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:36:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:36:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:36:07 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 22:36:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:36:09 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 22:36:10 GMT
EXPOSE 80
# Tue, 14 Feb 2023 22:36:11 GMT
CMD ["apache2-foreground"]
# Tue, 14 Feb 2023 23:55:21 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 14 Feb 2023 23:55:22 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 14 Feb 2023 23:55:24 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Tue, 14 Feb 2023 23:55:24 GMT
ENV DRUPAL_VERSION=9.5.3
# Tue, 14 Feb 2023 23:55:25 GMT
WORKDIR /opt/drupal
# Tue, 14 Feb 2023 23:55:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 14 Feb 2023 23:55:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:bacc4719e321895e65d456a3375ac7c1f594877d62056057ca20a3229ce824cd`  
		Last Modified: Thu, 09 Feb 2023 05:19:30 GMT  
		Size: 27.8 MB (27798198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e636df26c1ee371547725749130d6da89a612c5b1065b557945a1b1b070cbb51`  
		Last Modified: Thu, 09 Feb 2023 08:01:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851c6d96035d75f03084067fa543a0952ed24fe2b6d97df61cd3f63324d18b6e`  
		Last Modified: Thu, 09 Feb 2023 08:01:32 GMT  
		Size: 81.2 MB (81235683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0982858ffdde6edd4d8b77b2d45ce55f8cacd5b7ca4a1cc7c69069b20f570fb1`  
		Last Modified: Thu, 09 Feb 2023 08:01:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c6d2ba603906ba91a8ff1ac804e6196a27eb5d491383607e79525246744d07`  
		Last Modified: Thu, 09 Feb 2023 08:02:06 GMT  
		Size: 18.9 MB (18900811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28ed35bb5d20834320b0ab42b63d1b0cca9ec7f170cb79fe47c3cd76d020d24`  
		Last Modified: Thu, 09 Feb 2023 08:02:03 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5843fda39dc6740c037b34490a3a014fb589e3b4cbea4acd4b67650207e48dc`  
		Last Modified: Thu, 09 Feb 2023 08:02:03 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45a245651dee1e36f77a795f74c6ca88f86fe3eec545d2f9dbe3be3e0a2215f`  
		Last Modified: Tue, 14 Feb 2023 23:15:28 GMT  
		Size: 10.9 MB (10926471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bef2268585820e2a097e643ac60e88e968035c24e5a83f2103c4eca7b1a24b8`  
		Last Modified: Tue, 14 Feb 2023 23:15:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258d6e67695f8ace0212dac12e7513ce72feab84a5920f59a3e6f6bc2723eed7`  
		Last Modified: Tue, 14 Feb 2023 23:15:26 GMT  
		Size: 10.9 MB (10937159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f646e2738bf525aa8073970eae9683316add1e2ab2c41a9f6fa60712b66f46`  
		Last Modified: Tue, 14 Feb 2023 23:15:24 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5602e1285002c960f5dc5115ad4eea842ef7b0f54d810d163a5ea2dd3b375477`  
		Last Modified: Tue, 14 Feb 2023 23:15:24 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9e0525379d0408f36a9d0ec521c3b42e96eb7b7a6250282303a5fbc7f2c2bc`  
		Last Modified: Tue, 14 Feb 2023 23:15:24 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783b825253ccf0603ad9f0e3e4b3c1d09916c2600a98b2ed727f37a144632ccd`  
		Last Modified: Wed, 15 Feb 2023 00:26:28 GMT  
		Size: 2.1 MB (2102365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e023d62f2d71f2d8d7e7a02fab7f9b7e289faec3a1108ba0120d82cab53c7f31`  
		Last Modified: Wed, 15 Feb 2023 00:26:27 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06519d99e492e1a20604183bf220443cb750c44aa3c7fda7a9ff8d0b3b0beb40`  
		Last Modified: Wed, 15 Feb 2023 00:26:28 GMT  
		Size: 695.2 KB (695204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6747ca74245fc3f0b673d4e5154378a54c5740bd34288e1a032f0c8cfed9ff21`  
		Last Modified: Wed, 15 Feb 2023 00:26:27 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae56103b50e5559d952509b92f24f2ee6ccad57e90daa6a135e3575eeb408ada`  
		Last Modified: Wed, 15 Feb 2023 00:26:33 GMT  
		Size: 22.8 MB (22843394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
