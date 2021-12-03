## `drupal:7-php7.4-apache-buster`

```console
$ docker pull drupal@sha256:10b1aeb88ade9c50cc765bc4838b716329b2ffd0452a3c74a940a707ef21e53e
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

### `drupal:7-php7.4-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:b5958df5d9218072cb1275f71f130dd314e5e200a0c30e79969daffacb4efbc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152190289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6897cce0b014cb4152111e35ba739a244b336ddc49ff6f479412908224d375d0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:39:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 12:39:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 12:39:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:39:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 12:39:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:48:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 12:48:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 12:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 12:49:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 12:49:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 12:49:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:49:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:49:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 14:38:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 14:38:19 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 14:38:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 14:38:20 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 14:38:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 14:38:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:41:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 14:41:48 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:41:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 14:41:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 14:41:49 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 14:41:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:41:50 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 14:41:50 GMT
EXPOSE 80
# Thu, 02 Dec 2021 14:41:50 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 17:49:33 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 17:49:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 17:55:16 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 17:55:16 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 17:55:17 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13522578ad9c68f9a771d9dfc2a14315b97c7ee6690853b02cd9c261046d8b7`  
		Last Modified: Thu, 02 Dec 2021 15:31:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027e794f2380b6fb5275c0b6c78e9cbcc29821b043c51ad81ca54eb46a801a7`  
		Last Modified: Thu, 02 Dec 2021 15:32:07 GMT  
		Size: 76.7 MB (76681131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003069fe633e007e207bfc0b2084e0d3b19cabd7d7a308367946cd858fabcc6`  
		Last Modified: Thu, 02 Dec 2021 15:31:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afca0c798a59b50622df9aaad0dd407f7c7b9f77999cab832f70bffd3c8c63f`  
		Last Modified: Thu, 02 Dec 2021 15:32:39 GMT  
		Size: 18.7 MB (18679888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904a0292174da3a627c8e999351f8879c6bfabde14163b2ae51607d0c1120cf4`  
		Last Modified: Thu, 02 Dec 2021 15:32:36 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878e74c8c6b5ff2fd3739f532749ac8b45aa996736e2a2f27dcc66594406245`  
		Last Modified: Thu, 02 Dec 2021 15:32:36 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cabc759585527d8170ded333679a336272d34fe3d3639eb81fcd4afd554b4b`  
		Last Modified: Thu, 02 Dec 2021 15:39:30 GMT  
		Size: 10.8 MB (10757890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0f355ff269fbd8a5e68547368f185309f10ad76ff5843b48089b90f8e9efe`  
		Last Modified: Thu, 02 Dec 2021 15:39:26 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91875635f69d9961c1b3203c1ca80ec03b0ccab3a7bbe16e763a0636ea3cc45c`  
		Last Modified: Thu, 02 Dec 2021 15:39:31 GMT  
		Size: 13.9 MB (13859309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a864f6e4c8d1d717410a06ce2df7968ce243151f41c31b276de9c37b9c903a0`  
		Last Modified: Thu, 02 Dec 2021 15:39:27 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3347b8f8a6bb3d71e9dcd56712406b0cc244cb8d3f6d6f29b2d057cb12e16071`  
		Last Modified: Thu, 02 Dec 2021 15:39:27 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda0ea55460bc42da178ec0cbd19648bfbcb6afefa33e274869edb8ab135f43e`  
		Last Modified: Thu, 02 Dec 2021 15:39:26 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e4d5a96c201dd17583317a1b4f8cd10685884e114ef2a57abd93a0f94603ec`  
		Last Modified: Fri, 03 Dec 2021 18:04:37 GMT  
		Size: 1.7 MB (1672421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423de59485f98f6533afb9ea9c315a175d249ad61d545cdede0c3aab8156ce4e`  
		Last Modified: Fri, 03 Dec 2021 18:04:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c075d4018318d8c1fbbae8f87f79fc92be38f45b490dbb089af1f85a7480121`  
		Last Modified: Fri, 03 Dec 2021 18:12:05 GMT  
		Size: 3.4 MB (3380165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; arm variant v5

```console
$ docker pull drupal@sha256:d5453c6600cb645a58a71d2098dab082b2141327fdb3eeaddd6114a48f7c0b7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130353200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05b0d437f8271ecb3b80e8297108dd3c7365482f53bcb1613a72bbcf718dc0f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:44 GMT
ADD file:b509d9889433e2e1b4e7d30f6a1461c93f9c6a2a6f60e1802710cbc20e7a0e81 in / 
# Thu, 02 Dec 2021 02:51:46 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:37:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:37:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:38:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:38:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:38:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 01:44:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 01:44:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 01:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 01:45:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 01:45:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 01:45:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:45:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:45:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 03:12:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 03 Dec 2021 03:12:17 GMT
ENV PHP_VERSION=7.4.26
# Fri, 03 Dec 2021 03:12:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 03 Dec 2021 03:12:17 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 03 Dec 2021 03:12:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Dec 2021 03:12:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:17:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Dec 2021 03:17:13 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:17:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Dec 2021 03:17:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Dec 2021 03:17:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Dec 2021 03:17:16 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:17:16 GMT
WORKDIR /var/www/html
# Fri, 03 Dec 2021 03:17:16 GMT
EXPOSE 80
# Fri, 03 Dec 2021 03:17:17 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 10:50:49 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 10:50:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 10:50:51 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 10:50:51 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 10:50:55 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:6f8ed9eedee034be125ab31b8087fb60cf54bd4085e7e2dfbdc92ccae717fa06`  
		Last Modified: Thu, 02 Dec 2021 03:10:47 GMT  
		Size: 24.9 MB (24886215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da19821865bed5dd99ba944546eaafa4b0f2ba27b3c69169c67df37f85f522`  
		Last Modified: Fri, 03 Dec 2021 04:26:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f55ae21508192d706388fdfa217fd9efb8b10e2d827eaff2a13f0f149fcd14`  
		Last Modified: Fri, 03 Dec 2021 04:27:18 GMT  
		Size: 58.8 MB (58821006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a324e5a2c1bcbfd7c7a0130e62fba6afdea47bda0adb7d1ccd16baf92c541af`  
		Last Modified: Fri, 03 Dec 2021 04:26:38 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727ece955d38c5ed3aeece3b3b3c24c1fe36ea47acf4c888e4139608e67847d7`  
		Last Modified: Fri, 03 Dec 2021 04:28:07 GMT  
		Size: 18.0 MB (18026219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214010fb8fd2426950a23db0664eee54cff5ea814c5bd3132efa101f228a22f`  
		Last Modified: Fri, 03 Dec 2021 04:27:57 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3652966453573cda3158ef4f4afd163843bd5b43e9c260948f756e5dfe54ca7`  
		Last Modified: Fri, 03 Dec 2021 04:27:57 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875640a8abeca58362cf76410140149ac4b0a5e3ef73fe3b729bb282fe02e009`  
		Last Modified: Fri, 03 Dec 2021 04:38:52 GMT  
		Size: 10.8 MB (10756076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5820d9c90400e0545020fe99c735d077a4c0db6f21bf0e1424085b47d159a89f`  
		Last Modified: Fri, 03 Dec 2021 04:38:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bc2ec07254349e21440c726ce3c1d6ec00b13a682f454f120f71bade982df6`  
		Last Modified: Fri, 03 Dec 2021 04:38:57 GMT  
		Size: 12.9 MB (12920671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f3bcaaf25ab1771d643d870442b3d209fdbe0e2810c305f6111dbf5ae132e9`  
		Last Modified: Fri, 03 Dec 2021 04:38:47 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1692ae2083f333d2d0b00d3692008ca0b82148bccff20ee6f4983543f222aae8`  
		Last Modified: Fri, 03 Dec 2021 04:38:47 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bedbff8cc4b48b1c1f281e383b06b4f108f8fd7e4c8cd11b353f63c4501af8`  
		Last Modified: Fri, 03 Dec 2021 04:38:47 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f903b993461c76a10c56fd0be82b40804210f1998a717ccad0439bd531251c`  
		Last Modified: Fri, 03 Dec 2021 10:57:09 GMT  
		Size: 1.6 MB (1557072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8891c55af2783df96d9cf283e96512218284dde8690f14f77c2db2e7e0bc5d`  
		Last Modified: Fri, 03 Dec 2021 10:57:07 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4344dc01e7f1d41d9265f26690efa3b595e6017886239aa56397cfa70aead`  
		Last Modified: Fri, 03 Dec 2021 10:57:11 GMT  
		Size: 3.4 MB (3380167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:b9513034fe69783c383d05713ea5bd59e3d86239159a08989b138fc0c4586468
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127539032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddffbcb6b91de576152c95ac59affba3d2a82f723de99b5fb9d0f6ce938abe05`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:46 GMT
ADD file:4ac0de0d740f0c221cd4f912861a67009942fa5bdad24ac8b62c690dfa15024a in / 
# Wed, 17 Nov 2021 02:00:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:53:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 17 Nov 2021 14:53:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 17 Nov 2021 14:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:54:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Nov 2021 14:54:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Nov 2021 14:59:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 17 Nov 2021 14:59:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 17 Nov 2021 15:00:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 17 Nov 2021 15:00:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 17 Nov 2021 15:00:07 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 17 Nov 2021 15:00:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 15:00:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 15:00:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Nov 2021 16:19:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 17:20:00 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 17:20:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 17:20:01 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 17:20:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 18 Nov 2021 17:20:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:24:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:24:25 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:24:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:24:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:24:27 GMT
STOPSIGNAL SIGWINCH
# Thu, 18 Nov 2021 17:24:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:24:28 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:24:29 GMT
EXPOSE 80
# Thu, 18 Nov 2021 17:24:29 GMT
CMD ["apache2-foreground"]
# Fri, 19 Nov 2021 02:59:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Nov 2021 02:59:11 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 19 Nov 2021 03:17:44 GMT
ENV DRUPAL_VERSION=7.82
# Fri, 19 Nov 2021 03:17:44 GMT
ENV DRUPAL_MD5=51f8515161087935662b9835194a779b
# Fri, 19 Nov 2021 03:17:48 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:7bd9e64406c6f3044bd15f89c367f07ec4eaafb1035a5c3ee2f7b138be68017f`  
		Last Modified: Wed, 17 Nov 2021 02:16:39 GMT  
		Size: 22.8 MB (22754359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c4874d32ab574ccc33a379e317815780f747a38327c0c40f837b621ae089ac`  
		Last Modified: Wed, 17 Nov 2021 17:39:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadea33f39c706340283c3b97966190fa5fb372681381ef59297cb0276bb6d0d`  
		Last Modified: Wed, 17 Nov 2021 17:39:58 GMT  
		Size: 59.5 MB (59514745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db17542520a059bcd73f00bc89ec3d839b41fc55e649fd74b0fb46caf26ac625`  
		Last Modified: Wed, 17 Nov 2021 17:39:21 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614855b53f736d40b93dcd96a818fdc472467d35f60a37af4f107f6ed1c7520`  
		Last Modified: Wed, 17 Nov 2021 17:40:33 GMT  
		Size: 17.5 MB (17481397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3917ae947106b359ba488056a7ec049781bf40003d257ade2a5bc8658214505f`  
		Last Modified: Wed, 17 Nov 2021 17:40:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1723f5587d855c5b7a53c4717c4edddc175713e9c752c88c11240c4c8176f8`  
		Last Modified: Wed, 17 Nov 2021 17:40:24 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82568c6a1894b71bd6dccd39bfb10ab4c702909a584c56c920344ddbf40f9142`  
		Last Modified: Thu, 18 Nov 2021 19:37:41 GMT  
		Size: 10.8 MB (10756094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb4ec6e010d101f666033578982bf3d180bc1f765608ca52d87845010381fbc`  
		Last Modified: Thu, 18 Nov 2021 19:37:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7a450d8a0206a3afee53c3466aaa30d93572479c002b987255be6e7f61e43`  
		Last Modified: Thu, 18 Nov 2021 19:37:44 GMT  
		Size: 12.2 MB (12216378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333cd6209fdbf782f7dcd285683e95224d7b70bd2f96b6f7a76251b6ec3bb9a3`  
		Last Modified: Thu, 18 Nov 2021 19:37:36 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1587884c9b151e579513743b690263a5701f337b5c42cde302f53f93afd5ab1b`  
		Last Modified: Thu, 18 Nov 2021 19:37:36 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cd9e57e2b2cc2a3877c76d60b0280741bc91a030fa0ec101f32107e1e0cfd1`  
		Last Modified: Thu, 18 Nov 2021 19:37:36 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc57b28ca6719240eb2df14ba144999940a7ea71853674cb1fee57c09e5009b`  
		Last Modified: Fri, 19 Nov 2021 03:40:00 GMT  
		Size: 1.4 MB (1436588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cdeefe288941694759cc140268d845d4d2ac5fd3cab594b782997a6ab7aa0b`  
		Last Modified: Fri, 19 Nov 2021 03:39:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9308eb289a38a06f36f8d6870dacc7e2ef5c957d79b57bcb9be8476edcbb8ffd`  
		Last Modified: Fri, 19 Nov 2021 03:54:59 GMT  
		Size: 3.4 MB (3373707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:bcc21967b98e26169aa1c4e75da49cccb7db04894091d123dc561adfbf4cb01a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143649212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926738d712f6c4306526f23210f389eaa3ccdb0a25b2ac187f17e574d08da1c7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:16:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 12:16:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 12:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:17:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 12:17:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:21:33 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 12:21:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 12:21:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 12:21:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 12:21:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 12:21:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:21:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:21:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 13:10:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 13:10:50 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 13:10:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 13:10:52 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 13:11:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 13:11:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:13:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 13:13:05 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:13:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 13:13:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 13:13:07 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 13:13:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:13:09 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 13:13:10 GMT
EXPOSE 80
# Thu, 02 Dec 2021 13:13:11 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 12:16:59 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:17:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 12:27:20 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 12:27:21 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 12:27:23 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ea36970a3274ea258179497650464be3c09114dead10e1173e1a0f70916094`  
		Last Modified: Thu, 02 Dec 2021 13:49:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23015b38ce0d43ba0bc4564527399f28eeca0609957c7c5205008cee218e28a6`  
		Last Modified: Thu, 02 Dec 2021 13:49:54 GMT  
		Size: 70.4 MB (70359445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341100e2e27f907458e84d00b03ca15c5c4d256ea7e1bce71dfb0ff6e958ecd9`  
		Last Modified: Thu, 02 Dec 2021 13:49:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd5cde5c1891715285232fcbc925915573238e56a064bdb227126f5d42b41e9`  
		Last Modified: Thu, 02 Dec 2021 13:50:31 GMT  
		Size: 18.4 MB (18365315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7fd00581298f35ba586aa591fce16b1569c9cd517a41867ff4ad746389cc2`  
		Last Modified: Thu, 02 Dec 2021 13:50:28 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c574d44d00ff90bffaccf45957b8e3e056b5a9c673dc86503055dc357d75a4f`  
		Last Modified: Thu, 02 Dec 2021 13:50:28 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd98c57c99863a7901e2aa896c9bdac19a8f6391b063f1d1378429885ee38c`  
		Last Modified: Thu, 02 Dec 2021 13:57:47 GMT  
		Size: 10.5 MB (10544717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f6d4b47e42db9c5272f6b43a6e96b20961ad8b38ae4f6d6351e5ddb162ea8`  
		Last Modified: Thu, 02 Dec 2021 13:57:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe25c88dfe11177bd1f5659567b8ade4485b01fdae793359a570f4ec658cff6`  
		Last Modified: Thu, 02 Dec 2021 13:57:45 GMT  
		Size: 13.6 MB (13621575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2687033b810a5fffa6bb5b8b9f77a18b96c8f5e79d8814ff145d93ee2f077041`  
		Last Modified: Thu, 02 Dec 2021 13:57:43 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b3c519aade3d9c88daac875afcede90ac70b7a83d4e0422c204b6745d64df`  
		Last Modified: Thu, 02 Dec 2021 13:57:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0673f750e0dcb8116c4b50ca7c91c9b0c2495a2457ace6b15bd10a6c7a7685ae`  
		Last Modified: Thu, 02 Dec 2021 13:57:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359a4eefbd92c2de44034307a05ef59b50cd1d8d66cfadf12fd6e5af6ac55b11`  
		Last Modified: Fri, 03 Dec 2021 12:41:08 GMT  
		Size: 1.4 MB (1449330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5754bb1a6196ae786bf79bff9d1c7849d88d74bf74725ffc2e9f1e220043bc3`  
		Last Modified: Fri, 03 Dec 2021 12:41:07 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1e2601c7b7b500366d0ad71c9e29b93ff8d5df9b2ec8c2a6c86c9156fd6f3`  
		Last Modified: Fri, 03 Dec 2021 12:58:41 GMT  
		Size: 3.4 MB (3380054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:bab2f77011e902aeb4943fad3a049d29161bf8635afa4611a83d374f13870931
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158216882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a87f8dbd117caac1c2121c00621a4bce898ff83fca07a7694334553291d0ee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:00:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 16:00:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 16:01:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:01:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 16:01:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 16:07:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 16:07:39 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 16:07:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 16:07:51 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 16:07:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 16:07:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 16:07:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 16:07:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 17:58:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 17:58:13 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 17:58:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 17:58:13 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 17:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 17:58:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 18:02:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 18:02:29 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 18:02:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 18:02:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 18:02:33 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 18:02:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 18:02:34 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 18:02:34 GMT
EXPOSE 80
# Thu, 02 Dec 2021 18:02:35 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 07:31:25 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 07:31:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 07:45:13 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 07:45:13 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 07:45:16 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3bec8390a3fb9cacde110dff928f03c6bfbf4c67380782be7bc2ec468bad44`  
		Last Modified: Thu, 02 Dec 2021 19:05:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374e03f2cbaf2599705aba5989e4c2f0610646764f4b510df4d65fd56cdb13bb`  
		Last Modified: Thu, 02 Dec 2021 19:06:06 GMT  
		Size: 81.2 MB (81229810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8020b07a62641f451efc11a0c44d8280cb3c444a9a40c5d31cd6d56577eed4e4`  
		Last Modified: Thu, 02 Dec 2021 19:05:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc50bd197e40c6a692d5a12ba8a0279fd6b51a7fc071f33586d65a7480d3137c`  
		Last Modified: Thu, 02 Dec 2021 19:06:47 GMT  
		Size: 19.1 MB (19115011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f193a6fc508aff5a482a5347b34c22a1d61319180c7deff56bc670e778e06`  
		Last Modified: Thu, 02 Dec 2021 19:06:42 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0be64ba44e16f1f571c2fd5b22528316c119edda07ef07afe45fa177cfe60bc`  
		Last Modified: Thu, 02 Dec 2021 19:06:42 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ad18ed15b9f0657055c4535426a1a044fb8d5a03cc5938724ceaa12313a098`  
		Last Modified: Thu, 02 Dec 2021 19:15:59 GMT  
		Size: 10.8 MB (10757150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e05a7b09be71be1a52081a4c804d1c69a24e7a19fc274594e54a259a269d65`  
		Last Modified: Thu, 02 Dec 2021 19:15:54 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9d8703c6404b05eeaa38f20aca005daff89480a4107ce64db0f78bf2601fd0`  
		Last Modified: Thu, 02 Dec 2021 19:16:04 GMT  
		Size: 14.2 MB (14175392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c1985e9b075567281284b27939f410fe777870de234c8577f6b2cba88bc0f1`  
		Last Modified: Thu, 02 Dec 2021 19:15:54 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed7f639324438fde6552d01a0b96e983bd6647f00824f7e396683fd944db40d`  
		Last Modified: Thu, 02 Dec 2021 19:15:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de946aa74cf7047300bd5229ac997941f6b8e251f79ccb6d41ac650b59e8cb3c`  
		Last Modified: Thu, 02 Dec 2021 19:15:54 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2411913076b84c8c7151cdd5915c27aef974777e34b7f4ed76e0519c85dd5ea`  
		Last Modified: Fri, 03 Dec 2021 08:09:08 GMT  
		Size: 1.7 MB (1749042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac3ada60dcf0abaa7ca9092629ceab2c9c80c815c9ea09a022a9d818bafc6ed`  
		Last Modified: Fri, 03 Dec 2021 08:09:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874bbe19096d163ef002ccca77f7e597a753b18efbd08a879a8c5598fc664186`  
		Last Modified: Fri, 03 Dec 2021 08:21:58 GMT  
		Size: 3.4 MB (3380168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; mips64le

```console
$ docker pull drupal@sha256:3d30ccddf1a1677ea0694a1cc8d50f4851fc92a3b51f4f3d885b95db8300201e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134789744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cca16211ca06f428f64dc58650227897232dc08c0c8bbb468c17136dfb7211f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 17 Nov 2021 02:11:05 GMT
ADD file:442e2528f8dc5583975e61c403642ead88c26af80e5769940d11d2420eb6e56d in / 
# Wed, 17 Nov 2021 02:11:06 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:24:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 17 Nov 2021 10:24:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 17 Nov 2021 10:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:25:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Nov 2021 10:25:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Nov 2021 10:39:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 17 Nov 2021 10:39:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 17 Nov 2021 10:39:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 17 Nov 2021 10:39:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 17 Nov 2021 10:39:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 17 Nov 2021 10:39:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 10:39:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 10:39:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Nov 2021 13:48:15 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 19 Nov 2021 02:26:43 GMT
ENV PHP_VERSION=7.4.26
# Fri, 19 Nov 2021 02:26:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 19 Nov 2021 02:26:44 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 19 Nov 2021 02:27:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 19 Nov 2021 02:27:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 02:35:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 02:35:07 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 19 Nov 2021 02:35:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 02:35:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 02:35:09 GMT
STOPSIGNAL SIGWINCH
# Fri, 19 Nov 2021 02:35:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 19 Nov 2021 02:35:10 GMT
WORKDIR /var/www/html
# Fri, 19 Nov 2021 02:35:10 GMT
EXPOSE 80
# Fri, 19 Nov 2021 02:35:11 GMT
CMD ["apache2-foreground"]
# Fri, 19 Nov 2021 04:32:21 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Nov 2021 04:32:23 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 19 Nov 2021 04:32:23 GMT
ENV DRUPAL_VERSION=7.82
# Fri, 19 Nov 2021 04:32:24 GMT
ENV DRUPAL_MD5=51f8515161087935662b9835194a779b
# Fri, 19 Nov 2021 04:32:28 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:f95d3989b23de40aa9c78765869cf0e26ca2ed018dd048613fbc1f9df33d1bc1`  
		Last Modified: Wed, 17 Nov 2021 02:20:33 GMT  
		Size: 25.8 MB (25820129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ccdad319f1ac5bf0499b216dc0efd81717da51a949c3793cdad5ad3548166f`  
		Last Modified: Wed, 17 Nov 2021 15:42:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c0ca38354522a91f8e668cf8f3a9db99b50b9ad536617bb87bfc3d333b1c21`  
		Last Modified: Wed, 17 Nov 2021 15:43:30 GMT  
		Size: 61.4 MB (61403794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec16f6778008526a5a731bdb80797d1c4ea39425f31dbc631279933f2b4ced1`  
		Last Modified: Wed, 17 Nov 2021 15:42:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136ede21f222764292e63a724f8f7fc571ab068ec7741e7303589ad398398664`  
		Last Modified: Wed, 17 Nov 2021 15:44:03 GMT  
		Size: 18.6 MB (18612253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68829e797f0962dca1e3dd91add86600c4c9d7e93a8711f4c53de6a451137267`  
		Last Modified: Wed, 17 Nov 2021 15:43:50 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca69c6e42090df070412f36f9cb7d563c3c2fb866d3ed2eaaeb01a736be50d2`  
		Last Modified: Wed, 17 Nov 2021 15:43:50 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56146718a32eaa58fbf71ed2de318f58d01525243fe7e2d458d16b7eab6427`  
		Last Modified: Fri, 19 Nov 2021 04:21:34 GMT  
		Size: 10.8 MB (10755499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419ee9812ecdf554c578a600140b1a6c46dfae2f4308f89aa5afad255723ad8f`  
		Last Modified: Fri, 19 Nov 2021 04:21:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a959ed0fc8fb01e138098efe9f3add260ff52a00d64f4d43ce308fbf8ce942`  
		Last Modified: Fri, 19 Nov 2021 04:21:39 GMT  
		Size: 13.2 MB (13157801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63772de30c6818a5431f70825be5983e2959910b21b908f01ab47656b1fce117`  
		Last Modified: Fri, 19 Nov 2021 04:21:28 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a722d0110683388c1b2abee691fc0586fb6415689632b0555ac5056b9b7d4042`  
		Last Modified: Fri, 19 Nov 2021 04:21:28 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b6de1b7b21707d6a00d30a9b49f71f8a35eecf72d1970d168dc5ff78846c5e`  
		Last Modified: Fri, 19 Nov 2021 04:21:28 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79a87ab1dd6b8fc1fd116a2f6fee9064830014221edc8323bfef96abc70636f`  
		Last Modified: Fri, 19 Nov 2021 04:35:23 GMT  
		Size: 1.7 MB (1661149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a48f1880bad19e6f2b5e2811de1e7f5c97b27f2d6ed54dabf7ae81eb3f7bea`  
		Last Modified: Fri, 19 Nov 2021 04:35:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8630309a1de53dc035fcb731262d5155b8371846e9dd9852428c7b8185db9ee`  
		Last Modified: Fri, 19 Nov 2021 04:35:25 GMT  
		Size: 3.4 MB (3373465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:ccfc96746d86ff63234c7615130c04d2a5f16f9aac6d3e8d6908829e8bd4a44d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163590371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2088602d8d048f08faf9521411070100bd9d022f2d81c0853592e243f30a1d2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:12 GMT
ADD file:b9b5697bc2dd3ded7a158d973abc939cc5d197f1f0d9ff1fa8b3db3b7906de7a in / 
# Thu, 02 Dec 2021 07:22:18 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:53:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:53:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:54:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:55:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 02:00:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 02:00:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 02:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 02:01:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 02:01:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 02:01:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 02:02:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 02:02:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 03:27:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 03 Dec 2021 03:27:59 GMT
ENV PHP_VERSION=7.4.26
# Fri, 03 Dec 2021 03:28:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 03 Dec 2021 03:28:05 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 03 Dec 2021 03:28:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Dec 2021 03:29:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:33:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Dec 2021 03:33:27 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:33:32 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Dec 2021 03:33:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Dec 2021 03:33:36 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Dec 2021 03:33:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:33:41 GMT
WORKDIR /var/www/html
# Fri, 03 Dec 2021 03:33:43 GMT
EXPOSE 80
# Fri, 03 Dec 2021 03:33:47 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 16:31:50 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 16:31:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 16:47:00 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 16:47:01 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 16:47:07 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:da5263f5d65ecaf2dcd9400908302b4c477c13afa707110e4d85b4b946e9a3ae`  
		Last Modified: Thu, 02 Dec 2021 07:32:41 GMT  
		Size: 30.6 MB (30562306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8f6c7bf36c9a359b779def1339d11fe1d9c1422d6a518b6431c941f70bb683`  
		Last Modified: Fri, 03 Dec 2021 04:38:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3507a81e5d8123871a651605ea2edc67d3b3faaa82eb682639d539c385e14e0a`  
		Last Modified: Fri, 03 Dec 2021 04:39:34 GMT  
		Size: 82.3 MB (82291748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ec8b19b49c5228741833ff588ab20a7146158440b5a7ff46d9b99b10a861ae`  
		Last Modified: Fri, 03 Dec 2021 04:38:58 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0787cb2a8b4cfc3740ad1d60792d898ed2c569959406198414518ef15aedf45`  
		Last Modified: Fri, 03 Dec 2021 04:40:18 GMT  
		Size: 19.8 MB (19818258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea12444160c73138213201471db8e68e0a794f6118c6ef3dae7ab11254f687b`  
		Last Modified: Fri, 03 Dec 2021 04:40:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcfee3895ba69f663982e7954ebbe2ae0a45697a9e48e203df759a5ec5cb998`  
		Last Modified: Fri, 03 Dec 2021 04:40:13 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135aacc48569a180fb3fde4110eedcebbe8d77b9f0a4565c4498b82a4103ebe6`  
		Last Modified: Fri, 03 Dec 2021 04:48:14 GMT  
		Size: 10.8 MB (10757538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25a63de9a16df88f8e7f214c51d72723b90fc979f38d07586e89619fa7af3d8`  
		Last Modified: Fri, 03 Dec 2021 04:48:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9395c86b7946aef5a69c95d97d1f28b436ebfe605bc8e388f3afa8a6fa539678`  
		Last Modified: Fri, 03 Dec 2021 04:48:13 GMT  
		Size: 14.9 MB (14871608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c675f53aa4f4e490e3fedcad4f24f505f080cb45341af0024d29973aea47935`  
		Last Modified: Fri, 03 Dec 2021 04:48:10 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570cc65d4639c980a331f0bdd9f014d0ed6e41599acb93f819db29061092106a`  
		Last Modified: Fri, 03 Dec 2021 04:48:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364cdc7324c69c6adcf410c6ae79c2524b714673f5d4814a798ccd091fdf3a5c`  
		Last Modified: Fri, 03 Dec 2021 04:48:10 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd98539f11e31067469a5bb5c0261fa535316364c3cdec54f9109bb78bd7a9`  
		Last Modified: Fri, 03 Dec 2021 17:08:32 GMT  
		Size: 1.9 MB (1902968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da41e553a76b2c2568bea91342567daec7379af3cc60bbd9d8a6bbf9317412f`  
		Last Modified: Fri, 03 Dec 2021 17:08:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753f652190291bf11ef3907eea2b49a53e4227fbcd7b162e49d6333ea52adcd1`  
		Last Modified: Fri, 03 Dec 2021 17:38:46 GMT  
		Size: 3.4 MB (3380168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:5ae7085d4e101af0c66da140daa6e3c537f23a4756408dd81c8c2dc9390a6c5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137870188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9707a13284c4a22276d767f12d065c80a3b70bbe032b47c5387d8cad8345aa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:41 GMT
ADD file:31d79ffa066673b66c0325dbebd1942a91b69cf7ecd099a238f8fe8ea808dc09 in / 
# Thu, 02 Dec 2021 07:19:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 13:06:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 13:06:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 13:06:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 13:07:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 13:07:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 13:09:22 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 13:09:22 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 13:09:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 13:09:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 13:09:31 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 13:09:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 13:09:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 13:09:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 13:45:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 13:45:34 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 13:45:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 13:45:34 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 13:45:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 13:45:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 13:47:04 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:47:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 13:47:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 13:47:05 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 13:47:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:47:05 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 13:47:06 GMT
EXPOSE 80
# Thu, 02 Dec 2021 13:47:06 GMT
CMD ["apache2-foreground"]
# Thu, 02 Dec 2021 23:34:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 23:34:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Dec 2021 23:42:37 GMT
ENV DRUPAL_VERSION=7.83
# Thu, 02 Dec 2021 23:42:38 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Thu, 02 Dec 2021 23:42:39 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:9db828d777b90dcc2d341a4b3c3f7d99b1665d766b83afb9c326389d04ccc3da`  
		Last Modified: Thu, 02 Dec 2021 07:25:46 GMT  
		Size: 25.8 MB (25769061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00adb866cc42f70c03a11a3f32466de280815ff710c19c4d1e4be048bd49385`  
		Last Modified: Thu, 02 Dec 2021 14:18:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2020bd7583ae58120082ff6edec8b44afd5d503ee3693a92091ee6c7cbbf19d7`  
		Last Modified: Thu, 02 Dec 2021 14:18:17 GMT  
		Size: 64.7 MB (64712007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3c94bcead758993b2fbbb69b8f60d85da7ca92db1d7c10102dabe72a030c8c`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5af4dfe0a1a7672129cca14f4ec5d9fe166b039ea82fbd3015ae3a063c4530d`  
		Last Modified: Thu, 02 Dec 2021 14:18:40 GMT  
		Size: 18.5 MB (18524860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f99998986ec3d6033d1f28c5115f6d91b93d2cf4c973852877fe6a5615533`  
		Last Modified: Thu, 02 Dec 2021 14:18:37 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47becfb5e0a89fe00001213e04c5f36077afd6f481b8da6371d13401b11893ec`  
		Last Modified: Thu, 02 Dec 2021 14:18:37 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3818a1f73db7629f35512aabf837ffce2f0989113704908171812ef0e5352b13`  
		Last Modified: Thu, 02 Dec 2021 14:24:11 GMT  
		Size: 10.8 MB (10756341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ceea206c924d43ea1f95e9635e6d32cfafdfc5bbc80101cdbdda207451940c3`  
		Last Modified: Thu, 02 Dec 2021 14:24:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97db73e198d90c48a020871cdbd2d208ca9183ca7ee350d60c13eff1bcdf8bae`  
		Last Modified: Thu, 02 Dec 2021 14:24:11 GMT  
		Size: 13.1 MB (13067277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c488fab1ce971cb7f4d67eeff8ac8bd024379991a79fb813b3131c43f212d01`  
		Last Modified: Thu, 02 Dec 2021 14:24:09 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25601843e92342717d0ab8491fb17bde0bb4858f4e1e5dd5d0d3819f595696af`  
		Last Modified: Thu, 02 Dec 2021 14:24:09 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86683b60691faef16f24b1063782c507cf2d9e4afb4de069bcc71a819b7c57ec`  
		Last Modified: Thu, 02 Dec 2021 14:24:09 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e25cc08221ee8b9545759ea3d50a12e1ccfade8ae2011e8f61de991edaa398`  
		Last Modified: Thu, 02 Dec 2021 23:53:48 GMT  
		Size: 1.7 MB (1654732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f1e7ae5de0e68425a297a35d2ac6897cebbc13a97556697350e4f0e637ebbe`  
		Last Modified: Thu, 02 Dec 2021 23:53:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a33da5e554933d3ba43dfd2967a60ba0595fa53e0cd4f742a36bc47fcc197ad`  
		Last Modified: Thu, 02 Dec 2021 23:58:55 GMT  
		Size: 3.4 MB (3380166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
