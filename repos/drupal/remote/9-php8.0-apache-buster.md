## `drupal:9-php8.0-apache-buster`

```console
$ docker pull drupal@sha256:b3663d83147e9f30e3160a15b60725da0ec55d8083021eb60307660d1382eef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:9-php8.0-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:2558c2dfbabd9affc56c9f260867201ed724479025310a5be1e63e370801a47e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170246387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8653d4d9a0db125cd2e8eca2a659ca11de0090ea40d0f8895748425e9f689c2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:20:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 05:20:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 05:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:20:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 05:20:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 05:24:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 05:24:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 05:24:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 05:24:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 05:24:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 05:24:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:24:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:24:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 07:11:02 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 21 Dec 2022 07:11:02 GMT
ENV PHP_VERSION=8.0.26
# Wed, 21 Dec 2022 07:11:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Wed, 21 Dec 2022 07:11:02 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Wed, 21 Dec 2022 07:11:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 07:11:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:14:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 07:14:11 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:14:12 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 07:14:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 07:14:12 GMT
STOPSIGNAL SIGWINCH
# Wed, 21 Dec 2022 07:14:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:14:12 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 07:14:12 GMT
EXPOSE 80
# Wed, 21 Dec 2022 07:14:12 GMT
CMD ["apache2-foreground"]
# Wed, 21 Dec 2022 13:31:11 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:31:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 13:31:12 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Wed, 21 Dec 2022 13:31:12 GMT
ENV DRUPAL_VERSION=9.5.0
# Wed, 21 Dec 2022 13:31:12 GMT
WORKDIR /opt/drupal
# Wed, 21 Dec 2022 13:31:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 21 Dec 2022 13:31:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5e7e2c529af2f434f1cd170dacc2d1d41e98be050c7513fcf7967a1366ccab`  
		Last Modified: Wed, 21 Dec 2022 07:26:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d385a4ba170008aa047844209f3315470643dd6cf691a34edb91a2b2fc50d1b`  
		Last Modified: Wed, 21 Dec 2022 07:26:43 GMT  
		Size: 76.7 MB (76687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07776926a26c83e59429f19e43d5f71af16d4beee2837c3c5873353005c859b8`  
		Last Modified: Wed, 21 Dec 2022 07:26:31 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ef243fc95955dd3f0c6d6935bc05e6ba16b9438cd6e09d34a9c382e447813`  
		Last Modified: Wed, 21 Dec 2022 07:27:00 GMT  
		Size: 18.7 MB (18684910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b1be175ef3b283aea7539d0cfb4ef65c25edbc5228136a4c05d1e71b305ced`  
		Last Modified: Wed, 21 Dec 2022 07:26:58 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0285f3aabfba16572b76b4ef98e5a29df703fac45d6da70db2e2f1606f21bc3`  
		Last Modified: Wed, 21 Dec 2022 07:26:57 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fecd55956c02d104c50cc3da500a85684fa335fe21f677f9e09b2995b4f28a`  
		Last Modified: Wed, 21 Dec 2022 07:37:36 GMT  
		Size: 11.2 MB (11208084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114bbd5fcff10e2e7659c741aa63027c40415995e0facea416943629706a3237`  
		Last Modified: Wed, 21 Dec 2022 07:37:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b69a74fbe42d3bf7b3448597eb0a9ba6f024b4a7dda4682ad7018c0a625ec50`  
		Last Modified: Wed, 21 Dec 2022 07:37:36 GMT  
		Size: 10.7 MB (10726192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e358237a862d8ce90e6acf503af024b68b11e33c9752ce15eda5403b2cb902c`  
		Last Modified: Wed, 21 Dec 2022 07:37:34 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef5ecde69e634b0f45847a6cc239cb6e66dc24a3d35ce044bcb5e256ddb75cc`  
		Last Modified: Wed, 21 Dec 2022 07:37:34 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fc5c75ebfd5084f09d416276aa2d22e6d01f7beac724b96dffb406b85e3cfd`  
		Last Modified: Wed, 21 Dec 2022 07:37:34 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464dc07a0f236826bd382244f330109ba654ef4b1e126f7de77efe76b0416120`  
		Last Modified: Wed, 21 Dec 2022 13:47:50 GMT  
		Size: 2.2 MB (2247796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87487840465fab6060384902a9ff28a7cbe84236208aea2b24b347b3b186adfb`  
		Last Modified: Wed, 21 Dec 2022 13:47:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d08372c773e6bf3f59584b12863b0b6a9739ceffb9c084089dd190b69b7323b`  
		Last Modified: Wed, 21 Dec 2022 13:47:50 GMT  
		Size: 695.2 KB (695204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a1b23e5f44c721dfa7f4a9aeefc1ba1c7040edb7ae53feadfc62c908c5158e`  
		Last Modified: Wed, 21 Dec 2022 13:47:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0830e2d831039830f0bf91603882cdd8e60148c4eb2747e8f7a4e20fd8569993`  
		Last Modified: Wed, 21 Dec 2022 13:47:55 GMT  
		Size: 22.9 MB (22850235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:ac149279c21d19050a0871efe50655acbef2e98e826184e904c1848a8f9624c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145420453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0182e753191e2464e9c85103f789034cfce5c6d63de075bd0aea5de623c9f265`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 06 Dec 2022 00:59:27 GMT
ADD file:be297820b3c24f32c3d19e62f8aad3c9d2b37db08077869258a7d3aba92f555f in / 
# Tue, 06 Dec 2022 00:59:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:43:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 03:43:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 03:43:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 03:43:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 03:43:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 03:46:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 06 Dec 2022 03:46:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 06 Dec 2022 03:47:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 06 Dec 2022 03:47:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 06 Dec 2022 03:47:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 06 Dec 2022 03:47:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 03:47:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 03:47:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 04:34:12 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 06 Dec 2022 04:34:12 GMT
ENV PHP_VERSION=8.0.26
# Tue, 06 Dec 2022 04:34:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Tue, 06 Dec 2022 04:34:12 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Tue, 06 Dec 2022 04:34:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 04:34:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 04:36:54 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:36:54 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 04:36:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 04:36:54 GMT
STOPSIGNAL SIGWINCH
# Tue, 06 Dec 2022 04:36:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:36:55 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 04:36:55 GMT
EXPOSE 80
# Tue, 06 Dec 2022 04:36:55 GMT
CMD ["apache2-foreground"]
# Tue, 06 Dec 2022 14:24:25 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 14:24:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 06 Dec 2022 14:24:26 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Sat, 17 Dec 2022 02:24:12 GMT
ENV DRUPAL_VERSION=9.5.0
# Sat, 17 Dec 2022 02:24:12 GMT
WORKDIR /opt/drupal
# Sat, 17 Dec 2022 02:24:30 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 17 Dec 2022 02:24:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f2a5c00904a21a940a9e4ec3efaca80bebbbf2775e4c9bbe0ce9c05e967335f0`  
		Last Modified: Tue, 06 Dec 2022 01:06:56 GMT  
		Size: 22.7 MB (22748937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0fd527e893f67f85a1c13343cbede410f56ac2185449a54edd3b425543be96`  
		Last Modified: Tue, 06 Dec 2022 04:53:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac07484df679107c13570d32f6ecb607555e90ad4d72b959e42627a3f272b0e8`  
		Last Modified: Tue, 06 Dec 2022 04:53:39 GMT  
		Size: 59.5 MB (59542386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e21f2c80981b6bcaf17192519e63c71cc6376e9e11ebd6bc867f7fd4e961d0`  
		Last Modified: Tue, 06 Dec 2022 04:53:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6426e1b3ae8dc0074d6704d89e7af2a4fdb5d1c026e3bc03910e230b492bb932`  
		Last Modified: Tue, 06 Dec 2022 04:54:02 GMT  
		Size: 17.5 MB (17481393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedaeb7a61222f811004832054ecd1d55ecc2c810c5f95a36d25ea8ab3b63aef`  
		Last Modified: Tue, 06 Dec 2022 04:53:59 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e4c5ec25dbc17be63b6f6375b83a5656af1e407f05dbec39f4cf55cf8aa180`  
		Last Modified: Tue, 06 Dec 2022 04:53:59 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aeddeda89675fb48353fb79f614936f7142fb7e04756699fe63dce374921307`  
		Last Modified: Tue, 06 Dec 2022 05:02:33 GMT  
		Size: 11.2 MB (11206043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f64ae089352d46dd174930f1010255e5848fd440a0374ef0c030279fa5f6f`  
		Last Modified: Tue, 06 Dec 2022 05:02:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fa977dad2f832ce1e2c7609e87b8f945aadbc2560b8e34fa5215ba2634f64`  
		Last Modified: Tue, 06 Dec 2022 05:02:31 GMT  
		Size: 9.3 MB (9256792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d216f92cc371fc94e8c65c4a2c65d357faafa1296e32758628e472747d561`  
		Last Modified: Tue, 06 Dec 2022 05:02:29 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c509107375abb2b08e57e5a4e19807436a5277357cba40212240907241bfbc`  
		Last Modified: Tue, 06 Dec 2022 05:02:29 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5d3722d8a491263514fdf8ef2be2facc28f0cec0e099f9062e5d76c26034a6`  
		Last Modified: Tue, 06 Dec 2022 05:02:29 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ef18ae780c27389fe54f0f905dde9809c5ef5e1b806ab1b91dd7d8596301c6`  
		Last Modified: Tue, 06 Dec 2022 14:50:52 GMT  
		Size: 1.6 MB (1633088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f58a1df3584e5afe806c9f7a200dc33e69070b22bafe009d51fcb07bea8c877`  
		Last Modified: Tue, 06 Dec 2022 14:50:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa659bfae32a3efae268cc9c74ab038e430d5f0a5113f9cce3a38564b157bc2`  
		Last Modified: Tue, 06 Dec 2022 14:50:52 GMT  
		Size: 695.2 KB (695198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d47092cb5fc593a6e6e6b03f2dbb8715a47c1c3991c6e0f4fb59a70d13c72c`  
		Last Modified: Sat, 17 Dec 2022 02:52:31 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94044374677e0fea38bedd45a6315c226203e0990bb6fe5df556816c5f475a3`  
		Last Modified: Sat, 17 Dec 2022 02:52:38 GMT  
		Size: 22.9 MB (22850721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:21f4ed0f62832f79dd2daeda74daf5b86fbb6e777bcf77aad156bcd3a4cb2757
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.7 MB (161722367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f284539f5498eabd97c56488ee1c10adbe0637cf869cd0f1424b3cc64a3ac3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 11:37:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 11:37:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 11:37:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 11:37:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 11:37:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 11:40:33 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 06 Dec 2022 11:40:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 06 Dec 2022 11:40:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 06 Dec 2022 11:40:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 06 Dec 2022 11:40:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 06 Dec 2022 11:40:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 11:40:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 11:40:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 12:25:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 06 Dec 2022 12:25:09 GMT
ENV PHP_VERSION=8.0.26
# Tue, 06 Dec 2022 12:25:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Tue, 06 Dec 2022 12:25:09 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Tue, 06 Dec 2022 12:25:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 12:25:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:27:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 12:27:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:27:14 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 12:27:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 12:27:14 GMT
STOPSIGNAL SIGWINCH
# Tue, 06 Dec 2022 12:27:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:27:15 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 12:27:15 GMT
EXPOSE 80
# Tue, 06 Dec 2022 12:27:15 GMT
CMD ["apache2-foreground"]
# Tue, 06 Dec 2022 18:14:56 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 18:14:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 06 Dec 2022 18:14:57 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Fri, 16 Dec 2022 23:52:22 GMT
ENV DRUPAL_VERSION=9.5.0
# Fri, 16 Dec 2022 23:52:22 GMT
WORKDIR /opt/drupal
# Fri, 16 Dec 2022 23:52:51 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 16 Dec 2022 23:52:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcfb88424deadf3813dacd34bdd5c43e0efbd63081ff1150e5dec324b5cb9ca`  
		Last Modified: Tue, 06 Dec 2022 12:36:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe65ddacb555d1b9f51638b7e3ba1d5bb8acc73fbb6c25384b75e2be98e18d5`  
		Last Modified: Tue, 06 Dec 2022 12:36:18 GMT  
		Size: 70.4 MB (70362880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fa4c2f5fe9157eb2e01d87095eef0519b1db09108d017084f6446fff830a5a`  
		Last Modified: Tue, 06 Dec 2022 12:36:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fb17e1902a12541964d328ffbd818597a447c3dad5401122d30cbbe4f21ed9`  
		Last Modified: Tue, 06 Dec 2022 12:36:35 GMT  
		Size: 18.6 MB (18583978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2faaa2f977fa2552852fd7399b80207db3e069cbf8b0d3f1abb2aeb70e9843b`  
		Last Modified: Tue, 06 Dec 2022 12:36:33 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899e7f56be7b5447675b077c77b40db71fe57dbfd32740a7953fd36e77ac8913`  
		Last Modified: Tue, 06 Dec 2022 12:36:33 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e299b38af431f2af55293796def0392017417cf41cd1e8afe9cb95a83f871f`  
		Last Modified: Tue, 06 Dec 2022 12:42:15 GMT  
		Size: 11.2 MB (11206852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07870aca9ed67b4a776ef012932b7522a0c1a09128daf7999ed9e81308e0d61`  
		Last Modified: Tue, 06 Dec 2022 12:42:13 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7cb79f4b34e6b4ce85ca8af829d3fbf3dce864e7ffcc9511f5d131ff75019`  
		Last Modified: Tue, 06 Dec 2022 12:42:15 GMT  
		Size: 10.2 MB (10201436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3841749f9c3073bf57ed03dc1f03c2df705f2a6250b32caa3afbd9041ee9f3b6`  
		Last Modified: Tue, 06 Dec 2022 12:42:13 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4fc960acad5c3ddd2b95f9b4a48f6e27cbdd7e3f5093a9136cda9361fd36b1`  
		Last Modified: Tue, 06 Dec 2022 12:42:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc896b645fc3e5f671ccba7f4a7c3798dfa6efcb60c60ff2bc186c752101d385`  
		Last Modified: Tue, 06 Dec 2022 12:42:13 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a36854c50512c72f98fdeb8e83feca5ad1c16a6a88e76b0c62102de469b4eea`  
		Last Modified: Tue, 06 Dec 2022 18:30:19 GMT  
		Size: 1.9 MB (1900213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472bbf6c855b8ac65a47f70ec5587847b5470186e4c381426777c941f13200c5`  
		Last Modified: Tue, 06 Dec 2022 18:30:19 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a88dd152f9c5f8bd88d0bc0b1818f93fdb43748ae068ea79086216468aa97f`  
		Last Modified: Tue, 06 Dec 2022 18:30:19 GMT  
		Size: 695.2 KB (695200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab758c63999bdcd0a4e9671960427baecd080ba3be876dc51abea4f9610a7a91`  
		Last Modified: Sat, 17 Dec 2022 00:07:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b69a53f16532589d35a7bfac958ec5be449550ba3b173438128fde29fc17958`  
		Last Modified: Sat, 17 Dec 2022 00:07:42 GMT  
		Size: 22.9 MB (22850821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:c59120a6042a171e2cc75e003eb1ea292ad9b189c16b31420eb778c7b5d05244
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.5 MB (175521742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85b649dffbf0238d478617878e1c19a4c686cc512b239aff5a32d944a585f1f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:45 GMT
ADD file:48a2a0e6cb166df412bb4f6ad30537c66bc6be97ce4c8fc582fd5ac8c6129b5a in / 
# Wed, 21 Dec 2022 01:39:46 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:52:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 02:52:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 02:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:52:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 02:52:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 02:56:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 02:56:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 02:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 02:56:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 02:56:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 02:56:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 02:56:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 02:56:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 04:36:40 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 21 Dec 2022 04:36:40 GMT
ENV PHP_VERSION=8.0.26
# Wed, 21 Dec 2022 04:36:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.26.tar.xz.asc
# Wed, 21 Dec 2022 04:36:42 GMT
ENV PHP_SHA256=0765bfbe640dba37ccc36d2bc7c7b7ba3d2c3381c9cd4305f66eca83e82a40b3
# Wed, 21 Dec 2022 04:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 04:36:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:39:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 04:39:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:39:30 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 04:39:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 04:39:31 GMT
STOPSIGNAL SIGWINCH
# Wed, 21 Dec 2022 04:39:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:39:33 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 04:39:34 GMT
EXPOSE 80
# Wed, 21 Dec 2022 04:39:35 GMT
CMD ["apache2-foreground"]
# Wed, 21 Dec 2022 15:28:45 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 15:28:46 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 15:28:48 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Wed, 21 Dec 2022 15:28:48 GMT
ENV DRUPAL_VERSION=9.5.0
# Wed, 21 Dec 2022 15:28:49 GMT
WORKDIR /opt/drupal
# Wed, 21 Dec 2022 15:29:02 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 21 Dec 2022 15:29:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9099d8a02dc0a7901931d2811fa3078b18ecd3a40a156cbcfd91629126463f80`  
		Last Modified: Wed, 21 Dec 2022 01:45:34 GMT  
		Size: 27.8 MB (27798412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059e8367727edb1fc1a41e9b0f8ad5b0608020745ccabd6b8d52e53026bd118c`  
		Last Modified: Wed, 21 Dec 2022 04:56:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8ad3db0ab49efd6bd406a7d3ad6840dbb73a96a726765be6e3a8850335c2a6`  
		Last Modified: Wed, 21 Dec 2022 04:57:11 GMT  
		Size: 81.2 MB (81234660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d0ba56dcb1911150c21614d7e7a92926708de4a7f09f08247c3d90328b56f5`  
		Last Modified: Wed, 21 Dec 2022 04:56:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536877caf92b1b7ac69f2c2d84e14f87f2646d80052e877d9e458f64c563425`  
		Last Modified: Wed, 21 Dec 2022 04:57:41 GMT  
		Size: 18.9 MB (18900816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a64f24e01d83808b6a5b80fedb86fd9df898ab2b45512f5fc1609e1711faf9`  
		Last Modified: Wed, 21 Dec 2022 04:57:38 GMT  
		Size: 426.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e068cec5c0ab47f8a2059829fbe559e03b130c176e6cfdb86af792ccab4def0e`  
		Last Modified: Wed, 21 Dec 2022 04:57:38 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924aed964b4600d6e99ecc173da1df7a9d1e565f26e5c22338712afe8b5aeb77`  
		Last Modified: Wed, 21 Dec 2022 05:11:02 GMT  
		Size: 11.0 MB (10993430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5793ac9a52b0344314fbadaa3da103e94439683efaa7ada396e91ae80b6f4fe8`  
		Last Modified: Wed, 21 Dec 2022 05:10:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3869f74f913b340db0a158586fd1ebe155dfab3e7c89040aee25ccb498470`  
		Last Modified: Wed, 21 Dec 2022 05:11:01 GMT  
		Size: 10.9 MB (10936942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765d257dd622efad43377c0ee743669f77e97a4a3b5dcc175c4c32409fa44f6f`  
		Last Modified: Wed, 21 Dec 2022 05:10:59 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bee00b43a9da361381ee4c9ba62e1e749c55990975e38f77bce35e47e9734c9`  
		Last Modified: Wed, 21 Dec 2022 05:10:59 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a10b66268e46f4b9b45f1c080f9e5d7aa3a7527a3c5c70ef6b0ec1f07d5d3c`  
		Last Modified: Wed, 21 Dec 2022 05:10:59 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e84bfcb6955532de8cd074b4fac53004faae2178fac24ffc8cc369bd2cd61b6`  
		Last Modified: Wed, 21 Dec 2022 15:53:30 GMT  
		Size: 2.1 MB (2102385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182ad2dcd957237b2e8b0586dd417cdc0d8f65a8191f859149390a98a78622e`  
		Last Modified: Wed, 21 Dec 2022 15:53:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036fe90f166454a456fdabefdf7e76d75497e354c08a0817eb0aa42e86e662d`  
		Last Modified: Wed, 21 Dec 2022 15:53:30 GMT  
		Size: 695.2 KB (695198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6a20fd5046acbd9edebc6499945b394b27533fc1dca32f4a2de4a36197cdcd`  
		Last Modified: Wed, 21 Dec 2022 15:53:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57584696186d6460952d15edee01d56c5c0a3b2ae61b27996af3dde93d0702f8`  
		Last Modified: Wed, 21 Dec 2022 15:53:35 GMT  
		Size: 22.9 MB (22853998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
