## `drupal:9-php7.4-apache-buster`

```console
$ docker pull drupal@sha256:1ecdbb81a2dcf754d766faad5a2bfea36971c3d0a3356a14fe19be67146e4f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:9-php7.4-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:fe140b483967866fe038a41118556599854ce8064c25a317f27606b4ceae822f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168756388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df914cf4c2fe2362904052206aa6cf6fdde334ba9b3eab6a7a588f486ac4ec1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 09:58:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 09:58:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 09:58:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 09:58:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 09:58:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 10:02:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 10:02:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 10:02:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 10:02:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 10:02:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 10:02:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 10:02:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 10:02:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 11:16:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 14:35:11 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 14:35:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 14:35:11 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 14:35:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Sep 2022 14:35:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 14:37:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 14:37:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 29 Sep 2022 14:37:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 14:37:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 14:37:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 29 Sep 2022 14:37:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 29 Sep 2022 14:37:26 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 14:37:26 GMT
EXPOSE 80
# Thu, 29 Sep 2022 14:37:27 GMT
CMD ["apache2-foreground"]
# Thu, 29 Sep 2022 15:58:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 29 Sep 2022 15:58:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 15:58:34 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 20:01:10 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 20:01:10 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 20:01:21 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 20:01:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7926108d61967de3c3b394f117df9a36ef11dcc7cc15729265869f6e5318a82e`  
		Last Modified: Tue, 13 Sep 2022 11:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a32af496e5b7b67ea2e864ade872ec4811aa871eb14dd3dd8e1cdfb3acc5427`  
		Last Modified: Tue, 13 Sep 2022 11:30:20 GMT  
		Size: 76.7 MB (76685702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48af7de5a6952f43c58d2fb6f3a24ee447392b1bf3d720a9ec69b690c7717ae7`  
		Last Modified: Tue, 13 Sep 2022 11:30:08 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa4808661da9ef3a05ed6368fbf9d8dd15cba9c3a812d28b227f66b14de5684`  
		Last Modified: Tue, 13 Sep 2022 11:30:41 GMT  
		Size: 18.7 MB (18682052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0cd632b13a6c1270788d4626fe9eae2b513f2ea1be092d8f5b05ab55124561`  
		Last Modified: Tue, 13 Sep 2022 11:30:38 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2248ede2395b89c0e8f3585bf3297c39ff9df8f1e3729213bd33fcb61b9d68df`  
		Last Modified: Tue, 13 Sep 2022 11:30:38 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b256be506a508cdbf9cd15be2d87876788fa7fc315bfd380f0a2f96d6af60b5`  
		Last Modified: Thu, 29 Sep 2022 15:14:49 GMT  
		Size: 10.8 MB (10756783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77407e2fabc071b23c7c2465a4e1a9e6892def1e840072881a6a702182bf4921`  
		Last Modified: Thu, 29 Sep 2022 15:14:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140e0f9e476bc487cfeb6e21c00c52faa3c6d757b306bfc4a0af09dcf8ec9046`  
		Last Modified: Thu, 29 Sep 2022 15:14:48 GMT  
		Size: 11.0 MB (11021897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e654333d239436cc1a6be6dcf7dd6441513ba1093797af3c66ac2f2bed7578`  
		Last Modified: Thu, 29 Sep 2022 15:14:46 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c247f2a6415937b792ab643cd81cf09967f3e4115e3ea9f1add2de2090e8e1a`  
		Last Modified: Thu, 29 Sep 2022 15:14:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50d673086b74eac02af9c6916d1d273e67aa8cbfa518ea1a2d87cc27adf66f6`  
		Last Modified: Thu, 29 Sep 2022 15:14:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03aad589e59b455b2037845d9edb25b3a4450533bfab8c96254aa97ef8024174`  
		Last Modified: Thu, 29 Sep 2022 16:12:20 GMT  
		Size: 1.9 MB (1900078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c7ca6e259fdcbdf4ae447504524499b8e168474cc332616a1b106ae49c775c`  
		Last Modified: Thu, 29 Sep 2022 16:12:20 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9e0f4dbff01fbbdb19e369cb4aae13fb053b22cebf1bec151455bfe73bcfab`  
		Last Modified: Thu, 29 Sep 2022 16:12:20 GMT  
		Size: 692.6 KB (692587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e820029c50639cdb3d277d0d2e21f8f3b587fe9feae673e2b2214f14692eced4`  
		Last Modified: Thu, 29 Sep 2022 20:26:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec619c9c9e18c7da8af581273cdcaec5dd3f5160ac6db14659394121d114e0c7`  
		Last Modified: Thu, 29 Sep 2022 20:26:14 GMT  
		Size: 21.9 MB (21880676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:d74b728043c2f4d3869e414a8a80afd9ae9c7840ec982d4eb1b06ea8a7de0b14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144456871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a64ceab771929b0c3832a6c8a38e6ca9a16763a51d51b0aaa1423e55a069fab6`
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
# Tue, 13 Sep 2022 23:28:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 15:52:19 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 15:52:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 15:52:19 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 15:52:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Sep 2022 15:52:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:00:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 16:00:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:00:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 16:00:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 16:00:10 GMT
STOPSIGNAL SIGWINCH
# Thu, 29 Sep 2022 16:00:11 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:00:11 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 16:00:11 GMT
EXPOSE 80
# Thu, 29 Sep 2022 16:00:11 GMT
CMD ["apache2-foreground"]
# Thu, 29 Sep 2022 21:59:30 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 29 Sep 2022 21:59:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 21:59:30 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 21:59:30 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 21:59:31 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 22:00:03 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 22:00:04 GMT
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
	-	`sha256:2b2989582783ec8e30fe73d0f5159e0a211f6f3a8b198e6b9bbf1ffb8bae1f28`  
		Last Modified: Thu, 29 Sep 2022 18:09:14 GMT  
		Size: 10.8 MB (10755042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76082e9813150f91b129606625bd77ac2052350b7eb02ea0ed749192f2b22a`  
		Last Modified: Thu, 29 Sep 2022 18:09:11 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb1fa5f9368bd7d1288f81bccca12bd9648c9ec33ab8f660a3235fb15111dbf`  
		Last Modified: Thu, 29 Sep 2022 18:09:13 GMT  
		Size: 9.7 MB (9745395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbd35d4bc1cb25dd406c4644d5a2d28d814da076923f1ea7f0a113ca65021cb`  
		Last Modified: Thu, 29 Sep 2022 18:09:11 GMT  
		Size: 2.5 KB (2464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4297379b126d9d39abe47e5964a1e73a9aa53a37d2991b1b016a8d7be2d1d0c4`  
		Last Modified: Thu, 29 Sep 2022 18:09:11 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c3925cfd8337e19549d14c7a7bb701d3ece5f854df48ef824ad54138db1ea3`  
		Last Modified: Thu, 29 Sep 2022 18:09:11 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3daa2292eccee14607deb76fb141131616aee4383a517f61978858dbcd65775`  
		Last Modified: Thu, 29 Sep 2022 22:50:01 GMT  
		Size: 1.6 MB (1616228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c0b6af7137473a856aaf78288ab5b12ef7f0ba912f99e3e26ddd35ca18ad10`  
		Last Modified: Thu, 29 Sep 2022 22:50:01 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5686cb455ccf1b145df1c9f5092d104b776049dce0ef9c2a6e0929dba770dfc6`  
		Last Modified: Thu, 29 Sep 2022 22:50:01 GMT  
		Size: 692.6 KB (692595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07792a2bc48a0d3cb64f1c66cd6fbb41547f1e54495b65aa4c6242fe5a6518ef`  
		Last Modified: Thu, 29 Sep 2022 22:50:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b74e6688966068aa380b77b9f01ca6f038f5f4f187cc704aab32b9ae8257bc`  
		Last Modified: Thu, 29 Sep 2022 22:50:21 GMT  
		Size: 21.9 MB (21880733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:ae3c882a5b0959291b8ec287eaae909518472de0206e8be88bff1183f46f444c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.4 MB (159401212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d835896732c27309ca6dfd47e79874f3b72b700413476dbb48f07b1c99077440`
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
# Wed, 05 Oct 2022 08:48:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 05 Oct 2022 08:48:22 GMT
ENV PHP_VERSION=7.4.32
# Wed, 05 Oct 2022 08:48:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Wed, 05 Oct 2022 08:48:24 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Wed, 05 Oct 2022 08:48:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 05 Oct 2022 08:48:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:50:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 05 Oct 2022 08:50:28 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:50:28 GMT
RUN docker-php-ext-enable sodium
# Wed, 05 Oct 2022 08:50:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 05 Oct 2022 08:50:30 GMT
STOPSIGNAL SIGWINCH
# Wed, 05 Oct 2022 08:50:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 05 Oct 2022 08:50:32 GMT
WORKDIR /var/www/html
# Wed, 05 Oct 2022 08:50:33 GMT
EXPOSE 80
# Wed, 05 Oct 2022 08:50:34 GMT
CMD ["apache2-foreground"]
# Wed, 05 Oct 2022 23:00:58 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 23:00:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Oct 2022 23:01:01 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Wed, 05 Oct 2022 23:01:01 GMT
ENV DRUPAL_VERSION=9.4.7
# Wed, 05 Oct 2022 23:01:02 GMT
WORKDIR /opt/drupal
# Wed, 05 Oct 2022 23:01:21 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 Oct 2022 23:01:23 GMT
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
	-	`sha256:2d2dcec1a2d54725713dd82cdc4ea3a9bf5366b947e8740178626f33fd053120`  
		Last Modified: Wed, 05 Oct 2022 09:18:33 GMT  
		Size: 10.5 MB (10543386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a94e55c2a38fd49d496a324f7088b4c97d25e0576c4cc52cb67d9deca60892`  
		Last Modified: Wed, 05 Oct 2022 09:18:30 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e555cdc672c0aed5e2f6b4f2e1968e133cdd1d110af3afa2449ae69928e122a`  
		Last Modified: Wed, 05 Oct 2022 09:18:32 GMT  
		Size: 10.0 MB (9963996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1cf08c214fbc670e11137bc68b12a8357ff644f37b3d53d4bf26088abef316`  
		Last Modified: Wed, 05 Oct 2022 09:18:30 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849ff1a3f8b57c23d625b0bd55f83c56fde7c8faaa5b58a56ceddbef82fdc12`  
		Last Modified: Wed, 05 Oct 2022 09:18:30 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b032f3a9d6ea9b232a743b43f9361623f7d7e4fa25191a2d8f51cebe38a748d`  
		Last Modified: Wed, 05 Oct 2022 09:18:30 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c491a817c89de85d571bfc30357c616af0e561a3452c558c3f96b4d0289a86`  
		Last Modified: Wed, 05 Oct 2022 23:34:27 GMT  
		Size: 1.7 MB (1668815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa1a8f3f0f20844926e077bf0c4554c52c84df104febc5b105f099f4c03cb53`  
		Last Modified: Wed, 05 Oct 2022 23:34:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f340a82de331fbc1966f82cc27c0a4c4347d8a5c660682eb6b65045780a4b5c`  
		Last Modified: Wed, 05 Oct 2022 23:34:26 GMT  
		Size: 692.6 KB (692588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc865123e49d859f6b77938b04c95ba328042f9f94fd01c796c758230dd56e73`  
		Last Modified: Wed, 05 Oct 2022 23:34:26 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daef6b1b736faf2f8358354f9d00080895c149dc97e81ad1586d518968c934a`  
		Last Modified: Wed, 05 Oct 2022 23:34:32 GMT  
		Size: 21.9 MB (21882223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:baf274170c998defa4b7f663383476ae738e8cf42389732e8bdb033adbe70814
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173223879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc09f30a268e96297ee7e50b37a0ed2654920226d5b77faad38ffe313c40f027`
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
# Wed, 05 Oct 2022 06:48:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 05 Oct 2022 06:48:08 GMT
ENV PHP_VERSION=7.4.32
# Wed, 05 Oct 2022 06:48:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Wed, 05 Oct 2022 06:48:10 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Wed, 05 Oct 2022 06:48:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 05 Oct 2022 06:48:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 05 Oct 2022 06:50:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 05 Oct 2022 06:50:06 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 05 Oct 2022 06:50:06 GMT
RUN docker-php-ext-enable sodium
# Wed, 05 Oct 2022 06:50:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 05 Oct 2022 06:50:08 GMT
STOPSIGNAL SIGWINCH
# Wed, 05 Oct 2022 06:50:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 05 Oct 2022 06:50:10 GMT
WORKDIR /var/www/html
# Wed, 05 Oct 2022 06:50:11 GMT
EXPOSE 80
# Wed, 05 Oct 2022 06:50:12 GMT
CMD ["apache2-foreground"]
# Wed, 05 Oct 2022 15:28:08 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:28:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Oct 2022 15:28:11 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Wed, 05 Oct 2022 15:28:11 GMT
ENV DRUPAL_VERSION=9.4.7
# Wed, 05 Oct 2022 15:28:12 GMT
WORKDIR /opt/drupal
# Wed, 05 Oct 2022 15:28:25 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 Oct 2022 15:28:26 GMT
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
	-	`sha256:b0af69bb6057c2c0971fa7d2456ecdda3825c27c19a897675db630689697f81e`  
		Last Modified: Wed, 05 Oct 2022 07:19:04 GMT  
		Size: 10.5 MB (10543914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c5e83b1d766fa34c285d11803550b394bfbe885924b5b47b07f79cecdb0fa1`  
		Last Modified: Wed, 05 Oct 2022 07:19:01 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e6a962ed8d4e49a950412e6d0b9ff90e2004f23758773d4a6ff30e7c62c16d`  
		Last Modified: Wed, 05 Oct 2022 07:19:03 GMT  
		Size: 10.4 MB (10391049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635abb6f260ad644ee0231f331e4f4f2d07a082b6a19f3bb0b0396159b05317`  
		Last Modified: Wed, 05 Oct 2022 07:19:01 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1495174b186471781622643a351354c1f0644b8d8f6462d511e025f07ea74dc`  
		Last Modified: Wed, 05 Oct 2022 07:19:01 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf81c064019a7d6d76322b7bd6bc1afe782c019336e6abb8ed6c878648e75e94`  
		Last Modified: Wed, 05 Oct 2022 07:19:01 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574444f4b0ac2495d470e5f36af98b754e1b06febe3823c1b96bce870d7b35ae`  
		Last Modified: Wed, 05 Oct 2022 15:59:54 GMT  
		Size: 1.8 MB (1779761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108bca9ae0864315d94df248518b190a60c4466218542434a98bcc6cbd98f4ca`  
		Last Modified: Wed, 05 Oct 2022 15:59:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67681dbc6b39f1edb5ff171c35c4be200d1d3cb8ebe8da550f733c78f23405c5`  
		Last Modified: Wed, 05 Oct 2022 15:59:54 GMT  
		Size: 692.6 KB (692585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0de37a58b9b78a49f4eb7fe6db9a7538fca6996a529fd5d8b9b5faf4c84d42`  
		Last Modified: Wed, 05 Oct 2022 15:59:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69f9e66f51b5b0a476cca747998afe11f2222e127ce314f22f779f15fc50e73`  
		Last Modified: Wed, 05 Oct 2022 16:00:00 GMT  
		Size: 21.9 MB (21881978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
