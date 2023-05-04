## `drupal:9-php8.0-apache-buster`

```console
$ docker pull drupal@sha256:096e4746d1bc28f73464ba318630ace32488727893e7c8a8939d777c97753f8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:9-php8.0-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:c33747621523befbe94cac61aa3a91d0a3269c51e6fd2f9e60aeda195391613a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170204991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dacfb980cb591040fd1dca21ba7f6112eed4edc03c2a7bbe221396cfe006465`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:44:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:44:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:44:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:44:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:44:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:48:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:48:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:48:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:48:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:48:30 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:48:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:48:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:48:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 05:32:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 05:32:01 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 05:32:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 05:32:01 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 05:32:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 05:32:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:35:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 05:35:01 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:35:02 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 05:35:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 05:35:02 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 05:35:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:35:02 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 05:35:02 GMT
EXPOSE 80
# Wed, 12 Apr 2023 05:35:02 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 11:39:51 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 11:39:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 11:39:51 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 22:24:24 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 22:24:24 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 22:24:34 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 22:24:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abc141d8a2f096cdcf270bfbbb8955898adc6be2c5458b8168559dcd67169`  
		Last Modified: Wed, 12 Apr 2023 05:44:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5e539f1793f643bd81ceb8fd73b581e2e4078cb3bb5d738204614f50520ee3`  
		Last Modified: Wed, 12 Apr 2023 05:44:33 GMT  
		Size: 76.7 MB (76693050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db22bb7dedbf0dea869e86ec5db1a578254d435219591a7099a0303880db235`  
		Last Modified: Wed, 12 Apr 2023 05:44:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d16eee0e00ffce627379730b8dbb2c23062597a5d8d60646690db77595bbd1`  
		Last Modified: Wed, 12 Apr 2023 05:44:50 GMT  
		Size: 18.7 MB (18686859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d06ccd7d353c777583d2aef15b62555cafa0a1e5cf7ce237ce2a78c234eed3`  
		Last Modified: Wed, 12 Apr 2023 05:44:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b0c62691b2eb2d2c140fe25f9c2c6a545b2378e8699da2534414873937336e`  
		Last Modified: Wed, 12 Apr 2023 05:44:47 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c241dda83c18d8778107ca1cad7708427721a6f4f72de6fa60dc086d6cc8722a`  
		Last Modified: Wed, 12 Apr 2023 05:54:37 GMT  
		Size: 11.1 MB (11141059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a440f0ae024a738163b4c288402edeb8fbdddb87ce4ade0dd669b04e969705f`  
		Last Modified: Wed, 12 Apr 2023 05:54:34 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0b18761505d018a482e3a489c811e8362fb7335b0a4ae87546172719bed58a`  
		Last Modified: Wed, 12 Apr 2023 05:54:36 GMT  
		Size: 10.7 MB (10726476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ad27ecf8b4d7cca231b56d494eb453c35b907ca05bc3d5e63b481333129e20`  
		Last Modified: Wed, 12 Apr 2023 05:54:34 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc567bf200cae3168eb4ce3a952cf220e549682dd9096e0425d5c470a9cb304`  
		Last Modified: Wed, 12 Apr 2023 05:54:34 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dd1075f2379fa276eb3b772e1960f50690476f36a77c86218480e90baaad1b`  
		Last Modified: Wed, 12 Apr 2023 05:54:34 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b65058e647ce4a4f74622eb98a21f1e07492c55c6992d4bf09c35e9a2fa4a1f`  
		Last Modified: Wed, 12 Apr 2023 11:52:53 GMT  
		Size: 2.2 MB (2247776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6544a0d0daacd6670c0810403b4620ca52c46f25b9410b7c690072e39758f8d9`  
		Last Modified: Wed, 12 Apr 2023 11:52:53 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081290735b435fd36d7852005401e0324bfa556e8667673167e19282231394f2`  
		Last Modified: Wed, 12 Apr 2023 11:52:53 GMT  
		Size: 697.5 KB (697531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe2e3116064d8323aea70be0b551fa55268b4383b6eef1bf36c76dc73503b63`  
		Last Modified: Thu, 20 Apr 2023 22:41:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc9496d730824c6b59c7a7f58fe5fa98bcbd439f41fbe0b2f50c90546684d4`  
		Last Modified: Thu, 20 Apr 2023 22:41:06 GMT  
		Size: 22.9 MB (22867281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:f92861ac387a80f10efc4b7861c4da65439b463d5a02f0740e2d5fe87a1f444e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145372275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891980fd2d7e45ab40269707b9b84db2bea147b65514ce11b9975c248e37f0b1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:02 GMT
ADD file:72785c92abeacda7808e9e65787e604ed7fbc159c53eb4b2337628501418e9ce in / 
# Wed, 12 Apr 2023 00:00:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:47:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:47:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:47:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:47:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:47:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 02:50:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 02:50:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 02:51:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 02:51:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 02:51:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 02:51:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:51:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:51:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:18:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 04:18:34 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 04:18:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 04:18:34 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 04:18:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:18:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:20:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 04:20:57 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:20:57 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 04:20:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 04:20:58 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 04:20:58 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:20:58 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 04:20:58 GMT
EXPOSE 80
# Wed, 12 Apr 2023 04:20:58 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 10:50:11 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 10:50:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 10:50:12 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 23:32:47 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 23:32:47 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 23:33:19 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 23:33:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:2f777f2c33b3c8a258e4118224a280169c60be31db805388525da1f620f59a86`  
		Last Modified: Wed, 12 Apr 2023 00:03:58 GMT  
		Size: 22.7 MB (22747664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3f4f788163258f651c15735b37581f8ab347f41135709e56b7fef261646ce5`  
		Last Modified: Wed, 12 Apr 2023 04:29:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319605d85c72d8f79f93c202d32813b850eacee30c03352db28b27fc8c4cdc25`  
		Last Modified: Wed, 12 Apr 2023 04:29:42 GMT  
		Size: 59.5 MB (59543394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86d5cdf08a337d824cacd8c4a3cae11a14be3dfd59d80ef2cbe4c6e1dac4a78`  
		Last Modified: Wed, 12 Apr 2023 04:29:31 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bcd269a6e344d3bfba6155df77630dc7e12c47673afcb31169ae14fdaab243`  
		Last Modified: Wed, 12 Apr 2023 04:29:59 GMT  
		Size: 17.5 MB (17481740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dab86b7af9a45f71eb6cfb2950165732aebe9cfe880b71cd52acef43112248`  
		Last Modified: Wed, 12 Apr 2023 04:29:56 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc541ff01dc31675c89fd9c0c39f8ebfb77ca89d19959fe9e567f6210c446e0`  
		Last Modified: Wed, 12 Apr 2023 04:29:56 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bebf80293112a0d9695be8c3d5b79c6c88a167269a5b9d78038f401bbeb99fb`  
		Last Modified: Wed, 12 Apr 2023 04:39:42 GMT  
		Size: 11.1 MB (11138906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90eebab696b699c2c8726882657c5b119876c0dee1865a14099e76eca61f7911`  
		Last Modified: Wed, 12 Apr 2023 04:39:39 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0698b68de6489130a8a8d1b1a2929cf13e995e8325bf957b985fc7c09ade44b`  
		Last Modified: Wed, 12 Apr 2023 04:39:42 GMT  
		Size: 9.3 MB (9256689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5303cafc8ff2443b1acab35702430b8ccd46cdd428e21a3ee8fb27e64d4866`  
		Last Modified: Wed, 12 Apr 2023 04:39:39 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d794cf73ddc0d9295bdcee566d5c2c654ecf380c242e187040432bfe031f4fa5`  
		Last Modified: Wed, 12 Apr 2023 04:39:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca39b2c3e14de63f8fcc07d10a4ede188dc7f87176492d91082b526eef507bf`  
		Last Modified: Wed, 12 Apr 2023 04:39:39 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6b59c39dc4beb4af34bbb9578a617136b574a1c04c84d6537828e3cbcad008`  
		Last Modified: Wed, 12 Apr 2023 11:05:27 GMT  
		Size: 1.6 MB (1633058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e6148f04b3bf67ddb252e23a1985d06e9ab371d70c420a0d502e3be5ccf097`  
		Last Modified: Wed, 12 Apr 2023 11:05:26 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6553a544633c0d4146499be5f25045760716cad6d5d852c91c2b8c428f614ebe`  
		Last Modified: Wed, 12 Apr 2023 11:05:26 GMT  
		Size: 697.5 KB (697531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45821341502c6a22f2f7cf2820b4b98894ecd622ce7b8011ffd546a04d58b15`  
		Last Modified: Thu, 20 Apr 2023 23:52:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0850313bd9f21b987686b623bfe47c292bd49e5f948b5aa6d4d06cf8446c61fa`  
		Last Modified: Thu, 20 Apr 2023 23:52:38 GMT  
		Size: 22.9 MB (22867263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:d61ca7f6e0c860a7878b0850d5d4562da06198a5de930f0bc6cfa5287f978919
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.7 MB (161698846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4527034fb41ef1d2109e2938e9db1d909e37691522866eb96e984baa2de8d030`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 04:05:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 04:05:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 04:06:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 04:06:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 04:06:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 04:09:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 04:09:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 04:09:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 04:09:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 04:09:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 04:09:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 04:09:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 04:09:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 05:42:29 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 05:42:29 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 05:42:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 05:42:29 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 05:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 05:42:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 05:44:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 05:44:41 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 05:44:41 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 05:44:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 05:44:41 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 05:44:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 05:44:41 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 05:44:41 GMT
EXPOSE 80
# Wed, 03 May 2023 05:44:42 GMT
CMD ["apache2-foreground"]
# Wed, 03 May 2023 23:17:45 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 03 May 2023 23:17:45 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Wed, 03 May 2023 23:17:45 GMT
ENV DRUPAL_VERSION=9.5.9
# Wed, 03 May 2023 23:17:45 GMT
WORKDIR /opt/drupal
# Wed, 03 May 2023 23:18:04 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 03 May 2023 23:18:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1eed75396074e4a334cbfa2e9f018727d6d9645818e26f818e58ab869b1cf6`  
		Last Modified: Wed, 03 May 2023 05:52:11 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237165e9d0718003bf4f084a14158d89f600091e3e6fad044addb827e4c02e1`  
		Last Modified: Wed, 03 May 2023 05:52:18 GMT  
		Size: 70.4 MB (70366411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63fae9b8b287117dd852404d06f2982cedfc392773a3550a80f8a890263b8c2`  
		Last Modified: Wed, 03 May 2023 05:52:10 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d395c2b7f79878dead98a97c8e62d97eba8218307dfc285c239cc70bdb0b493`  
		Last Modified: Wed, 03 May 2023 05:52:34 GMT  
		Size: 18.6 MB (18587020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62b10c78915532aab3dd7375bf561721bdd0489e030095f383d53c8017f60b4`  
		Last Modified: Wed, 03 May 2023 05:52:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a90b63c3b6fd4a0dfb67f2d260162b94e929a842e05590875cd3d0bd3a0396d`  
		Last Modified: Wed, 03 May 2023 05:52:32 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45145a54743067ad56c469e5ffece46a2177d5735cce9f62936eab53c78c5744`  
		Last Modified: Wed, 03 May 2023 06:02:03 GMT  
		Size: 11.1 MB (11139735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73958b88676df4a8560667be325e9c0a180ca3f2bdbeef4402653db43afec2de`  
		Last Modified: Wed, 03 May 2023 06:02:01 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96e1634755b25da696b9c43eca53f5b075f0c352e3512fdf3b0fd430854184f`  
		Last Modified: Wed, 03 May 2023 06:02:02 GMT  
		Size: 10.2 MB (10201827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4438ba5115862a27efed65e2e349edae7c678a7afd2b0528f3a07df883be2e6c`  
		Last Modified: Wed, 03 May 2023 06:02:01 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8764b00ae8049b48311320c9896580424435d01318da8efc356eeb4f96bc30d3`  
		Last Modified: Wed, 03 May 2023 06:02:01 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64711751ecec0c953aac85b22982754eb39d71e34b6bb1469a431d3ddc4e983a`  
		Last Modified: Wed, 03 May 2023 06:02:01 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb304ba868b7e1050a69ea626e04dd396641e3c3123fc53c051f9077d18a5799`  
		Last Modified: Wed, 03 May 2023 23:35:44 GMT  
		Size: 1.9 MB (1900257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0298ef1deba98f03c84b8e643a752f3cc432756ebc6dcb05420115c926c28`  
		Last Modified: Wed, 03 May 2023 23:35:43 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0088b67be34ec6a58446c613c29891182cd5c061171081f368c5e8dba9503274`  
		Last Modified: Wed, 03 May 2023 23:35:44 GMT  
		Size: 697.5 KB (697532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19cbb8697479012a574e30bbb07fcf8688f7a8957743a10e231678bc43a64e2`  
		Last Modified: Wed, 03 May 2023 23:35:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baecb4cb586f432ac3f6cf34e9735aae0b982c90b7ccd6b75cb517cb5c10c57`  
		Last Modified: Wed, 03 May 2023 23:35:47 GMT  
		Size: 22.9 MB (22877994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:1a861349a0545f4e2a2de1a4fb0e53d0794742ab6c79e50d8b5016ccf66df885
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176117135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7b41a42ca4cdf9b127ddb14e3b5d32260097beed059b20867c375c5706c7c9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:21 GMT
ADD file:0f4c5475f636be52b419806a7ea7d8d81fc1203c9228544c1324e79277739a3f in / 
# Wed, 12 Apr 2023 00:39:21 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:32:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 05:32:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 05:32:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:32:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 05:32:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 05:38:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 05:38:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 05:38:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 05:38:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 05:38:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 05:38:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:38:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:38:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 08:25:42 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 12 Apr 2023 08:25:43 GMT
ENV PHP_VERSION=8.0.28
# Wed, 12 Apr 2023 08:25:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 12 Apr 2023 08:25:43 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 12 Apr 2023 08:25:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 08:25:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:30:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 08:30:41 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:30:41 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 08:30:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 08:30:42 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 08:30:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:30:42 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 08:30:42 GMT
EXPOSE 80
# Wed, 12 Apr 2023 08:30:42 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 23:26:02 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 23:26:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 23:26:03 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 22:43:37 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 22:43:37 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 22:43:50 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 22:43:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ae6c02ab25c72d784ae8832cdcb583320ab9a3046938adc3c659ae607da19b43`  
		Last Modified: Wed, 12 Apr 2023 00:43:29 GMT  
		Size: 27.8 MB (27797581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e1f48a4bc80b7054b42143701c08cbf89d22af9c6c80dcc460033912c3d57a`  
		Last Modified: Wed, 12 Apr 2023 08:43:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4147d8a2fa45b9efa31f62f7bc8571416934b188e6d65672ea939ec7c11d836`  
		Last Modified: Wed, 12 Apr 2023 08:44:17 GMT  
		Size: 81.2 MB (81237423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accec47a5a7eee4ceb9702fa00d0efd5137fd4c2c280d2c296fa4ad1dedd982d`  
		Last Modified: Wed, 12 Apr 2023 08:43:59 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7ab116483cffade5ca90343f882dca71cddebf203fe4f07cf6f1e9ffa6c0a2`  
		Last Modified: Wed, 12 Apr 2023 08:44:36 GMT  
		Size: 19.1 MB (19117880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dc15d7898c63d7f749721b9bb0efe8249cc30b2eed8ed2c1782a751a1795ed`  
		Last Modified: Wed, 12 Apr 2023 08:44:32 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7821bc1551e5702d4374cb4e74e5f1e9493f3255155ef3b6902890ed5fe1e7fd`  
		Last Modified: Wed, 12 Apr 2023 08:44:32 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56171fa591ba82ea882fa9aa4d98d0e753321c046b380fcad8c53436d60a057`  
		Last Modified: Wed, 12 Apr 2023 08:55:10 GMT  
		Size: 11.1 MB (11140340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d88adf6ed9c688d7a21369675f2eb1cd40a866da18fc7e41175cc8e9c858959`  
		Last Modified: Wed, 12 Apr 2023 08:55:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a454bd9241b77432fc7da8e3925c1bc67ec2c64a7e93cc9d76b7f5d6ddf3c766`  
		Last Modified: Wed, 12 Apr 2023 08:55:10 GMT  
		Size: 10.9 MB (10937753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78adbccdd3024c3c216a2aaacf33a489b2edf418a4f86d0a1b42dedd0ce55df2`  
		Last Modified: Wed, 12 Apr 2023 08:55:07 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e5c706e6ae3c78ba3712484cf41c2c011bc2c451382be32e9571728400804b`  
		Last Modified: Wed, 12 Apr 2023 08:55:07 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c8e8e3b9e8ad49030213a09fe90d1f16d13d44b33dc1b6ebe00651972e94b2`  
		Last Modified: Wed, 12 Apr 2023 08:55:07 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3678d4466cad91df703887b358d4eacbeacbcc3d4bb0ef54cb71519023320c4`  
		Last Modified: Wed, 12 Apr 2023 23:40:37 GMT  
		Size: 2.3 MB (2316500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26464073051a0aef17088da598390acc6bd0e5196674bdaf2c46b37b6274724a`  
		Last Modified: Wed, 12 Apr 2023 23:40:36 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1002f6ab7a70a57497c9b4545b8689289af1d7985ee341147c96c7fa8fa894d`  
		Last Modified: Wed, 12 Apr 2023 23:40:36 GMT  
		Size: 697.5 KB (697533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502287cc00fb0d661d05642ab81832f0fc0098312f91e52888911b8d6fb25ef1`  
		Last Modified: Thu, 20 Apr 2023 23:02:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e4f66677689a002b92f0377d6052093ae5e214f83090350bf6063d191c892`  
		Last Modified: Thu, 20 Apr 2023 23:02:13 GMT  
		Size: 22.9 MB (22866099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
