## `drupal:rc-php8.1-apache-buster`

```console
$ docker pull drupal@sha256:be8922569f54637ed1bafcdd078753e95956cf93373b8cd47c371617c11efd58
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
$ docker pull drupal@sha256:553e8a76a27e65a60ef07d636ff77a747752f676738402a3189ac1179c318d82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167399901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1decf58d7f0f08ab897baf0a5993db2ff1b32dd244fc02ebe65591749e96104b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:43:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 12:43:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 12:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:44:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 12:44:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 12:47:29 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 12:47:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 12:47:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 12:47:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 12:47:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 12:47:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 12:47:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 12:47:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 12:47:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 13 May 2022 22:36:31 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 22:36:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 22:36:31 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 22:36:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 22:36:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 22:39:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 22:39:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 22:39:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 22:39:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 22:39:46 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 22:39:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 22:39:46 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 22:39:46 GMT
EXPOSE 80
# Fri, 13 May 2022 22:39:46 GMT
CMD ["apache2-foreground"]
# Sat, 14 May 2022 00:21:15 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 May 2022 00:21:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 00:21:16 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 14 May 2022 00:21:16 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 14 May 2022 00:21:16 GMT
WORKDIR /opt/drupal
# Sat, 14 May 2022 00:21:25 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 14 May 2022 00:21:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f244825368f69cd0cfb49ee42a4574bace42e16ac2c9b2515a060b3dfe388d37`  
		Last Modified: Wed, 11 May 2022 14:41:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb682e3d268ef81e7e393af85a67246e65aaec51212990db89e5c5ae6577903`  
		Last Modified: Wed, 11 May 2022 14:41:13 GMT  
		Size: 76.7 MB (76683095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea16ce02660cac335bec012c37c79819d15be720c06a8a90493087b0adf2af5`  
		Last Modified: Wed, 11 May 2022 14:41:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5b7334d3648574cfeb7dbc68f99f1617c1caa7cd79d2e4424d06de8ab04536`  
		Last Modified: Wed, 11 May 2022 14:41:34 GMT  
		Size: 18.7 MB (18681908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbba56d4063a24484d45167b6176688a1e48a5f84b6b7388c5bc4c38c43c2a1`  
		Last Modified: Wed, 11 May 2022 14:41:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3822be6520ec3ffee2785df51bc81caac54142ce3ce21a67ed807d4576abe552`  
		Last Modified: Wed, 11 May 2022 14:41:31 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202afc1f398642c9efa8c4c1dc7bc3602a2bc426a98993e57fc680d41c2674eb`  
		Last Modified: Fri, 13 May 2022 23:17:17 GMT  
		Size: 12.0 MB (12047053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399f3ca5ee12433cb95cac9d438a7393020c4c104c22fc51a57649d86535a48e`  
		Last Modified: Fri, 13 May 2022 23:17:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a567cf8f27cb9caceb415b7eea25763b712200b6f11fefd635cf1d95d2f28e2`  
		Last Modified: Fri, 13 May 2022 23:17:16 GMT  
		Size: 11.0 MB (10981845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d2f1891e4b1e704bb17c50347d0838c8141d0a06c0b90168f2e2e6561fc295`  
		Last Modified: Fri, 13 May 2022 23:17:14 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f32a6c18a24d240c324652de6ed36b9d1233124baa4b9f2b62a16488961ba`  
		Last Modified: Fri, 13 May 2022 23:17:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06abd4137939e5490acb6f0d544fa8678f7ad3fd6a241130a216f1754185490`  
		Last Modified: Fri, 13 May 2022 23:17:14 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e5886fe9474e0e603b81a6c48a3bdd052cc7b725d1e041f17377458b666fb5`  
		Last Modified: Sat, 14 May 2022 00:33:30 GMT  
		Size: 2.1 MB (2082340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968d95ecfdedd421f08a6147f0f2a108e142a8751f2170ff342d34fb0b4380eb`  
		Last Modified: Sat, 14 May 2022 00:33:30 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b807f542440cb03ee4fedc9d80b067cafd65c3120193397212e8bb988d6a0d57`  
		Last Modified: Sat, 14 May 2022 00:33:30 GMT  
		Size: 661.6 KB (661587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd03a571163971530752b9c8cd55b5f105e0c2ed9b3d5c8ff0e335967c25758`  
		Last Modified: Sat, 14 May 2022 00:33:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fab5818434c440c3300c79442c63c76393078e732c7c81ef2547d2f307620`  
		Last Modified: Sat, 14 May 2022 00:33:34 GMT  
		Size: 19.1 MB (19115299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:74c1d9e3313ea12ef3441aec578ac069315763b3b191aaad1fa8b283cfbefbff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142602589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:364bb58b9b1f96ea974425d92745484337ff5af429169e30d98b090598e17006`
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
# Wed, 11 May 2022 14:46:41 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 14:46:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 14:46:42 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 14:47:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 14:47:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 14:51:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 14:51:51 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 14:51:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 14:51:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 14:51:53 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 14:51:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 14:51:54 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 14:51:54 GMT
EXPOSE 80
# Wed, 11 May 2022 14:51:55 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 22:37:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 22:37:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 22:37:46 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Thu, 12 May 2022 22:37:46 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Thu, 12 May 2022 22:37:47 GMT
WORKDIR /opt/drupal
# Thu, 12 May 2022 22:38:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 12 May 2022 22:38:19 GMT
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
	-	`sha256:f2125fbef6c1ac8114533efc292351ef82d7ace5393a485ef95500292ee6e160`  
		Last Modified: Wed, 11 May 2022 17:38:09 GMT  
		Size: 12.1 MB (12089203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec53a5b947aefb5ab770f114d10d2393b11c4cbfca738ebc52f5114ad436008`  
		Last Modified: Wed, 11 May 2022 17:38:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d5361001c3f01ee974f7d1997495e50f4aa704c7695c61329aa6eab408dcb2`  
		Last Modified: Wed, 11 May 2022 17:38:11 GMT  
		Size: 9.5 MB (9481913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3dc423310f6d50c267dac0c9c75e79c4c475ce30c43df6063f0da77242fd8d6`  
		Last Modified: Wed, 11 May 2022 17:38:05 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f200a2bcc0649fc27878e652a419e1030155fdfa9998c2d78ef28c52d221a9a4`  
		Last Modified: Wed, 11 May 2022 17:38:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c2c10635870bd6e9dfa2d00521588cabd9374f44c9cefd61aeb9132ddded0e`  
		Last Modified: Wed, 11 May 2022 17:38:04 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503fb130a2a41daa9015188fd6539000ac2c0852573a852d7ca647222241da08`  
		Last Modified: Thu, 12 May 2022 23:45:14 GMT  
		Size: 1.5 MB (1479795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de10e47849870c240f045d71555f04090e9530e3ffe61e8bd2531ac4cdc8c66`  
		Last Modified: Thu, 12 May 2022 23:45:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7bc2a4ecd9a7f26dc810c71c3e26406a4ba8cd3454c775338266590644f924`  
		Last Modified: Thu, 12 May 2022 23:45:14 GMT  
		Size: 661.6 KB (661590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4165df0cb618b97348bcf65e5298d44c770b485c935833083c58646c28e2c929`  
		Last Modified: Thu, 12 May 2022 23:45:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9e8ec28f98290216f340220044a6dbe50501d0ad3ab6aa38b7f9b73271860a`  
		Last Modified: Thu, 12 May 2022 23:45:41 GMT  
		Size: 19.1 MB (19117500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:1c9b5d6c85978348ffb918908ab638ca0de0f68d8bdc8e99c50c99dfa6bfd061
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.5 MB (159450171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02bccb4a17176852d53f0cee3753554e4aca49837532b2e960430dd0b73ee579`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:26:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 05:26:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 05:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:27:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 05:27:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 05:31:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 05:31:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 05:31:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 05:31:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 05:31:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 05:31:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 05:31:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 05:31:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 05:31:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 13 May 2022 23:01:20 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 23:01:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 23:01:22 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 23:01:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 23:01:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 23:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 23:05:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 23:05:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 23:05:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 23:05:24 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 23:05:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 23:05:26 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 23:05:27 GMT
EXPOSE 80
# Fri, 13 May 2022 23:05:28 GMT
CMD ["apache2-foreground"]
# Sat, 14 May 2022 00:31:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 May 2022 00:31:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 00:31:11 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 14 May 2022 00:31:11 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 14 May 2022 00:31:12 GMT
WORKDIR /opt/drupal
# Sat, 14 May 2022 00:31:36 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 14 May 2022 00:31:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd6c01fc5ec55059b00e207fae5b859fd64fd15f05fa6f179fd6f704009eb72`  
		Last Modified: Wed, 11 May 2022 07:36:16 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da393b4f986c787bdf0377253a237ff08ee9739b128928e86442a70cf152a91`  
		Last Modified: Wed, 11 May 2022 07:36:26 GMT  
		Size: 70.4 MB (70363643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78671f24ef92877860da8aca9d56f5ed116741ecfee59cda214e2cb95360eb5`  
		Last Modified: Wed, 11 May 2022 07:36:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183254bc6a0cf2d41bd2c917d82e2a2ce89303061a7979940c72c903cf06af5`  
		Last Modified: Wed, 11 May 2022 07:36:49 GMT  
		Size: 18.4 MB (18367229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48752f3e4882bdc86651b70884249e593661430972904082a6605e923e6899a4`  
		Last Modified: Wed, 11 May 2022 07:36:46 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88bdb51d152471ade5a83217635d0e5e96594a27edbe1e3587004a85d042f8`  
		Last Modified: Wed, 11 May 2022 07:36:46 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250b7a5d8bdbf093957e3e958cf2d5e41374192b9d5d7bb8246df738f596b425`  
		Last Modified: Fri, 13 May 2022 23:59:40 GMT  
		Size: 11.8 MB (11832318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb67b92a792ec0c1033e62a6e2458b5abda209b0cb916e197772ca753a19f33`  
		Last Modified: Fri, 13 May 2022 23:59:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c47f1e3ac64c8b006230b2cc15b5a6ef627bef5cfab10fc63a2a525618bca95`  
		Last Modified: Fri, 13 May 2022 23:59:38 GMT  
		Size: 11.1 MB (11052404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ff5b454079a5d2eac72c08aa81441a16e8344a469631627fe12be98a164907`  
		Last Modified: Fri, 13 May 2022 23:59:36 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51962fa64d826b66ddac40ceda342359e924e69fc638ae4ba6bf8fbc1561c12`  
		Last Modified: Fri, 13 May 2022 23:59:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e54164a3e6d218432090afa368ace92eb02aa91b5ed6719496107ea81419fc`  
		Last Modified: Fri, 13 May 2022 23:59:36 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda6e63473970cf4f02e14decff2b4e816b5ab38114049557ff3fcd9ef330ff8`  
		Last Modified: Sat, 14 May 2022 00:54:39 GMT  
		Size: 2.1 MB (2139304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d417e9317e156cd167899df94c008cbb346b7e5ac01468efc785d55d86f76`  
		Last Modified: Sat, 14 May 2022 00:54:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfa448685192e91a0541a1e094d03a09c485ac1e2fb1836da36c3ed247ade41`  
		Last Modified: Sat, 14 May 2022 00:54:39 GMT  
		Size: 661.6 KB (661585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a12992546e89079e0de166bd3f806a35db420bc90afedfc04844c25169836c9`  
		Last Modified: Sat, 14 May 2022 00:54:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88daf3e8810e4906118f77bd79391ddbe3b57e51bd0c59d9b2ccfef91deb3d52`  
		Last Modified: Sat, 14 May 2022 00:54:44 GMT  
		Size: 19.1 MB (19118775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:71ebbaf1c0458050e5700c4ccfea2a9e87c0d6fdea8ab4836b2c5a2bdc0ac765
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172688006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a01bf27544c525d466dcaed6485f1973556dbc7ba393ec300eebdf91ec088aaa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:39:41 GMT
ADD file:fc7b00a8a5b0e703ac3ede5e2e51257f5ee709fcd35fee53e7b99d144cd873e4 in / 
# Wed, 11 May 2022 01:39:42 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:25:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 07:25:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 07:25:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:25:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 07:25:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 07:29:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 07:29:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 07:29:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 07:29:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 07:29:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 07:29:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 07:29:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 07:29:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 07:29:29 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 13 May 2022 22:54:57 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 22:54:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 22:54:58 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 22:55:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 22:55:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 22:57:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 22:57:53 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 22:57:53 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 22:57:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 22:57:55 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 22:57:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 22:57:57 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 22:57:58 GMT
EXPOSE 80
# Fri, 13 May 2022 22:57:59 GMT
CMD ["apache2-foreground"]
# Sat, 14 May 2022 00:08:47 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 May 2022 00:08:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 00:08:49 GMT
COPY file:95091188fdd3c74d6d01c7de0880a7368fde28cdcf2258fe6769e04bf78b518a in /usr/local/bin/ 
# Sat, 14 May 2022 00:08:49 GMT
ENV DRUPAL_VERSION=10.0.0-alpha4
# Sat, 14 May 2022 00:08:50 GMT
WORKDIR /opt/drupal
# Sat, 14 May 2022 00:09:04 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 14 May 2022 00:09:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b1c376c64b69c16b8b035dfd04b99bb7769a5afdfb56a1241aa4ec8743e85aa7`  
		Last Modified: Wed, 11 May 2022 01:47:22 GMT  
		Size: 27.8 MB (27799149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98173136b3e272988632d9fd1ca9c1f6bd6c1f7c166f61707607412f3113b2e`  
		Last Modified: Wed, 11 May 2022 09:26:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbaae31a7374a9f2d4288a8c381faf678da4f129691d4fa24a031d40bf7f43f`  
		Last Modified: Wed, 11 May 2022 09:26:14 GMT  
		Size: 81.2 MB (81227366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf1fb5abca72cb9047ecb7db95c628c36fff0f57103064288a53e8d13608d20`  
		Last Modified: Wed, 11 May 2022 09:26:02 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595f53c65b84b4aa43f1a462bde65fb83dde7d2f6abe06c7a104eb7cc59656de`  
		Last Modified: Wed, 11 May 2022 09:26:38 GMT  
		Size: 18.9 MB (18900628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bf5c95b7ebbc19469cae218df214e2922c16646217ec524a9f75720f5c9fd5`  
		Last Modified: Wed, 11 May 2022 09:26:34 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25edc2564b03493ed70f8671ac1716067e045b2ea56051f8cd2cc0cad6f555f5`  
		Last Modified: Wed, 11 May 2022 09:26:34 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ffafe0550d001e5ddd8668175e7aceed8f9ac5eb3616b3e81fa6ec2457806d`  
		Last Modified: Fri, 13 May 2022 23:39:53 GMT  
		Size: 11.8 MB (11832859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256078766b50c42398c9ddb73ada03564980e17857af91940fa0d3f75743d73`  
		Last Modified: Fri, 13 May 2022 23:39:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8393ad7a211fe4a8199abdc4f6029bac4237e0e09461eead4be898a828aa269b`  
		Last Modified: Fri, 13 May 2022 23:39:51 GMT  
		Size: 11.2 MB (11201018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333044e1f976cae72cc6d1a06c0905c561083289b1616c86df038c770e299644`  
		Last Modified: Fri, 13 May 2022 23:39:50 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aac9374c2260b89c702e691b3f098a12e490ce47ddf29e20c9499fadd691a15`  
		Last Modified: Fri, 13 May 2022 23:39:50 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52cecd1d0483ecd4c4bd96d0929cca3ed04fd00aef90fbdbe793b2aeea68912c`  
		Last Modified: Fri, 13 May 2022 23:39:50 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3a55d321c25438af8bbe8e15979fe5567977f491477fdd7f33523ed194906b`  
		Last Modified: Sat, 14 May 2022 00:29:42 GMT  
		Size: 1.9 MB (1940705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94edd0ce48566d795e4ad68a08e3b1ed06fa080fa9e045b6ac461cc18dda741e`  
		Last Modified: Sat, 14 May 2022 00:29:41 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276d8f26a4c42e6212cb0223c4e2025bf133b14124d36aaba945e5f94ee3bd79`  
		Last Modified: Sat, 14 May 2022 00:29:42 GMT  
		Size: 661.6 KB (661586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c76ddda093668b578b89759e814e6fe4f5a1e675d4f5b754203ac27a2e4b1e`  
		Last Modified: Sat, 14 May 2022 00:29:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bd8f2ad316b645589469b8d4008775dc60c22663282b75efb6db75acf878bd`  
		Last Modified: Sat, 14 May 2022 00:29:46 GMT  
		Size: 19.1 MB (19118814 bytes)  
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
