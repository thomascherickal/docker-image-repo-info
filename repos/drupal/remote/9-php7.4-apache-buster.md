## `drupal:9-php7.4-apache-buster`

```console
$ docker pull drupal@sha256:38f777f476ac6f091559e0877eabeef1ead6b74fe20ded45f718def0c80fe1b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:9-php7.4-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:8a509d30c61fc57be0e4b01079c2a20f3c50be9f6702d8e49d6a7915cfca89e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169006329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cbc7963351f5853bd079991b5de19583834f8390c7de4a2ad28abfaa88de32`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 14:09:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 14:09:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 14:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 14:10:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 14:10:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 14:18:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 28 Sep 2021 14:18:00 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 28 Sep 2021 14:18:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 28 Sep 2021 14:18:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 28 Sep 2021 14:18:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 28 Sep 2021 14:18:16 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 28 Sep 2021 14:18:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 28 Sep 2021 14:18:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 14:18:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 14:18:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 16:12:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 16:12:56 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 16:12:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 16:12:56 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 16:13:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 16:13:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:16:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 16:16:26 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:16:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 16:16:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 16:16:27 GMT
STOPSIGNAL SIGWINCH
# Tue, 28 Sep 2021 16:16:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 28 Sep 2021 16:16:27 GMT
WORKDIR /var/www/html
# Tue, 28 Sep 2021 16:16:28 GMT
EXPOSE 80
# Tue, 28 Sep 2021 16:16:28 GMT
CMD ["apache2-foreground"]
# Wed, 29 Sep 2021 13:20:17 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 13:20:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Oct 2021 21:37:36 GMT
COPY file:ef9ddfde9c1b01ce4b269763b45bce1abf8c9d7539baca060c7e89490e1e7845 in /usr/local/bin/ 
# Tue, 05 Oct 2021 21:37:36 GMT
ENV DRUPAL_VERSION=9.2.6
# Tue, 05 Oct 2021 21:37:36 GMT
WORKDIR /opt/drupal
# Tue, 05 Oct 2021 21:37:45 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Oct 2021 21:37:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815fd546abc9ddfff4d51c04a1a23dd4dfaeb7cc97bd3bfd2ff16c29efa926dc`  
		Last Modified: Tue, 28 Sep 2021 17:16:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860ed1b5b2bd43b112c3f76d417cbc0a8e56856076eeed83e30453f0ca5cb2d`  
		Last Modified: Tue, 28 Sep 2021 17:16:37 GMT  
		Size: 76.7 MB (76681149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7cb65357dc94c36bd249a314d8a60031a13dca9ab7a33bad789de68e0fe910`  
		Last Modified: Tue, 28 Sep 2021 17:16:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e96b690475613ed7c93756fbc819bf22bdf7857c88b026ee2d8e2f59a0ae2cd`  
		Last Modified: Tue, 28 Sep 2021 17:17:00 GMT  
		Size: 18.7 MB (18679434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf75eff774a1e52453c7a41a9c3396d3173ee00fdd634573825be74d02689d44`  
		Last Modified: Tue, 28 Sep 2021 17:16:55 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5599b8044782dc8e659d8c0efae4245b51caf5c41c45f6803df215eebc63928f`  
		Last Modified: Tue, 28 Sep 2021 17:16:55 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93eeab7ff5e639ca41e27eaf2cc7abf0365f9718f6136f0dcb81f14b41b2563`  
		Last Modified: Tue, 28 Sep 2021 17:24:44 GMT  
		Size: 10.7 MB (10709958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1a75d546230237819e74c4ad8e4ffbdb00f76afc48813f09eaed5db53f3405`  
		Last Modified: Tue, 28 Sep 2021 17:24:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbf0a0173287c8762e26e75273a8d0025a48885df607f6a2191399dbf2822ee`  
		Last Modified: Tue, 28 Sep 2021 17:24:44 GMT  
		Size: 14.3 MB (14345466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9f370b18b516d5b3eca08a96ee6e13bc9754ea59fe772ae886bce5750743a0`  
		Last Modified: Tue, 28 Sep 2021 17:24:41 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b4f05ea31f121129bacd0258f687cc6e8a4693aa32eac21b37909cfa4b3e2e`  
		Last Modified: Tue, 28 Sep 2021 17:24:41 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad64a5fca50b03f432de0dd07a178037cfdd1003734bd1dd301ecb92be22b0a9`  
		Last Modified: Tue, 28 Sep 2021 17:24:41 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d140c5f7038c9528895223b5574b8b5b93c0f24b4cc4b488a52aca0d9c3dfe`  
		Last Modified: Wed, 29 Sep 2021 13:30:27 GMT  
		Size: 1.7 MB (1702184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb813f10e2950569afd8a7e2e1c958f3e00f1c5372e259ff4e4f593735a24ef`  
		Last Modified: Wed, 29 Sep 2021 13:30:26 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cba4c3c16288a34da6c575bd134c38b3d165167a740035af6f397f9ea52a173`  
		Last Modified: Tue, 05 Oct 2021 21:49:30 GMT  
		Size: 557.0 KB (556998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b70f22aa92339fc1bad0e576dcc00e8e3afb80bb34adbf29b426d6be213fdf`  
		Last Modified: Tue, 05 Oct 2021 21:49:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcf5d742f3c093607e0056ac34c65bf311f521c387be38df43336abbcd566e3`  
		Last Modified: Tue, 05 Oct 2021 21:49:37 GMT  
		Size: 19.2 MB (19179288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:633b35110543ae5404524698ca8fa55b2da002d9e3349d4a489b4821335d29f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.4 MB (144417919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866a690ad7e777dc934dd17c1a18856ca727fd46d8624e562def65b911512557`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 30 Sep 2021 18:04:11 GMT
ADD file:e71f315aa894d483f75b32109fff32974c43ce2e684cd28eb6492bc6fc450931 in / 
# Thu, 30 Sep 2021 18:04:12 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 07:32:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 01 Oct 2021 07:32:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 01 Oct 2021 07:33:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 07:33:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 01 Oct 2021 07:33:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 01 Oct 2021 07:38:59 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 01 Oct 2021 07:39:00 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 01 Oct 2021 07:39:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 01 Oct 2021 07:39:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 01 Oct 2021 07:39:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 01 Oct 2021 07:39:25 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 01 Oct 2021 07:39:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 01 Oct 2021 07:39:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Oct 2021 07:39:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Oct 2021 07:39:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 01 Oct 2021 09:22:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 01 Oct 2021 09:22:47 GMT
ENV PHP_VERSION=7.4.24
# Fri, 01 Oct 2021 09:22:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Fri, 01 Oct 2021 09:22:48 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Fri, 01 Oct 2021 09:23:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 01 Oct 2021 09:23:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:27:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Oct 2021 09:27:23 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:27:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Oct 2021 09:27:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Oct 2021 09:27:26 GMT
STOPSIGNAL SIGWINCH
# Fri, 01 Oct 2021 09:27:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 01 Oct 2021 09:27:27 GMT
WORKDIR /var/www/html
# Fri, 01 Oct 2021 09:27:28 GMT
EXPOSE 80
# Fri, 01 Oct 2021 09:27:28 GMT
CMD ["apache2-foreground"]
# Sat, 02 Oct 2021 16:20:46 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 16:20:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Oct 2021 21:51:15 GMT
COPY file:ef9ddfde9c1b01ce4b269763b45bce1abf8c9d7539baca060c7e89490e1e7845 in /usr/local/bin/ 
# Tue, 05 Oct 2021 21:51:15 GMT
ENV DRUPAL_VERSION=9.2.6
# Tue, 05 Oct 2021 21:51:16 GMT
WORKDIR /opt/drupal
# Tue, 05 Oct 2021 21:51:43 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Oct 2021 21:51:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:421f17c521234da0c5b07d4f6e44314149dc3790ef12134e85e61741452c9f96`  
		Last Modified: Thu, 30 Sep 2021 18:20:50 GMT  
		Size: 22.7 MB (22746246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5641096c59071429c7049e0a56b96248a9c5b5a0602ce5a6ba2759e4aa2c6834`  
		Last Modified: Fri, 01 Oct 2021 10:45:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34d253e914adbe6836b8bb6d270843021c149273390997f6f27515250a1ffe`  
		Last Modified: Fri, 01 Oct 2021 10:46:36 GMT  
		Size: 59.5 MB (59515650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8c9a413d0316c765600e4964f6ac594e9f6b6e07bb8aa09e8ee94c3bd04ea0`  
		Last Modified: Fri, 01 Oct 2021 10:45:59 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb467ed6328728133eeae61870752cbf3be5d7b042b3cac583aba97eb23a689`  
		Last Modified: Fri, 01 Oct 2021 10:47:07 GMT  
		Size: 17.5 MB (17481676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02abeb58de9eb0d474d6148dee801ec0d3c620c16ce905534ef8ccb716358761`  
		Last Modified: Fri, 01 Oct 2021 10:46:58 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acb6064e5301ebfea3fbcd5dd72971bd66bf831524c3827fd22a587f4aa94b9`  
		Last Modified: Fri, 01 Oct 2021 10:46:57 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9062bd10fb671829bc37c8cebc9950931facd1c7fae53f90c765254c86a3894`  
		Last Modified: Fri, 01 Oct 2021 11:02:04 GMT  
		Size: 10.7 MB (10708154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6f9b47ef89bf14ba071c1c935a23f71e328b76854bf093856f7b2ab1abe253`  
		Last Modified: Fri, 01 Oct 2021 11:01:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e51d3079fb15cbbd9a8d75f54a8dc23710f67b7bd3e294d20f940686f94f269`  
		Last Modified: Fri, 01 Oct 2021 11:02:08 GMT  
		Size: 12.7 MB (12748956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4eac40430fa1d50aacd062470e1083237098bff6a56ea8356e60f26a7f03572`  
		Last Modified: Fri, 01 Oct 2021 11:01:59 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42c0be37892c52568f0e5410886faf87304d920a83ea2042648553f60354ccc`  
		Last Modified: Fri, 01 Oct 2021 11:01:59 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba216c33f72c8b21ddfc773ab0413323c602d7086f8a3b5692f3c577fc3731d`  
		Last Modified: Fri, 01 Oct 2021 11:01:59 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cc2abc5a5dbf8e700c81260066e8100872b191f4149535b72f4af03617efac`  
		Last Modified: Sat, 02 Oct 2021 16:51:54 GMT  
		Size: 1.5 MB (1474146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf40e62bb1103d0e5c6d3943848c71b55f14ff3e7e9bba5cd51b00131ca865d`  
		Last Modified: Sat, 02 Oct 2021 16:51:53 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17eb0fda43aeb983666e936e310fe0152e8a9f134e83dce745b88f8dddf2920`  
		Last Modified: Tue, 05 Oct 2021 22:31:24 GMT  
		Size: 557.0 KB (557008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ee233817df4d493471f39698dc70337733e949059980374fe0d9ab4da0941`  
		Last Modified: Tue, 05 Oct 2021 22:31:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b55fbd529f469767cb2996e552450926b929c1a54e6e53d515f42c1dc0c308`  
		Last Modified: Tue, 05 Oct 2021 22:31:50 GMT  
		Size: 19.2 MB (19180195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:0370c2e7f678fbb239ee5e85eb0324fd9bdad4544c1fe632cc991167c4f1b184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (161049934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7424242ab9fa164496700af1631f02d92a0dd3c6daed8f0c0ced5585c6f544d2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:03:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 09:03:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 09:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:03:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 09:03:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 09:09:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 28 Sep 2021 09:09:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 28 Sep 2021 09:09:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 28 Sep 2021 09:09:12 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 28 Sep 2021 09:09:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 28 Sep 2021 09:09:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 28 Sep 2021 09:09:13 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 28 Sep 2021 09:09:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 09:09:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 09:09:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 10:14:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 10:14:57 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 10:14:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 10:14:58 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 10:15:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 10:15:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:17:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 10:17:39 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:17:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 10:17:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 10:17:40 GMT
STOPSIGNAL SIGWINCH
# Tue, 28 Sep 2021 10:17:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 28 Sep 2021 10:17:40 GMT
WORKDIR /var/www/html
# Tue, 28 Sep 2021 10:17:40 GMT
EXPOSE 80
# Tue, 28 Sep 2021 10:17:40 GMT
CMD ["apache2-foreground"]
# Wed, 29 Sep 2021 06:08:00 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 06:08:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Oct 2021 20:58:58 GMT
COPY file:ef9ddfde9c1b01ce4b269763b45bce1abf8c9d7539baca060c7e89490e1e7845 in /usr/local/bin/ 
# Tue, 05 Oct 2021 20:58:58 GMT
ENV DRUPAL_VERSION=9.2.6
# Tue, 05 Oct 2021 20:58:58 GMT
WORKDIR /opt/drupal
# Tue, 05 Oct 2021 20:59:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Oct 2021 20:59:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b35a86ab1457a11a2b4250ccd7fc7d2055bca36ae4977bb4ca142a6ccc282a9`  
		Last Modified: Tue, 28 Sep 2021 11:05:50 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58411526b4c384b02c019d7de41d51086a2bcc8a27082f904e905478b1ae523`  
		Last Modified: Tue, 28 Sep 2021 11:06:01 GMT  
		Size: 70.4 MB (70356720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4637358d71d7946b8a93b46f810bf3a92817cce3132b12e12de9cd3e0b9d7b0`  
		Last Modified: Tue, 28 Sep 2021 11:05:50 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81add154ae07b25be8d1bd3b9f5ba0278370bee84e4f9e51387927527a6a0124`  
		Last Modified: Tue, 28 Sep 2021 11:06:26 GMT  
		Size: 18.6 MB (18580201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313a1aa35ccd32b5bd0ea7ac88fc8a5e9d0b3ff5e0413c30aa5c1802c3c1f06`  
		Last Modified: Tue, 28 Sep 2021 11:06:23 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2ddf244fc185a22cfe2fa737fe1412694dae1bfa44ff646970d873d274cff9`  
		Last Modified: Tue, 28 Sep 2021 11:06:22 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0269f878d0bed9ec921d3324d6dc5c0d52bc6c52f30464b58fe546f34d600bb1`  
		Last Modified: Tue, 28 Sep 2021 11:15:41 GMT  
		Size: 10.7 MB (10708744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4eb0d8b54ce1a01bf3900116c69052a8cdf356ad59503e39003ee1a6014bd6`  
		Last Modified: Tue, 28 Sep 2021 11:15:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05841ffbff68b4cd1df3f457ecefba43ce765c8601f516a5d60d86c219fa5a0`  
		Last Modified: Tue, 28 Sep 2021 11:15:41 GMT  
		Size: 14.1 MB (14054167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a69fd39bd41aa90a529827378a0c7ae8aea5ea98f5fc3695bcb5e73db3cabfe`  
		Last Modified: Tue, 28 Sep 2021 11:15:38 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c13d7c3d7f1cf13f44f2c691de390838da93d32ed230af647d1d8bd5628911`  
		Last Modified: Tue, 28 Sep 2021 11:15:38 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ed4ea780319eb53369e2aca33935004fd09374eb5e601883c5e72f96ea54e3`  
		Last Modified: Tue, 28 Sep 2021 11:15:38 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c8e4700f6abf7e3b44f14ca26e697d8e1200fe3c4d2e74fd27db20902b982d`  
		Last Modified: Wed, 29 Sep 2021 06:24:42 GMT  
		Size: 1.7 MB (1692215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02dd6645e81836507dd83a5b0576c51ad35baa0b10eb22fde40df0c5e5e63ec`  
		Last Modified: Wed, 29 Sep 2021 06:24:42 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31cb0ddaf9015906354c2fafa3d56e22556cf210000db523e3ee55245481f8c0`  
		Last Modified: Tue, 05 Oct 2021 21:18:31 GMT  
		Size: 557.0 KB (557002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79533c933e660250f1cb1c896702c7fe5ec31d10aad97ba8c96f87e9d604be`  
		Last Modified: Tue, 05 Oct 2021 21:18:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8f5256ff52e59e034dbdc4598042c254c178b093b58d019a915ffb1f7e5f`  
		Last Modified: Tue, 05 Oct 2021 21:18:42 GMT  
		Size: 19.2 MB (19179990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:6bec09b638e3d638c1393cf3f7cf62ae76f59ead136151abc0d7943a811e890b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175131229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6082116d99de3a4e3a4d60c2c110ea6c3c3b494768aef4ab151ef5029f26299a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:49 GMT
ADD file:c090abbb3afcfebf797e06e2ac4b778acb4e97d5dca79c29d1927f43cf14b23e in / 
# Tue, 28 Sep 2021 01:40:49 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 13:19:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 13:19:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 13:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 13:20:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 13:20:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 13:29:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 28 Sep 2021 13:29:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 28 Sep 2021 13:29:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 28 Sep 2021 13:29:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 28 Sep 2021 13:29:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 28 Sep 2021 13:29:19 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 28 Sep 2021 13:29:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 28 Sep 2021 13:29:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 13:29:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 13:29:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 15:27:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 15:27:03 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 15:27:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 15:27:04 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 15:27:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 15:27:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:31:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 15:31:41 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:31:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 15:31:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 15:31:43 GMT
STOPSIGNAL SIGWINCH
# Tue, 28 Sep 2021 15:31:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:31:44 GMT
WORKDIR /var/www/html
# Tue, 28 Sep 2021 15:31:45 GMT
EXPOSE 80
# Tue, 28 Sep 2021 15:31:45 GMT
CMD ["apache2-foreground"]
# Wed, 29 Sep 2021 03:24:13 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 03:24:15 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 29 Sep 2021 03:24:15 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Wed, 06 Oct 2021 18:50:24 GMT
ENV DRUPAL_VERSION=9.2.7
# Wed, 06 Oct 2021 18:50:24 GMT
WORKDIR /opt/drupal
# Wed, 06 Oct 2021 18:50:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 06 Oct 2021 18:50:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:82f7c8b98609aee82696182c03cb09ae62ceab1b17f8eec1e233a68180876d41`  
		Last Modified: Tue, 28 Sep 2021 01:50:06 GMT  
		Size: 27.8 MB (27797629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede349f021642655631250b04dbc18b6b8ecca6cf158e90bdbb94e31cabf201`  
		Last Modified: Tue, 28 Sep 2021 16:55:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78136b891d9a1d22d9233d2f5448cb1557a37e0bf8d062a9f9b61f68141939f2`  
		Last Modified: Tue, 28 Sep 2021 16:56:18 GMT  
		Size: 81.2 MB (81229337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eede2d4a61188f319e769095f2738a68eafdb2300f4a88fb0cf6becf68c22021`  
		Last Modified: Tue, 28 Sep 2021 16:55:56 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa5e8df4b3a82b0e9de7fc6db1e8849f49d81bc73079c674d563e7918d95982`  
		Last Modified: Tue, 28 Sep 2021 16:56:50 GMT  
		Size: 19.1 MB (19114923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe659eadcb5d4ade4693bd05be3e3e06bfc565fa01f0df339c6fdf2a6b05d23`  
		Last Modified: Tue, 28 Sep 2021 16:56:42 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496e626eb7d14f50453f86364afaacc7e0910a24a6622dc11a25d070f3af80d5`  
		Last Modified: Tue, 28 Sep 2021 16:56:42 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaf32979984ad15d1bb2be3bbbbcbfc61b7ad9ce780f183a402ac3cc2159c7b`  
		Last Modified: Tue, 28 Sep 2021 17:08:53 GMT  
		Size: 10.7 MB (10709291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7809334216e9eff398b4fa46dec2d2e46a8e0f6e55c3e869198263165814311e`  
		Last Modified: Tue, 28 Sep 2021 17:08:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29fec0ba91585e08fd20d5dff69092d6ed0463bb457b821e0ec2ed94f0f2c4a`  
		Last Modified: Tue, 28 Sep 2021 17:08:55 GMT  
		Size: 14.8 MB (14751779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d211e97cb59a5fe154a3718f2066750389c53743375b1b11d4106175b794fd4c`  
		Last Modified: Tue, 28 Sep 2021 17:08:50 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b00b348d04ce78fb0a85d385971222a2d752c1a379ca988aa3391ebd54dec`  
		Last Modified: Tue, 28 Sep 2021 17:08:50 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45c9c897aaf88fd558d59cccb034225509efa4d7a2b1df38a48f413f03291fe`  
		Last Modified: Tue, 28 Sep 2021 17:08:50 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a61f2aaeb6c29ad1a1b26b708e3e64bef25828c341fd52e6babe703adebf4a`  
		Last Modified: Wed, 29 Sep 2021 03:49:09 GMT  
		Size: 1.8 MB (1786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c2015c562cbb5dbcbc58705f26eb506260d4861d58437d8498236077896e4d`  
		Last Modified: Wed, 29 Sep 2021 03:49:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae03aa7b22c3ff96d34667b923c4c62f01c96447e1a01787d2f2a4ac07c84475`  
		Last Modified: Wed, 29 Sep 2021 03:49:08 GMT  
		Size: 553.2 KB (553184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67db85c9c0aedd906872019ae9c687f1df3e22e711592533eb25d12287b6e9c8`  
		Last Modified: Wed, 06 Oct 2021 19:06:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f610b36e929a01d8fe3f304d04515f96a3c3b281a2c53acaefb8ceedf2d001dd`  
		Last Modified: Wed, 06 Oct 2021 19:07:02 GMT  
		Size: 19.2 MB (19182737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:fad2b3d912ed7158915e2c5b3c241ba77880d21991678208252320aa8aff7de8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.4 MB (180370985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5fa96c57457c0249d0efc7c5b17a12b1cca3ecff4500d9e711ee5e894318e9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 02:27:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 05 Oct 2021 02:27:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 05 Oct 2021 02:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 02:32:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Oct 2021 02:33:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Oct 2021 02:42:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 05 Oct 2021 02:42:59 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 05 Oct 2021 02:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 05 Oct 2021 02:44:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 05 Oct 2021 02:44:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 05 Oct 2021 02:45:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 05 Oct 2021 02:45:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 05 Oct 2021 02:45:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 02:45:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 02:45:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Oct 2021 05:49:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Oct 2021 05:49:27 GMT
ENV PHP_VERSION=7.4.24
# Tue, 05 Oct 2021 05:49:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 05 Oct 2021 05:49:35 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 05 Oct 2021 05:50:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 05:50:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Oct 2021 05:58:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Oct 2021 05:58:58 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 05 Oct 2021 05:59:09 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Oct 2021 05:59:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Oct 2021 05:59:23 GMT
STOPSIGNAL SIGWINCH
# Tue, 05 Oct 2021 05:59:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 05 Oct 2021 05:59:27 GMT
WORKDIR /var/www/html
# Tue, 05 Oct 2021 05:59:30 GMT
EXPOSE 80
# Tue, 05 Oct 2021 05:59:35 GMT
CMD ["apache2-foreground"]
# Wed, 06 Oct 2021 10:42:07 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 10:42:11 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 06 Oct 2021 10:42:12 GMT
COPY file:ef9ddfde9c1b01ce4b269763b45bce1abf8c9d7539baca060c7e89490e1e7845 in /usr/local/bin/ 
# Wed, 06 Oct 2021 10:42:14 GMT
ENV DRUPAL_VERSION=9.2.6
# Wed, 06 Oct 2021 10:42:15 GMT
WORKDIR /opt/drupal
# Wed, 06 Oct 2021 10:42:35 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 06 Oct 2021 10:42:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5bb0e399334e40c90da8aea82dee066d6b56d1d6141ea84ff56062903ac086`  
		Last Modified: Tue, 05 Oct 2021 07:37:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0076a8ad1cfe3f9dd6fc7c53ff5948a137e948063b5c59aeb48186024acc8eff`  
		Last Modified: Tue, 05 Oct 2021 07:37:18 GMT  
		Size: 82.3 MB (82292002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93b47eab4c8230fa6b2d3c4ef1f6b3575b09e3264c579d088c920a88e6f12e`  
		Last Modified: Tue, 05 Oct 2021 07:37:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff3a832b964bed19afda367e89f790dedaa475ebe65880b62c73742cf5e53e`  
		Last Modified: Tue, 05 Oct 2021 07:37:42 GMT  
		Size: 19.8 MB (19818466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5349a69f942f33f8f20b56207ff685eff82ba9aac9ae5d477d61cf319cc1984a`  
		Last Modified: Tue, 05 Oct 2021 07:37:39 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1e651f6d401535a48484766984a6d9169572c85f4bae58639b0e345285d6e5`  
		Last Modified: Tue, 05 Oct 2021 07:37:38 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99497239007697f6ccd2624c46dbc6dbf8d017dff6efe3a2f037ae0e78f904c`  
		Last Modified: Tue, 05 Oct 2021 07:48:05 GMT  
		Size: 10.7 MB (10709937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbea9e2bbdf2bb6b4018f79cea31f294dbc5ee7466e62a8509c514fb9dde733`  
		Last Modified: Tue, 05 Oct 2021 07:48:01 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c5aa5b17014f64e25b1a37a3179aed35fe611ae83d8a0138844e3d67644abb`  
		Last Modified: Tue, 05 Oct 2021 07:48:04 GMT  
		Size: 15.3 MB (15313303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce038eaedb349dc7c6cb257d8f991bfc47324d771c6c3c45292942c16763a69c`  
		Last Modified: Tue, 05 Oct 2021 07:48:01 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29922c0ea6fc522a56aea1ce5859dfddd8b4256cff5b95891a0807dd628cccdb`  
		Last Modified: Tue, 05 Oct 2021 07:48:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa658987dac31614ef8169a41b89eb53db6483b58f0b88d3bece7ac913d04aa3`  
		Last Modified: Tue, 05 Oct 2021 07:48:01 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5b703ae7a77941dfb429ee5eb0c639d88d1b0965cbaf2613dd231fc6c9e85`  
		Last Modified: Wed, 06 Oct 2021 11:16:26 GMT  
		Size: 1.9 MB (1940280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cf927284f1084f6011f3b9aac70e7d3f15c1e6501eb1d3a7ef198cd1e87ede`  
		Last Modified: Wed, 06 Oct 2021 11:16:25 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55b94804f143b7ac3ecc8f904946ac12fb3522211aabf527a40146c073f54f7`  
		Last Modified: Wed, 06 Oct 2021 11:16:25 GMT  
		Size: 557.0 KB (557004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aefe17e948bb24342c48c152b4f21e652ad3df654d7bdc302a76daa689e8c9`  
		Last Modified: Wed, 06 Oct 2021 11:16:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d112843873af89571e9f341009f13b69a94ba3cdb44b1e4849ce4c02c3667d3`  
		Last Modified: Wed, 06 Oct 2021 11:18:35 GMT  
		Size: 19.2 MB (19180379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:fe4f47bbeb02f0a5baa36359cba660e8f21bb6ff0eb22a3d21ddc0a4c7da1ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154653068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dea8e5ec76831b628ad4fd8736a9337ce1c03cff492ddd889de18f5df0dc7e8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:54:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 28 Sep 2021 05:54:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 28 Sep 2021 05:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:54:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Sep 2021 05:54:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 28 Sep 2021 05:57:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 28 Sep 2021 05:57:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 28 Sep 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 28 Sep 2021 05:57:12 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 28 Sep 2021 05:57:13 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 28 Sep 2021 05:57:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 28 Sep 2021 05:57:13 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 28 Sep 2021 05:57:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 05:57:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Sep 2021 05:57:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Sep 2021 06:37:11 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 28 Sep 2021 06:37:11 GMT
ENV PHP_VERSION=7.4.24
# Tue, 28 Sep 2021 06:37:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Tue, 28 Sep 2021 06:37:12 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Tue, 28 Sep 2021 06:37:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Sep 2021 06:37:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:38:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Sep 2021 06:38:45 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:38:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Sep 2021 06:38:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Sep 2021 06:38:46 GMT
STOPSIGNAL SIGWINCH
# Tue, 28 Sep 2021 06:38:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 28 Sep 2021 06:38:46 GMT
WORKDIR /var/www/html
# Tue, 28 Sep 2021 06:38:46 GMT
EXPOSE 80
# Tue, 28 Sep 2021 06:38:46 GMT
CMD ["apache2-foreground"]
# Tue, 28 Sep 2021 14:51:25 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 14:51:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Oct 2021 21:00:25 GMT
COPY file:ef9ddfde9c1b01ce4b269763b45bce1abf8c9d7539baca060c7e89490e1e7845 in /usr/local/bin/ 
# Wed, 06 Oct 2021 18:46:09 GMT
ENV DRUPAL_VERSION=9.2.7
# Wed, 06 Oct 2021 18:46:10 GMT
WORKDIR /opt/drupal
# Wed, 06 Oct 2021 18:46:43 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 06 Oct 2021 18:46:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b76cd23951c492c8e2173a040e37c99137663c238bb4676be1b20cd0aa79a23`  
		Last Modified: Tue, 28 Sep 2021 07:13:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ecfc599bf380f4f380b456fd0f21d532486d8c06bcca669ff770fabbed286`  
		Last Modified: Tue, 28 Sep 2021 07:14:05 GMT  
		Size: 64.7 MB (64711834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa51e922d4723fd053e815145ccb1fdb121a98e1e7023f9d0f45afdcc1a800e`  
		Last Modified: Tue, 28 Sep 2021 07:13:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3bd562733611aea3c2e26b3ee5abb6885ee31c55e8813b9ee3f03d35c5b169`  
		Last Modified: Tue, 28 Sep 2021 07:14:20 GMT  
		Size: 18.5 MB (18524684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4c9630f2733f9a15625fba03109b5bdff57819f9b6310b9860b6f40ec35f27`  
		Last Modified: Tue, 28 Sep 2021 07:14:17 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7cfc52206c3999e99c32a18bafcb85128359c74dc590d8f4c7fe4555720f6a`  
		Last Modified: Tue, 28 Sep 2021 07:14:17 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4949ad8b3345394491b0482de6faaf10770907a7805b5bdf84cbc1f8471aec9`  
		Last Modified: Tue, 28 Sep 2021 07:20:10 GMT  
		Size: 10.7 MB (10708509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa29c772828728c527f1a47c02b58a7a512aee0a9e95a03a5ddc19c41719cb0`  
		Last Modified: Tue, 28 Sep 2021 07:20:08 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a639be5058e88c55e757b10d046c596491eb661ed9af447cd2372e650e70920e`  
		Last Modified: Tue, 28 Sep 2021 07:20:10 GMT  
		Size: 13.5 MB (13514741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd4a7512764133a035f79f436d28ca48e5b1e1ac276cc29e5ab38db46c8b43a`  
		Last Modified: Tue, 28 Sep 2021 07:20:08 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505196a9bd8b3cd72b293dd031478b9b635de1b8ea113e4aea3981ed4374a995`  
		Last Modified: Tue, 28 Sep 2021 07:20:08 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7e08a8c79f92cd4b8858567a735897d2b53bb0e4f4c398ea5eb6e853d1f845`  
		Last Modified: Tue, 28 Sep 2021 07:20:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1932d2ba51f988baf9b2f0b84f1bf87864a7262f604967dfb8f34bdedf658a89`  
		Last Modified: Tue, 28 Sep 2021 15:05:36 GMT  
		Size: 1.7 MB (1686963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e878d1394a1973d18d60c993ba81a594444bcc532fc9113e3566a4965de88231`  
		Last Modified: Tue, 28 Sep 2021 15:05:36 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d65cb6efa8bee4f0e4a87dbeca5d2e1c3eff6f63e71012ea0881404a3b305`  
		Last Modified: Tue, 05 Oct 2021 21:16:41 GMT  
		Size: 557.0 KB (557003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86400735d984c338cc50183c236922b56deda52ed849778b096aaaafe60fb980`  
		Last Modified: Wed, 06 Oct 2021 19:03:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff64012d42f5392d2f3a84d288ec3a96cb3a8982069a5a6442e86778eb85f5`  
		Last Modified: Wed, 06 Oct 2021 19:03:21 GMT  
		Size: 19.2 MB (19182609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
