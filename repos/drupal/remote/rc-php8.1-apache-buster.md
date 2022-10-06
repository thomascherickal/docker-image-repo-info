## `drupal:rc-php8.1-apache-buster`

```console
$ docker pull drupal@sha256:52d1b37fdba7e5e42cff8d0c4a51e804dfbb077f62c6b831b2641f30328e4bed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:rc-php8.1-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:988e1ec0a41835c99d2c473a46646c6f90d6daba99cc2ce84eed97810c6a8190
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165994083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f321c788fc98c1c85772127e95258a536f42e20953e757b02cf4e164771f13`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:22:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 05 Oct 2022 07:22:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 05 Oct 2022 07:23:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:23:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 05 Oct 2022 07:23:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 05 Oct 2022 07:26:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 05 Oct 2022 07:26:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 05 Oct 2022 07:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 05 Oct 2022 07:26:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 05 Oct 2022 07:26:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 05 Oct 2022 07:26:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Oct 2022 07:26:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Oct 2022 07:26:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 05 Oct 2022 07:52:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 05 Oct 2022 07:52:54 GMT
ENV PHP_VERSION=8.1.11
# Wed, 05 Oct 2022 07:52:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.11.tar.xz.asc
# Wed, 05 Oct 2022 07:52:54 GMT
ENV PHP_SHA256=3005198d7303f87ab31bc30695de76e8ad62783f806b6ab9744da59fe41cc5bd
# Wed, 05 Oct 2022 07:53:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 05 Oct 2022 07:53:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 05 Oct 2022 07:56:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 05 Oct 2022 07:56:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 05 Oct 2022 07:56:05 GMT
RUN docker-php-ext-enable sodium
# Wed, 05 Oct 2022 07:56:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 05 Oct 2022 07:56:05 GMT
STOPSIGNAL SIGWINCH
# Wed, 05 Oct 2022 07:56:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 05 Oct 2022 07:56:05 GMT
WORKDIR /var/www/html
# Wed, 05 Oct 2022 07:56:05 GMT
EXPOSE 80
# Wed, 05 Oct 2022 07:56:05 GMT
CMD ["apache2-foreground"]
# Thu, 06 Oct 2022 00:04:55 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 00:04:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 06 Oct 2022 00:04:56 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 06 Oct 2022 00:04:56 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Thu, 06 Oct 2022 00:04:56 GMT
WORKDIR /opt/drupal
# Thu, 06 Oct 2022 00:05:08 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 06 Oct 2022 00:05:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caafd74e30285bd82a1099001fdf19d68f60215ba05e12c11340639dc0a73f93`  
		Last Modified: Wed, 05 Oct 2022 08:53:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45715cafb97372e282f0648031a4262cd5bc34a8ce99a69c52a7ecbd1b8c126`  
		Last Modified: Wed, 05 Oct 2022 08:53:41 GMT  
		Size: 76.7 MB (76685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5328863c71ccdb1520344da48f46073fd3675534ca660a0886215a3108b9477`  
		Last Modified: Wed, 05 Oct 2022 08:53:30 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d484c2d69b14085576b62d019b18a555de540b9c9d04b7834a15d504a61903d9`  
		Last Modified: Wed, 05 Oct 2022 08:54:01 GMT  
		Size: 18.7 MB (18682095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf8ffbd2f0e980468903416d66292244a20e06b9ca9d9320ee2ef9ac0fc6fdb`  
		Last Modified: Wed, 05 Oct 2022 08:53:59 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d8654c6608de8e61da9589091c125f2ec04e1b10d268904eaa118db8bfbf7e`  
		Last Modified: Wed, 05 Oct 2022 08:53:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dddb620b50d78ced37c70c6bfec4ff74de97c0870c951506eb47fb6ed4484bd`  
		Last Modified: Wed, 05 Oct 2022 08:57:35 GMT  
		Size: 12.1 MB (12135061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114bb287f8a8ea70829640ec2d389fd86487a1c7db447f18701d03fe765c0d52`  
		Last Modified: Wed, 05 Oct 2022 08:57:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0873d1da4495b474d15bd441a007860cd71fd0872362652370fe1397c13a4fe4`  
		Last Modified: Wed, 05 Oct 2022 08:57:34 GMT  
		Size: 11.0 MB (10995434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3174dddb817a0846831902c16a57dd681a3a49947cd915d15d297644f39a210`  
		Last Modified: Wed, 05 Oct 2022 08:57:32 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ce6331ce87a6a1c39934bd9de78f3860f61ed126f8b3c022f452e64ac98def`  
		Last Modified: Wed, 05 Oct 2022 08:57:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d587f4ee02f51f5c066d1b81a3024683618f5b7ee1befaab302eb9adfe96316`  
		Last Modified: Wed, 05 Oct 2022 08:57:33 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffbfe6fab1a885e9d2266d23e144a0cecc40b161488c1e0450842b8f28e4039`  
		Last Modified: Thu, 06 Oct 2022 00:28:15 GMT  
		Size: 2.1 MB (2084318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d421e02cd0896253e8da98aa946fa2c37dd462cb79133de53b4f4147a1864e`  
		Last Modified: Thu, 06 Oct 2022 00:28:15 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ceef81d6a263fffeafaa03a18b484bd21eff2a06594c5276f75c09a2396edb`  
		Last Modified: Thu, 06 Oct 2022 00:28:15 GMT  
		Size: 692.6 KB (692594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae3d8ecb0317c47f64b99731756388ee1e01f79463685b663f4b6298e83acd`  
		Last Modified: Thu, 06 Oct 2022 00:28:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da68b9c7c8f5a7867103568bb8519636500324023c42324788c1c80776734f9`  
		Last Modified: Thu, 06 Oct 2022 00:28:19 GMT  
		Size: 17.6 MB (17575476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:f26c2ba9f91aa5fad54a138e9fc2648231364d183f20f6d7c6c48cf72507197d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141849325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1427c3d24fb972928e9f5a083d67df8b36167c114c8e30e543a01a0d50d267`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 03:43:14 GMT
ADD file:0a80cba5196c5f463d85aeb456ee0f5778155ac5b1d3ce93a2023f1141aac44a in / 
# Tue, 13 Sep 2022 03:43:14 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 19:45:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 19:45:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 19:46:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 19:46:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 19:46:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 19:53:24 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 19:53:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 19:53:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 19:53:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 19:53:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 19:53:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 19:53:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 19:53:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 21:08:03 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 29 Sep 2022 18:41:35 GMT
ENV PHP_VERSION=8.1.11
# Thu, 29 Sep 2022 18:41:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.11.tar.xz.asc
# Thu, 29 Sep 2022 18:41:35 GMT
ENV PHP_SHA256=3005198d7303f87ab31bc30695de76e8ad62783f806b6ab9744da59fe41cc5bd
# Thu, 29 Sep 2022 18:41:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Sep 2022 18:41:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 18:46:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 18:46:41 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 29 Sep 2022 18:46:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 18:46:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 18:46:41 GMT
STOPSIGNAL SIGWINCH
# Thu, 29 Sep 2022 18:46:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 29 Sep 2022 18:46:42 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 18:46:42 GMT
EXPOSE 80
# Thu, 29 Sep 2022 18:46:42 GMT
CMD ["apache2-foreground"]
# Thu, 29 Sep 2022 21:43:21 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 29 Sep 2022 21:43:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 21:43:22 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 21:43:22 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Thu, 29 Sep 2022 21:43:22 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 21:43:53 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 21:43:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:04df89f99dde583959eeb3f2964381f6e5a3199fa335ea1b9862aab596638515`  
		Last Modified: Tue, 13 Sep 2022 03:50:50 GMT  
		Size: 22.7 MB (22740495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c0e8bbe2c6e458b7783701258d3eae9edde02832a121b7f447c3d3783e1047`  
		Last Modified: Wed, 14 Sep 2022 00:06:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7d9007b99f7194046023d68fc9fd86ca8a98585cece2f4e55c1c5df6ee045b`  
		Last Modified: Wed, 14 Sep 2022 00:07:16 GMT  
		Size: 59.5 MB (59539491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104f39f65cce60b96bbdccc1c0d54e5b0acbdc48b47602ae70f2b0ba7bdd04d5`  
		Last Modified: Wed, 14 Sep 2022 00:06:57 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb9839442dcdc4588e996e77db1b251098b61c700793a1bf3fa7fbc0e1ca28`  
		Last Modified: Wed, 14 Sep 2022 00:07:45 GMT  
		Size: 17.5 MB (17480824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97959223410099ea3108cde3c6c828c8471a79f233b50247dda00efeeafd6fe4`  
		Last Modified: Wed, 14 Sep 2022 00:07:40 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54a809c6ac9ee541387127cb7994be3bce6b7cd55a71589db81353d88eee66`  
		Last Modified: Wed, 14 Sep 2022 00:07:40 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f86dbac37b141e31673698d39a0825771ad3065d5b7d0f034b2a407a6b5584`  
		Last Modified: Thu, 29 Sep 2022 21:28:11 GMT  
		Size: 12.1 MB (12133144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c453814bf3ec12dfd2d4f9a173fdc331b52a8cb74a88b9d3a2ebedcdf7d74e`  
		Last Modified: Thu, 29 Sep 2022 21:28:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f315af616b114a5bae3496fb9af4cdfbdf51c052edae494757f85f35b6df102`  
		Last Modified: Thu, 29 Sep 2022 21:28:11 GMT  
		Size: 10.2 MB (10200878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d6b5f6c586d967a0b4a9512aa1e81d0adeb9da0a130d383d32bfaeffdce636`  
		Last Modified: Thu, 29 Sep 2022 21:28:07 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b14f3dc733ef646423b706ef5a7248ec44069187db282c694425794c3c2c98`  
		Last Modified: Thu, 29 Sep 2022 21:28:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11a293708bf9021efab8d0d5527aa9ea45534f1a011001addc999724f5cb9fc`  
		Last Modified: Thu, 29 Sep 2022 21:28:07 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e82e02904673346074d0b2bae15ee93986a5bfd84a694a978915ae4813fbceb`  
		Last Modified: Thu, 29 Sep 2022 22:32:55 GMT  
		Size: 1.5 MB (1480184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392deca9eba760af43ac724ccd14304043408c8f4c80ccbc4ce070cc85c00105`  
		Last Modified: Thu, 29 Sep 2022 22:32:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f13af0bd930fa7eb9e1a3dc14d4389fac690ba89201e13e78d493470e5d4579`  
		Last Modified: Thu, 29 Sep 2022 22:32:55 GMT  
		Size: 692.6 KB (692587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2f1c045887e72b12f3fc03ea1fa89ee340ff7285b07f8ca6fe462fdd736225`  
		Last Modified: Thu, 29 Sep 2022 22:32:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1505844ec0bfd05889ea731970882c15d199260690054f634772ce96a710a9b0`  
		Last Modified: Thu, 29 Sep 2022 22:33:06 GMT  
		Size: 17.6 MB (17575647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:a8e26b762679465b872962c20a8f6e23d18b9be7fa9af898a86dbebb26621eac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158056233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d756fc82bdcbb5538e213a5125aa6bbb62cf2828b449f35aca8501fbb3db12f4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:21:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 05 Oct 2022 07:21:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 05 Oct 2022 07:21:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:21:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 05 Oct 2022 07:21:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 05 Oct 2022 07:25:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 05 Oct 2022 07:25:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 05 Oct 2022 07:26:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 05 Oct 2022 07:26:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 05 Oct 2022 07:26:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 05 Oct 2022 07:26:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Oct 2022 07:26:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Oct 2022 07:26:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 05 Oct 2022 07:59:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 05 Oct 2022 07:59:10 GMT
ENV PHP_VERSION=8.1.11
# Wed, 05 Oct 2022 07:59:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.11.tar.xz.asc
# Wed, 05 Oct 2022 07:59:12 GMT
ENV PHP_SHA256=3005198d7303f87ab31bc30695de76e8ad62783f806b6ab9744da59fe41cc5bd
# Wed, 05 Oct 2022 07:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 05 Oct 2022 07:59:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:03:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 05 Oct 2022 08:03:16 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:03:16 GMT
RUN docker-php-ext-enable sodium
# Wed, 05 Oct 2022 08:03:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 05 Oct 2022 08:03:18 GMT
STOPSIGNAL SIGWINCH
# Wed, 05 Oct 2022 08:03:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:03:20 GMT
WORKDIR /var/www/html
# Wed, 05 Oct 2022 08:03:21 GMT
EXPOSE 80
# Wed, 05 Oct 2022 08:03:22 GMT
CMD ["apache2-foreground"]
# Wed, 05 Oct 2022 22:46:45 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 22:46:46 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Oct 2022 22:46:47 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Wed, 05 Oct 2022 22:46:47 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Wed, 05 Oct 2022 22:46:48 GMT
WORKDIR /opt/drupal
# Wed, 05 Oct 2022 22:47:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 Oct 2022 22:47:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f294832078061b7415f272ec2761b7719b3e5280f601911d1a0a846bed1c697`  
		Last Modified: Wed, 05 Oct 2022 09:06:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb1423a6acc78299080d62705715735db968d712c0911f2a538c7bb78846c0c`  
		Last Modified: Wed, 05 Oct 2022 09:06:38 GMT  
		Size: 70.4 MB (70364283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881544aca2f719ccea538ad8809af4daf3fe9e67150d222ea07989311fe44c39`  
		Last Modified: Wed, 05 Oct 2022 09:06:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae13209809b5abef3c1b647925326afb012b6511c81cffb8c712758f3caa187e`  
		Last Modified: Wed, 05 Oct 2022 09:07:01 GMT  
		Size: 18.4 MB (18368122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01584fbc5074a7a7d1e26d03de2482b150008be4f61939960aa3f146e10b46`  
		Last Modified: Wed, 05 Oct 2022 09:06:58 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5248523969968f0f8f49ada0b881a295b69fe3ad0d0e8ae40a533be4975808`  
		Last Modified: Wed, 05 Oct 2022 09:06:58 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ce6ce758f12377e36a9b1c3270b7fe1304264102151aadf697dc91565b897f`  
		Last Modified: Wed, 05 Oct 2022 09:11:16 GMT  
		Size: 11.9 MB (11922051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fbf7301d45c60b680a08642c05c1fa74219c0ba105294ea378d32c49788b64`  
		Last Modified: Wed, 05 Oct 2022 09:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb3bc4c0b7fa0b85a7dac8123eda38dd1fd92e032f8fac70f270c149bcb72d6`  
		Last Modified: Wed, 05 Oct 2022 09:11:15 GMT  
		Size: 11.1 MB (11072287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f049b242b777759e286b0513f6af5368c1b3b41acb53691337d4c0c56879ef`  
		Last Modified: Wed, 05 Oct 2022 09:11:13 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63ebdc635b07fd607a3931a01ffbe5f8dff8763a0398b172db489c8aa5a1371`  
		Last Modified: Wed, 05 Oct 2022 09:11:13 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00785198b5e25a5c988c3f0335f431a9495c7c0afb86d145427c983c855f3ef5`  
		Last Modified: Wed, 05 Oct 2022 09:11:13 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d372c3010812db713f1f16b4c89ee30c79fc872bc3172ffeac6a7a6d785115b`  
		Last Modified: Wed, 05 Oct 2022 23:24:14 GMT  
		Size: 2.1 MB (2141115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5c86525d58b77cbbada02ed1dfbd3c3b9afacbf54d66363d18b685d5f883b`  
		Last Modified: Wed, 05 Oct 2022 23:24:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ff1936b14d47b5da7f1e4d3ae3f5eba7eac270ed78cbaa751265dea7458390`  
		Last Modified: Wed, 05 Oct 2022 23:24:13 GMT  
		Size: 692.6 KB (692588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3577730093988d42af14d69c282dddf8066e298b9498ff1ff44060a618c58b`  
		Last Modified: Wed, 05 Oct 2022 23:24:13 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89d2f28f0f1bc7105e21af6b89ffe964d9937d71d644eb60bc6b24059000585`  
		Last Modified: Wed, 05 Oct 2022 23:24:18 GMT  
		Size: 17.6 MB (17577979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:c1a4ff5a644762879bcc72af331fe8e09fe85c7e8b8e06231a4effc3e6ce122a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.3 MB (171286062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb30dfc7481c30e8ebdeaa3cfb975a2540e0ee27e30023cf029824fd1f7f388`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:08 GMT
ADD file:b1ef7e7f4c48770bde0d19751bb1624a887b657a5a5ab5d453fd5365b3448618 in / 
# Tue, 04 Oct 2022 23:40:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:32:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 05 Oct 2022 05:32:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 05 Oct 2022 05:32:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:32:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 05 Oct 2022 05:32:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 05 Oct 2022 05:36:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 05 Oct 2022 05:36:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 05 Oct 2022 05:36:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 05 Oct 2022 05:36:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 05 Oct 2022 05:36:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 05 Oct 2022 05:36:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Oct 2022 05:36:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Oct 2022 05:36:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 05 Oct 2022 06:01:56 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 05 Oct 2022 06:01:57 GMT
ENV PHP_VERSION=8.1.11
# Wed, 05 Oct 2022 06:01:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.11.tar.xz.asc
# Wed, 05 Oct 2022 06:01:59 GMT
ENV PHP_SHA256=3005198d7303f87ab31bc30695de76e8ad62783f806b6ab9744da59fe41cc5bd
# Wed, 05 Oct 2022 06:02:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 05 Oct 2022 06:02:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 05 Oct 2022 06:04:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 05 Oct 2022 06:04:52 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 05 Oct 2022 06:04:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 05 Oct 2022 06:04:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 05 Oct 2022 06:04:54 GMT
STOPSIGNAL SIGWINCH
# Wed, 05 Oct 2022 06:04:56 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 05 Oct 2022 06:04:56 GMT
WORKDIR /var/www/html
# Wed, 05 Oct 2022 06:04:57 GMT
EXPOSE 80
# Wed, 05 Oct 2022 06:04:58 GMT
CMD ["apache2-foreground"]
# Wed, 05 Oct 2022 15:16:02 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:16:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Oct 2022 15:16:05 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Wed, 05 Oct 2022 15:16:05 GMT
ENV DRUPAL_VERSION=10.0.0-beta2
# Wed, 05 Oct 2022 15:16:06 GMT
WORKDIR /opt/drupal
# Wed, 05 Oct 2022 15:16:20 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 Oct 2022 15:16:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d1d1dd08a5009b10b72285f23ffd4c1978d3445cc3855d22f4112018b15a9420`  
		Last Modified: Tue, 04 Oct 2022 23:46:26 GMT  
		Size: 27.8 MB (27797501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ef26ef223ed430be44b1235ee1081af95576204d4884d89a6e84dac64e910f`  
		Last Modified: Wed, 05 Oct 2022 07:06:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94647b3f1d6fd0bcf270dc4840a5ae6379b62e6d764b8b8d2937a0ab3a59b1c7`  
		Last Modified: Wed, 05 Oct 2022 07:06:31 GMT  
		Size: 81.2 MB (81230534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91945b578017157defacefb4c3d8bd957711756468948721f363702724ba8a60`  
		Last Modified: Wed, 05 Oct 2022 07:06:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290adc7cc28a1d3d90e930ddae2334588586c9eb0c7a221199a12806510639ed`  
		Last Modified: Wed, 05 Oct 2022 07:06:56 GMT  
		Size: 18.9 MB (18900656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80107ede7cd4b39b296becad1595f86914f27fd5895208ae467bde3525861dad`  
		Last Modified: Wed, 05 Oct 2022 07:06:53 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3aeb6a27065fdaee49f3b16b90097b252c18b0b9b61c8fd9255fb58b293763`  
		Last Modified: Wed, 05 Oct 2022 07:06:52 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4673b1a77dd86c7f90e096b5eecd06426c1c84e6ecb20277bcebb26cc28ca0`  
		Last Modified: Wed, 05 Oct 2022 07:11:37 GMT  
		Size: 11.9 MB (11922583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6d63c853aa0a0c1d8ba0d48d397df1c6a9c8e546275fabe2418b46d18080d0`  
		Last Modified: Wed, 05 Oct 2022 07:11:34 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5260ce4729568d81abedd011b598962e67f868af9a8f91cae9bf0674c3f985`  
		Last Modified: Wed, 05 Oct 2022 07:11:36 GMT  
		Size: 11.2 MB (11214750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d08f6b79dc00c492db52082f5a52e8908eb0dfdaffc0e47ce5684e227536c0`  
		Last Modified: Wed, 05 Oct 2022 07:11:34 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531709327d00109f4e63789eb26feeba95be8dd184406b00ecac6b36751cb05d`  
		Last Modified: Wed, 05 Oct 2022 07:11:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dfa7e7732d5ec487038bd8054d7af69ff71296828459af5a3a545588ba3259`  
		Last Modified: Wed, 05 Oct 2022 07:11:34 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d529928e5e733296414633be84a73c8068e366bc87035199c08c560c5339b772`  
		Last Modified: Wed, 05 Oct 2022 15:49:46 GMT  
		Size: 1.9 MB (1943488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4f679cba93f87d3e986a3028a3276fbee7cc9b71098f9440d72fe212825c27`  
		Last Modified: Wed, 05 Oct 2022 15:49:46 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f27e9298943c526696cd4813f7d2864fa31146b6afa739fd44cbbb930c6f38`  
		Last Modified: Wed, 05 Oct 2022 15:49:46 GMT  
		Size: 692.6 KB (692585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8504ae41a25a7678c69edc58bc0862ca88cd444caf3bc3b72b51bc88571bc5f`  
		Last Modified: Wed, 05 Oct 2022 15:49:46 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39317a073ed104c5694a56cb5999ba29a5bbf8a6b8c4354d0405f5fca7f477d`  
		Last Modified: Wed, 05 Oct 2022 15:49:51 GMT  
		Size: 17.6 MB (17578058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
