## `drupal:7-php8.1-apache-bullseye`

```console
$ docker pull drupal@sha256:8b34dd331671856e6f7ad88dcd0f1877a878f07174e4d725456ec062eac2f95d
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

### `drupal:7-php8.1-apache-bullseye` - linux; amd64

```console
$ docker pull drupal@sha256:d0f48edcf3f4d9e6858794db3a5646a46b6047ca3988d6e1b40f25200b9f6e98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171081625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e51bb99ca0d065ee55ff173c615cc88a77aa7d25d9defe728d2a373865898f6`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:27:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 02:27:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 02:27:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:27:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 02:27:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 02:31:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 02:31:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 02:31:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 02:31:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 02:31:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 02:31:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 02:31:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 02:31:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 03:53:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 03:53:09 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 03:53:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 03:53:09 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 03:53:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 03:53:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:56:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 03:56:16 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:56:16 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 03:56:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 03:56:17 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 03:56:17 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:56:17 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 03:56:17 GMT
EXPOSE 80
# Wed, 16 Aug 2023 03:56:17 GMT
CMD ["apache2-foreground"]
# Thu, 17 Aug 2023 04:55:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 04:55:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 17 Aug 2023 05:06:32 GMT
ENV DRUPAL_VERSION=7.98
# Thu, 17 Aug 2023 05:06:32 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Thu, 17 Aug 2023 05:06:33 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda2313473334ef7a53adde508d570f54649e80dee8e1608dcda3deb493ec79`  
		Last Modified: Wed, 16 Aug 2023 04:32:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362421c67441444258e8bb89d0e3a73c8f451ae88e63d779acf346bd571dd01f`  
		Last Modified: Wed, 16 Aug 2023 04:32:17 GMT  
		Size: 91.6 MB (91635644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e1d184cef7b6c914a1a333c13ec1d13f6bfac91245fab2d2e8119d53c6ffee`  
		Last Modified: Wed, 16 Aug 2023 04:32:04 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38301daa28eb1a7aec64bdd362969e3ff18f098269c1f036518e317a1af7e0a9`  
		Last Modified: Wed, 16 Aug 2023 04:32:34 GMT  
		Size: 19.2 MB (19248159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0adb5f5775772fb23252acb90379b74ce5809905e6fcd05853564f20589e21`  
		Last Modified: Wed, 16 Aug 2023 04:32:32 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6812f652098c26fec25d134794f657aea9bb5235c8f33d6c4afdf7fdc778f4`  
		Last Modified: Wed, 16 Aug 2023 04:32:32 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53653b482e6bab3e64a0d2c3b9e81aa396682012273b0c6b7bf4ca1712a2bf82`  
		Last Modified: Wed, 16 Aug 2023 04:40:34 GMT  
		Size: 12.1 MB (12149935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2efa845bb909a527eaed4c7eee46cb42f22557a2e818412bd9289aa2f319c1`  
		Last Modified: Wed, 16 Aug 2023 04:40:26 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1209792c52e2e074f377e34116be4a3621b64a5dcb8d11ee6d47fe4b52224de`  
		Last Modified: Wed, 16 Aug 2023 04:40:28 GMT  
		Size: 11.1 MB (11074008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594615025f37d5d1a8f74d34f89eae4605acc838e1eff43fbf2519abc3b22bb9`  
		Last Modified: Wed, 16 Aug 2023 04:40:26 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd90d2dedd0706dc5a92ee9d2080da912e0425a2e26556dea45ae1754b106a`  
		Last Modified: Wed, 16 Aug 2023 04:40:26 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7eca44e715687bf6dc5f5dbdcbbccb54dc556dcc7aaf0e3bfd083e95f49dfc`  
		Last Modified: Wed, 16 Aug 2023 04:40:26 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d86aea1c8875a28ce58b1356bbc2208b92515d972de6bed574b993dea1292c`  
		Last Modified: Thu, 17 Aug 2023 05:13:50 GMT  
		Size: 2.1 MB (2139539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcb2bafff155e97f5279a6b7730eb2f169aa3f5ae240caf0ee8c7baa0c334d7`  
		Last Modified: Thu, 17 Aug 2023 05:13:49 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb469d7c0ec1a531edca83c9a2e3dbe9786c54f0770947c8105c511857718bdb`  
		Last Modified: Thu, 17 Aug 2023 05:24:21 GMT  
		Size: 3.4 MB (3410780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; arm variant v5

```console
$ docker pull drupal@sha256:02654fc178950560b6901fe80bbf27895f9687b7bc5ce29154093906a3cf6a77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148439172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b146a07e4a3372892eda148c2058c21a03ff1eb1bef5fabc190e723d3229ef3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:48 GMT
ADD file:3b3acc24aa6c4e5b8cfc525e3f293f633aace75304eaf7d1615d63233866cd66 in / 
# Tue, 15 Aug 2023 23:48:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:39:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 05:39:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 05:39:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:39:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 05:40:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 05:42:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 05:42:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 05:42:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 05:42:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 05:42:56 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 05:42:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 05:42:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 05:42:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 06:57:23 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 06:57:23 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 06:57:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 06:57:24 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 06:57:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 06:57:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:00:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 07:00:53 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:00:54 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 07:00:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 07:00:54 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 07:00:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:00:54 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 07:00:54 GMT
EXPOSE 80
# Wed, 16 Aug 2023 07:00:54 GMT
CMD ["apache2-foreground"]
# Wed, 16 Aug 2023 17:23:25 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:23:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 16 Aug 2023 17:23:26 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 16 Aug 2023 17:23:26 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 16 Aug 2023 17:23:27 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:a1de04ebd80600d150cca674fb676a51a44730027c798fad7415210924b7fed2`  
		Last Modified: Tue, 15 Aug 2023 23:52:15 GMT  
		Size: 28.9 MB (28919119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642b54facc8f2ce6bced5c0e3636ada9a20e04e4ee4dbf65ed5fdc60550cfc2`  
		Last Modified: Wed, 16 Aug 2023 07:21:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5492bd9e4b1a1f4d210ba3a853affc6ea288641bc830454d6c1c42262c6da6ec`  
		Last Modified: Wed, 16 Aug 2023 07:22:14 GMT  
		Size: 73.7 MB (73686772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdae9b456d9478c272d32f411fefcb5ad99f6ac282067b60d9608f5dd8deda9`  
		Last Modified: Wed, 16 Aug 2023 07:21:57 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38083d79a1b7d076797a40970bd13025065d8004f4d1ea2593d80f5f75bb946`  
		Last Modified: Wed, 16 Aug 2023 07:22:35 GMT  
		Size: 18.5 MB (18548501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746c54c7edb0ee96608ab3c50c8702f2812dc31a6c32f20da8d303f037a60bb3`  
		Last Modified: Wed, 16 Aug 2023 07:22:31 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee458b78756083ca8eaad15acee3d567fc7255585c8494f8d47a79c97bc605c7`  
		Last Modified: Wed, 16 Aug 2023 07:22:31 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de60b18a69246ae51d4049b7fd8e80e96ad2dce1e3cb78eccfa6baed3f082f0`  
		Last Modified: Wed, 16 Aug 2023 07:30:30 GMT  
		Size: 12.1 MB (12148384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23042f64d67d83dbe075adde4012bfe262a9d5f31f845661460a061b6bea1bae`  
		Last Modified: Wed, 16 Aug 2023 07:30:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c57b62a8155057d4b279d1e5a2838157f6bad74ed32dba7d4d9d69a24c174f6`  
		Last Modified: Wed, 16 Aug 2023 07:30:29 GMT  
		Size: 10.1 MB (10093578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b65ebf0cd58d9d3c84eadfcf3b5dc9645b9f542d7116fff1cdbd7cfcfda16bb`  
		Last Modified: Wed, 16 Aug 2023 07:30:27 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735604ce0df913719f35883272c0eb20fdc37c9f93f4a06155139dc881e70b5c`  
		Last Modified: Wed, 16 Aug 2023 07:30:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f098b499ba2fcf97115766bcfce3c5d1a31b3ff53a6f06442db41c3d577271e1`  
		Last Modified: Wed, 16 Aug 2023 07:30:27 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcf5cbaf4ba1743e358d43613286f92d1ce81af36b31eb75250099eb8212de3`  
		Last Modified: Wed, 16 Aug 2023 17:29:56 GMT  
		Size: 1.6 MB (1626144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cb20e7216fda93605cd165728c2309221efc86a42cfba6cb1347a815b801ec`  
		Last Modified: Wed, 16 Aug 2023 17:29:56 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ba5e64c4f1a5053bab07aaea4be2bee358f6d8162f163bc64448b210338c8`  
		Last Modified: Wed, 16 Aug 2023 17:29:57 GMT  
		Size: 3.4 MB (3410779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; arm variant v7

```console
$ docker pull drupal@sha256:b835c87e4fb743250018d9ac80c1b72e6bfd17285562b82d75116e73f9ca3190
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140545847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb14dd38ea993673c883133f14117bd47e2f0c9a4a403701afeef05da228f2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:22:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 01:22:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 01:22:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:22:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 01:22:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 01:25:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 01:25:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 01:25:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 01:25:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 01:25:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 01:25:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 01:25:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 01:25:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 02:36:07 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 02:36:07 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 02:36:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 02:36:07 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 02:36:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 02:36:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 02:38:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 02:38:30 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 02:38:30 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 02:38:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 02:38:30 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 02:38:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 02:38:31 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 02:38:31 GMT
EXPOSE 80
# Wed, 16 Aug 2023 02:38:31 GMT
CMD ["apache2-foreground"]
# Thu, 17 Aug 2023 01:57:08 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:57:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 17 Aug 2023 02:07:19 GMT
ENV DRUPAL_VERSION=7.98
# Thu, 17 Aug 2023 02:07:19 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Thu, 17 Aug 2023 02:07:20 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf9baa46b712ba600654d5afbf0be5af14847890661f384e0312546808364c9`  
		Last Modified: Wed, 16 Aug 2023 03:07:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a318f2d8f7d02eab13c10fbad90835b65e4d3982cb2fefb8a9355b0623802e7`  
		Last Modified: Wed, 16 Aug 2023 03:07:35 GMT  
		Size: 69.3 MB (69320327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbed6e12d50649806bca87747bce8fc24efd43bbfa9297d6de240603072711dd`  
		Last Modified: Wed, 16 Aug 2023 03:07:22 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2beb7a7e94f366fdd6d7fbfc554b1ef5008e4c4430d5b8805e13b02ceb3b59f2`  
		Last Modified: Wed, 16 Aug 2023 03:07:53 GMT  
		Size: 18.0 MB (18008034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cdea6c4613ebf51f5518f807692dff5cf193371637d03a0d0809ee5e646bea`  
		Last Modified: Wed, 16 Aug 2023 03:07:50 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a02a657cd612f0f374b9e5316657f319c949f0134033543fa8d44e9ed7731`  
		Last Modified: Wed, 16 Aug 2023 03:07:50 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508655f826c54772547f3325ef113b7e1b2152d1c727e4a74cd7a0f145a0da2a`  
		Last Modified: Wed, 16 Aug 2023 03:16:05 GMT  
		Size: 12.1 MB (12148374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d7e8247849f364cab062942663621b444f8498d445b3a3a70c987645f2250b`  
		Last Modified: Wed, 16 Aug 2023 03:16:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37687775ed19788247cfad127be2f28f9adf0952136ebbb7638a69c2dbd5399c`  
		Last Modified: Wed, 16 Aug 2023 03:16:04 GMT  
		Size: 9.6 MB (9558763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9468980c9b37ca17cffb25bac6240fb62c0e69bd018e8d2ba4e30b29375bbf24`  
		Last Modified: Wed, 16 Aug 2023 03:16:01 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343e9011108a0d4cd3f67b9ed34b52aaf071f1197428c1e9bf864679bba5c791`  
		Last Modified: Wed, 16 Aug 2023 03:16:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd87d5c6932028c86f4d93b908d4b336a63642573083e7dc6560af82a0e01c2d`  
		Last Modified: Wed, 16 Aug 2023 03:16:02 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bfa9b9c83f8b039fb98f44ea351d25ce27c500056a6f81803e4c5ed1f6f3f`  
		Last Modified: Thu, 17 Aug 2023 02:14:45 GMT  
		Size: 1.5 MB (1515042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6edb6eeb94e0d63345b5ea3c9708f7eabf1db375291178ebe63dcbc7fbf315e`  
		Last Modified: Thu, 17 Aug 2023 02:14:44 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca932ebb5021b3c129104666fcb85909c79c53c9374ab67a9fefe84e573a76ef`  
		Last Modified: Thu, 17 Aug 2023 02:25:44 GMT  
		Size: 3.4 MB (3410780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:b08678bac41ab9e67135b38484371a3a59dab5454316a6f08aac83eac1a86717
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165268406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d53e345e95abefb56c59310c35d4bccb094055f2158d6d80e9311ce47b94a1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:36:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 04:36:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 04:37:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:37:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 04:37:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 04:40:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 04:40:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 04:40:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 04:40:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 04:40:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 04:40:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 04:40:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 04:40:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 05:57:31 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 05:57:31 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 05:57:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 05:57:32 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 05:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 05:57:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:00:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 06:00:27 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:00:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 06:00:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 06:00:27 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 06:00:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:00:28 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 06:00:28 GMT
EXPOSE 80
# Wed, 16 Aug 2023 06:00:28 GMT
CMD ["apache2-foreground"]
# Wed, 16 Aug 2023 21:22:30 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:22:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 16 Aug 2023 21:32:24 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 16 Aug 2023 21:32:24 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 16 Aug 2023 21:32:25 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d53169195bf445239992bba4330cc8cc3227e8fbe02b4d67c19ae8bbdc3ecf`  
		Last Modified: Wed, 16 Aug 2023 06:27:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63557276833fc21a5e01b9d70e12b186ffc5469d1c955d46092d1ab9477ec55f`  
		Last Modified: Wed, 16 Aug 2023 06:27:39 GMT  
		Size: 86.9 MB (86928358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b85e802013868fe6d4e61dbe6d9247157c971dbce49042a04acfb8078cd8e71`  
		Last Modified: Wed, 16 Aug 2023 06:27:29 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3fe5a17d0758f1677c7419c7627e3f5ac0ef5d7f917628b50dd7e6271a0891`  
		Last Modified: Wed, 16 Aug 2023 06:27:56 GMT  
		Size: 19.2 MB (19170271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f7769f59fd544babff897c2d129805e07ffbf8e20db9d4b8ffce3af3feaaea`  
		Last Modified: Wed, 16 Aug 2023 06:27:54 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35adf644235166fc75031658fcadcdd5ee58c03ba590533f7102a5ee1e7641`  
		Last Modified: Wed, 16 Aug 2023 06:27:54 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13132f9610ff1e104ca5d01be4de502ec72e5da58ad83df765f9b04c0b193c3`  
		Last Modified: Wed, 16 Aug 2023 06:35:50 GMT  
		Size: 12.1 MB (12149163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e116e0489ce4165910f2e49cbbf4c320d28131889c42a4f946bb1af1bdb63e`  
		Last Modified: Wed, 16 Aug 2023 06:35:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd43f18c84ead3d051078ee84fd336f12bb7ca4319b1f8dcfb643a3cd06f31c`  
		Last Modified: Wed, 16 Aug 2023 06:35:49 GMT  
		Size: 11.1 MB (11141447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7333d5c641d2ca1a4ed93df486ae8d52715e1fcd7443abe195be22035424caa`  
		Last Modified: Wed, 16 Aug 2023 06:35:48 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40794382f7d89a45ccb1780b07b929558a184ae59efb03e6814be3e871e15f3b`  
		Last Modified: Wed, 16 Aug 2023 06:35:48 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e591d51a3c96b0aed3ca1002455e94b45c2ad4448bc4d336e8bf9e3a9973f30`  
		Last Modified: Wed, 16 Aug 2023 06:35:48 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95773c099bfef6506ce1a73872e29382dd9ef5c66021e6d6344b16619be028f0`  
		Last Modified: Wed, 16 Aug 2023 21:39:26 GMT  
		Size: 2.4 MB (2399700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4dd42451621f2904ab7e5c6e9352847a280b534a00af0ee0570967d3c7795e`  
		Last Modified: Wed, 16 Aug 2023 21:39:25 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fd959581b59976a06d44eb7d24fe135948624f3ac505e6993123c45182ac61`  
		Last Modified: Wed, 16 Aug 2023 21:49:18 GMT  
		Size: 3.4 MB (3410781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; 386

```console
$ docker pull drupal@sha256:525b7a67e3c3a7345b87b7c4127d7dab8e38b30ab08f010caae8283fcdd7f144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.9 MB (173930856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd09714453f06725a859eb98df33b20588e4010ee1f8f7656d5cc433783310e5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:09:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 04:09:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 04:10:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:10:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 04:10:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 04:15:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 04:15:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 04:15:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 04:15:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 04:15:56 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 04:15:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 04:15:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 04:15:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 06:32:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 06:32:57 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 06:32:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 06:32:58 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 06:33:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 06:33:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:38:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 06:38:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:38:02 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 06:38:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 06:38:02 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 06:38:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:38:03 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 06:38:03 GMT
EXPOSE 80
# Wed, 16 Aug 2023 06:38:03 GMT
CMD ["apache2-foreground"]
# Wed, 16 Aug 2023 19:13:19 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 19:13:20 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 16 Aug 2023 19:26:28 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 16 Aug 2023 19:26:28 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 16 Aug 2023 19:26:29 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37249c64fc168c98487d1e6f2d9299c48a8aafaa8063585313136ae847cb9f2d`  
		Last Modified: Wed, 16 Aug 2023 07:33:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e280665baa73be4a3cefb31a7eec6824703c568eea84f5d4963410e27c6c1fc3`  
		Last Modified: Wed, 16 Aug 2023 07:33:44 GMT  
		Size: 92.7 MB (92720204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8756f7611e7e26ef36fa6ca6e430aa239bed64204f83df1464f63fa82461b125`  
		Last Modified: Wed, 16 Aug 2023 07:33:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f366aa2b9b4bfec2b184b18c680c594d48cfb4a25ab6ab4a0144eb24b7bb2489`  
		Last Modified: Wed, 16 Aug 2023 07:34:03 GMT  
		Size: 19.7 MB (19737240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2415ee7ae26686a9450a2bc37b14fef1cfda28ef3e9dee1e88d76054c4113725`  
		Last Modified: Wed, 16 Aug 2023 07:33:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272d22fdbff15853341b63f462377fb3557276d2963bdf934ceec56f7371a0f`  
		Last Modified: Wed, 16 Aug 2023 07:33:59 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffdc23516b15cb72753116623320ef1f7430463f596246c96557920bb1b566c`  
		Last Modified: Wed, 16 Aug 2023 07:42:47 GMT  
		Size: 12.1 MB (12149133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f355c7941d4e00191fe86a4ee14a0915849f29016316503773e46f31cb97ec1b`  
		Last Modified: Wed, 16 Aug 2023 07:42:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee806f72cc25ca92a73ba7ae1a9dd0634a6a45184ce498ea62b7388830dbb91`  
		Last Modified: Wed, 16 Aug 2023 07:42:46 GMT  
		Size: 11.3 MB (11306703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cebf567b59b90d10af0c0b6380f751b9cb8ad6a68483609c54723e59d264f1`  
		Last Modified: Wed, 16 Aug 2023 07:42:43 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92359f5c0e55ef1f8562fd3889c8a1afdfa231135080f09836523807cab2b7e`  
		Last Modified: Wed, 16 Aug 2023 07:42:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb281aa67b5be5a34357732d5ca51ac8b2ef3fc3199dd58d8c9606a8b02cbce1`  
		Last Modified: Wed, 16 Aug 2023 07:42:43 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7403457ce0bf646fe3838122e27b1e59a77d80491aa9e19d0786dd672b694777`  
		Last Modified: Wed, 16 Aug 2023 19:34:10 GMT  
		Size: 2.2 MB (2203712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ae6a2560cbd8dd453350a97cc0fff3d818d1709fc752fc57b18452ad623dea`  
		Last Modified: Wed, 16 Aug 2023 19:34:09 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583cf572189a7eee8cb6f873c44099099c90a775c01c0ce80da93db8d8fbc0d3`  
		Last Modified: Wed, 16 Aug 2023 19:45:36 GMT  
		Size: 3.4 MB (3410778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; mips64le

```console
$ docker pull drupal@sha256:4bffc61bcd64d7be7e6a560b6a9a0161b281c4e6da842319dcbcf355c3d6238a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147472986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06dafca6e21b00232f24a56cc4890ac28c493a5121d28ccb65ce04b04b077a4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 16 Aug 2023 00:09:57 GMT
ADD file:55aae3aeab6425dfb2efd03d619656959a01f591b2386ab3d046a6bd69624530 in / 
# Wed, 16 Aug 2023 00:10:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:55:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 01:55:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 01:57:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:57:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 01:57:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 02:12:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 02:12:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 02:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 02:13:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 02:14:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 02:14:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 02:14:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 02:14:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 08:21:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 08:21:13 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 08:21:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 08:21:20 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 08:22:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 08:22:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:36:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 08:36:06 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:36:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 08:36:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 08:36:20 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 08:36:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:36:26 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 08:36:30 GMT
EXPOSE 80
# Wed, 16 Aug 2023 08:36:34 GMT
CMD ["apache2-foreground"]
# Thu, 17 Aug 2023 03:11:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 03:11:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 17 Aug 2023 03:11:44 GMT
ENV DRUPAL_VERSION=7.98
# Thu, 17 Aug 2023 03:11:47 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Thu, 17 Aug 2023 03:11:57 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:7ef62af8109683ee92b199cf210a6e6134ce588b610d2a6b93fc467d34648300`  
		Last Modified: Wed, 16 Aug 2023 00:20:59 GMT  
		Size: 29.6 MB (29634580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd7fe23d582311b7614488754dba5e077fcf4528a6f28770c6cf25e6b59b59d`  
		Last Modified: Wed, 16 Aug 2023 10:04:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73153f8b2ebe947d96f38a2399fd32980c8517037b4b8221630d8e0f9aea456d`  
		Last Modified: Wed, 16 Aug 2023 10:05:43 GMT  
		Size: 71.8 MB (71814760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eb05b65a339176c06cbda4a2aae1a3e78a2477844d94c6b976c8b0c3ae2eea`  
		Last Modified: Wed, 16 Aug 2023 10:04:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86df2ac749f785553187e23d0a3bc44f1e7316d215788bade132b3a9892a8101`  
		Last Modified: Wed, 16 Aug 2023 10:06:14 GMT  
		Size: 18.9 MB (18947014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad7c8fe81aed7fde35babd30c780650733cbfdba14aa85c82cddd6a1c47e10b`  
		Last Modified: Wed, 16 Aug 2023 10:06:01 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f8a3f029e23afb1c059a242639183d3ca9bc07b60f23d0b50c8eb1425d0d22`  
		Last Modified: Wed, 16 Aug 2023 10:06:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6458d555a533e3a92a66c921c6adb576a151d9efe9850c4020bbad5af03d66`  
		Last Modified: Wed, 16 Aug 2023 10:19:36 GMT  
		Size: 11.9 MB (11931127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb841f93d516857458f9aaef3071282327b736f459f4b8b003e1886a5f91373`  
		Last Modified: Wed, 16 Aug 2023 10:19:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a319fd2d4f9ed4ab183edeceeea62d47f82f1e2bcae66bda654ed6c0f8de02`  
		Last Modified: Wed, 16 Aug 2023 10:19:39 GMT  
		Size: 10.2 MB (10218232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9848ad4255a5fde9a824c6efa10a8f21bd55600171cee5c195a15d22cb918109`  
		Last Modified: Wed, 16 Aug 2023 10:19:31 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4d656923e5e87e5c18fe79e566dc0726f3da4655d1472462cb0b4e8c93d106`  
		Last Modified: Wed, 16 Aug 2023 10:19:31 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff05401acea0d20fc4cf3a769047a30d44c23b26db697fc66e181320c20a76e`  
		Last Modified: Wed, 16 Aug 2023 10:19:31 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858992f4328767d50869eb424bfe0fe75ef0c212cae31ae669a57d3bd17544b0`  
		Last Modified: Thu, 17 Aug 2023 03:24:05 GMT  
		Size: 1.5 MB (1511061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39463b5edc20605f23ab75354a8d4066088326aac1512671fdbed910ce9e6a8f`  
		Last Modified: Thu, 17 Aug 2023 03:24:03 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5b8e7fd5a4c5352da22970ab02aac919dc82a625f96097712a1801b3b38037`  
		Last Modified: Thu, 17 Aug 2023 03:24:07 GMT  
		Size: 3.4 MB (3410418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; ppc64le

```console
$ docker pull drupal@sha256:d884c1759ddac842ecfcf521dd1fb501a5435fd7bb4590c0e4ed218cfe166f57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.4 MB (171434374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3686c3d89e0810eb915f1e8de7c32003bf67b7f0f9c45a9cd3a1081cd0d585d4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:50:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 05:50:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 05:51:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:51:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 05:51:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 05:56:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 05:56:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 05:57:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 05:57:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 05:57:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 05:57:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 05:57:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 05:57:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 08:11:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 08:11:20 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 08:11:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 08:11:25 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 08:13:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 08:13:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:21:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 08:21:44 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:21:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 08:21:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 08:21:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 08:21:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:21:50 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 08:21:51 GMT
EXPOSE 80
# Wed, 16 Aug 2023 08:21:53 GMT
CMD ["apache2-foreground"]
# Wed, 16 Aug 2023 23:16:12 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:16:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 16 Aug 2023 23:31:43 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 16 Aug 2023 23:31:43 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 16 Aug 2023 23:31:45 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f58460ae4d1635219c4f43f7c358dbf170607f986471841e24b6e86ef863f`  
		Last Modified: Wed, 16 Aug 2023 09:00:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ae32a73a3814d1a1ec1390af8aec38a4ac117408d90ae3c6eae9d2931a7497`  
		Last Modified: Wed, 16 Aug 2023 09:01:07 GMT  
		Size: 86.6 MB (86634571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa4b52b4a6fef86afdf845012a15a4852c69843e4ced842145a773fcc9e5e47`  
		Last Modified: Wed, 16 Aug 2023 09:00:43 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f852077bc8f4f2db43aaec43c7d51819f6537ef2b45127c6059227e91c1a9bc7`  
		Last Modified: Wed, 16 Aug 2023 09:01:34 GMT  
		Size: 20.5 MB (20463943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08143dcbf44876e4a6df5402434155eb0c5002c6605f811b55dc057b71adb4d2`  
		Last Modified: Wed, 16 Aug 2023 09:01:29 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd883334d37f39daa6c8cb99f53b8b1f255d35601dd514dbc9a311b8eccdb305`  
		Last Modified: Wed, 16 Aug 2023 09:01:29 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a8db520ce01c8af627575c192af3ab97b0bedea4f9a409fb3f8694968d6fc0`  
		Last Modified: Wed, 16 Aug 2023 09:14:35 GMT  
		Size: 12.2 MB (12150096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283e86483ce4b210cf835b8f46c1a2d524f24d7d42d96a7dfc617c11751c2de6`  
		Last Modified: Wed, 16 Aug 2023 09:14:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62418bc2222f622244b1324f1fe943d4c58efa81f75a2f03cb8a50031f0903`  
		Last Modified: Wed, 16 Aug 2023 09:14:37 GMT  
		Size: 11.5 MB (11475938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9180008a1446c07ea5905b21bd110356590903e7efb5d3586e21a5719eceff`  
		Last Modified: Wed, 16 Aug 2023 09:14:31 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7efd33c53284034def63c5d0be0b354baa6a61a98777bcf221ff3a01717a23f`  
		Last Modified: Wed, 16 Aug 2023 09:14:31 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92123f2b3e06478d455e8b297a5295fc672a367103a35e2acb011e899ac88493`  
		Last Modified: Wed, 16 Aug 2023 09:14:31 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149dc6549c1627c54524c27bfc631356868f4cffcb0ef5cab38904d027b7cd93`  
		Last Modified: Wed, 16 Aug 2023 23:44:22 GMT  
		Size: 2.0 MB (2002070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cac76dd48a249afce3176f073d199872cd4919b7d45b09dccdea71c0df5f77`  
		Last Modified: Wed, 16 Aug 2023 23:44:22 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b1a34efb2ca862abed7ce18afad194707a67cc06b39af35e41fcec4f300cc8`  
		Last Modified: Thu, 17 Aug 2023 00:03:49 GMT  
		Size: 3.4 MB (3410781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache-bullseye` - linux; s390x

```console
$ docker pull drupal@sha256:d2e72197e14e0f805d794385e1e64ada7fada487ab45247a73a3261e0b846c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147864103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc41f88e64377a80015feb41ab8776d6258bb8c7c6ec11e7276348a57a98d7f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:41:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 16 Aug 2023 07:41:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 16 Aug 2023 07:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 07:42:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Aug 2023 07:42:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 16 Aug 2023 07:44:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 16 Aug 2023 07:44:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 16 Aug 2023 07:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 16 Aug 2023 07:44:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 16 Aug 2023 07:44:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 16 Aug 2023 07:44:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 07:44:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Aug 2023 07:44:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Aug 2023 08:50:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 16 Aug 2023 08:50:09 GMT
ENV PHP_VERSION=8.1.22
# Wed, 16 Aug 2023 08:50:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Wed, 16 Aug 2023 08:50:09 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Wed, 16 Aug 2023 08:50:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 16 Aug 2023 08:50:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Aug 2023 08:52:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:52:20 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Aug 2023 08:52:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Aug 2023 08:52:20 GMT
STOPSIGNAL SIGWINCH
# Wed, 16 Aug 2023 08:52:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 16 Aug 2023 08:52:21 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 08:52:21 GMT
EXPOSE 80
# Wed, 16 Aug 2023 08:52:21 GMT
CMD ["apache2-foreground"]
# Wed, 16 Aug 2023 19:54:24 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 19:54:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 16 Aug 2023 20:06:21 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 16 Aug 2023 20:06:21 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 16 Aug 2023 20:06:22 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c4a850dbe1eb732c5c97fa54b1ae3648ebfbd750e52ee349967c21bae6f8e4`  
		Last Modified: Wed, 16 Aug 2023 09:11:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d023232c692aed043ea07319147d3143855c6fdc585cc1a41ee97d187e73bda`  
		Last Modified: Wed, 16 Aug 2023 09:12:02 GMT  
		Size: 71.6 MB (71629316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24f3d4c0f53a438b23e1654ed8498530e1b618518300d13c3f0ee7699d7aa9f`  
		Last Modified: Wed, 16 Aug 2023 09:11:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db2469cca674ba85980cf966fab82e8f39867c2dd29cfa34ff480c28e37398`  
		Last Modified: Wed, 16 Aug 2023 09:12:15 GMT  
		Size: 19.1 MB (19077528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d90dfc1bbc0b08d7df1a3a70d284629780e78111a2bcc97beef38d3eae9bd6`  
		Last Modified: Wed, 16 Aug 2023 09:12:12 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740c57f44be5b4f952f6d86b1b5cd85fd6f2d6815ddebf8459c429af09f7698f`  
		Last Modified: Wed, 16 Aug 2023 09:12:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21f026261e0571d5d83c995d7052ed117bf8743464d713d6d432f35f35b81da`  
		Last Modified: Wed, 16 Aug 2023 09:18:46 GMT  
		Size: 12.1 MB (12148784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9e0a83f3bda9d6f3162562a8f1a404a6689b17f573cc1210ba0cbe35f8206`  
		Last Modified: Wed, 16 Aug 2023 09:18:44 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3745b9c600fdab8abf262ab5526b503bc017bf4866899c493ccc18a0d4f599`  
		Last Modified: Wed, 16 Aug 2023 09:18:46 GMT  
		Size: 10.2 MB (10209279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f764f845df197a9f96f4008ab20a329951fbe29c77c12d255649678f245bf`  
		Last Modified: Wed, 16 Aug 2023 09:18:44 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9159e62a21f0ff1a81db69531a10fdd22bf60be41f2c01ff1f811b5e39fb9e5`  
		Last Modified: Wed, 16 Aug 2023 09:18:44 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ed5b8ebe88801b8d65d78649d32703ca13d99f70e00e690fe4248c6cde402d`  
		Last Modified: Wed, 16 Aug 2023 09:18:44 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99af11bb3c1b544c44d56975ad68238dc92818e93048b1d63485ae6d3bc6754`  
		Last Modified: Wed, 16 Aug 2023 20:13:05 GMT  
		Size: 1.7 MB (1729555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df5d02dcb1fb88ce1635cf195202f115d3f8348dbed826ae8b69b051a734c6d`  
		Last Modified: Wed, 16 Aug 2023 20:13:04 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62967ee4b74ed2a86865d1c4b79f1e0561a5fab1228b83eb74a633d9cb6aeeef`  
		Last Modified: Wed, 16 Aug 2023 20:19:57 GMT  
		Size: 3.4 MB (3410782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
