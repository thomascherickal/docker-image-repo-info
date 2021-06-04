## `drupal:7-php7.4-apache`

```console
$ docker pull drupal@sha256:b96a6ae663bb27fdee44f21e7c5d6ddcb08201b5ec231236d506eb7077be5ae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `drupal:7-php7.4-apache` - linux; amd64

```console
$ docker pull drupal@sha256:c5941d1c8ec761c21ddc06b719b99cb5f2d87dc7aa866791ff4588c4f800dad4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.1 MB (152111633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc17f5179725b8ca760cb696788b63875fed3d45a9da1a492b0b47e3f275b76b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 12:42:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 May 2021 12:42:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 May 2021 12:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 12:43:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 May 2021 12:43:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 12 May 2021 12:48:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 May 2021 12:48:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 May 2021 12:48:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 May 2021 12:48:30 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 May 2021 12:48:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 May 2021 12:48:32 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 12 May 2021 12:48:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 12 May 2021 12:48:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 12:48:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 12:48:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 May 2021 13:11:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Jun 2021 21:45:52 GMT
ENV PHP_VERSION=7.4.20
# Thu, 03 Jun 2021 21:45:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Thu, 03 Jun 2021 21:45:52 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Thu, 03 Jun 2021 21:46:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 03 Jun 2021 21:46:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:50:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Jun 2021 21:50:15 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:50:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Jun 2021 21:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Jun 2021 21:50:17 GMT
STOPSIGNAL SIGWINCH
# Thu, 03 Jun 2021 21:50:17 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:50:17 GMT
WORKDIR /var/www/html
# Thu, 03 Jun 2021 21:50:18 GMT
EXPOSE 80
# Thu, 03 Jun 2021 21:50:18 GMT
CMD ["apache2-foreground"]
# Thu, 03 Jun 2021 23:05:46 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 23:05:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Jun 2021 23:12:39 GMT
ENV DRUPAL_VERSION=7.81
# Thu, 03 Jun 2021 23:12:39 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Thu, 03 Jun 2021 23:12:41 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2040822db3250a09a3fee8c4e36a2a87d925b04776a46ea33dd94c111d5af366`  
		Last Modified: Wed, 12 May 2021 14:24:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4ca5ae9dfad3ef8929b7c016d54518c9d29b6da520c7728e17885936824da8`  
		Last Modified: Wed, 12 May 2021 14:24:34 GMT  
		Size: 76.7 MB (76679546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1fe7c6d9669614ca12d3a7e70ba5aa1a348b8620e251245d7dbf01f8b927b8`  
		Last Modified: Wed, 12 May 2021 14:24:17 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b26fc9ce030104e3ed1dc2b6231067d9eaa629b129a71c9bc21aed211beb9dd`  
		Last Modified: Wed, 12 May 2021 14:25:36 GMT  
		Size: 18.7 MB (18679215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3492f4769444367000d2c12c6b1482630c1a6df69440fa64ee6d34e6ce93f2ae`  
		Last Modified: Wed, 12 May 2021 14:25:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dec05775a74fc3e3e317e71f6b606242142211e697a35c9dcfcef9ea4887113`  
		Last Modified: Wed, 12 May 2021 14:25:31 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77107a42338e317f4e7f615781151c093ea1d1ce6b546c01f998ddb23428d80b`  
		Last Modified: Thu, 03 Jun 2021 23:00:13 GMT  
		Size: 10.7 MB (10683966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58e4093c52a90c69bc4dbb5b52b9d72c8708bbdd4e399c832825675cfe8990b`  
		Last Modified: Thu, 03 Jun 2021 23:00:10 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32715f578d3551449631d4adad0318ec0f488cf038529ba9f14f3be3edc8724`  
		Last Modified: Thu, 03 Jun 2021 23:00:12 GMT  
		Size: 13.8 MB (13841171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a73fb2558cefc3be8d537b1e286e38677182e59a5b3378f736c93c46c811c40`  
		Last Modified: Thu, 03 Jun 2021 23:00:10 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667b573fcff78ef690b873a96185645530203561e6a74a472960a8cd10b7cf2e`  
		Last Modified: Thu, 03 Jun 2021 23:00:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e2da936ffe1248e4bc536a028df1d858387a7d4d491f3c2ef81f2df1be8e4e`  
		Last Modified: Thu, 03 Jun 2021 23:00:09 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b105d607c56fd50f93b8134c5ca87596f8074c18156c7aac613a39b83febc63`  
		Last Modified: Thu, 03 Jun 2021 23:15:56 GMT  
		Size: 1.7 MB (1702953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d23568d8cba85a3d1205314634548b69bc8b3cc9b16ea4d71dfd9c2cec0475`  
		Last Modified: Thu, 03 Jun 2021 23:15:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89ba18304343935b43e585931bea5cc0242a9396e006a2ba125d0eed91067f9`  
		Last Modified: Thu, 03 Jun 2021 23:23:04 GMT  
		Size: 3.4 MB (3373148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; arm variant v5

```console
$ docker pull drupal@sha256:74576ebc50f2dc4e029ea00b4da5af6bbdce03aad58baaa284f05229bbfd3516
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130304124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4c5c13d2e2106046934075f99320476d36dbc6a8b0de20eb100ce38b771cf2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Thu, 03 Jun 2021 21:48:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 03 Jun 2021 21:48:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 03 Jun 2021 21:49:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 21:49:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 03 Jun 2021 21:49:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 03 Jun 2021 22:01:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 03 Jun 2021 22:01:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 03 Jun 2021 22:01:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 03 Jun 2021 22:01:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 03 Jun 2021 22:01:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 03 Jun 2021 22:01:41 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 03 Jun 2021 22:01:41 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 03 Jun 2021 22:01:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 03 Jun 2021 22:01:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 03 Jun 2021 22:01:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 03 Jun 2021 22:44:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Jun 2021 22:44:30 GMT
ENV PHP_VERSION=7.4.20
# Thu, 03 Jun 2021 22:44:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Thu, 03 Jun 2021 22:44:31 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Thu, 03 Jun 2021 22:44:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 03 Jun 2021 22:44:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Jun 2021 22:51:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Jun 2021 22:51:37 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 03 Jun 2021 22:51:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Jun 2021 22:51:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Jun 2021 22:51:39 GMT
STOPSIGNAL SIGWINCH
# Thu, 03 Jun 2021 22:51:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 03 Jun 2021 22:51:39 GMT
WORKDIR /var/www/html
# Thu, 03 Jun 2021 22:51:40 GMT
EXPOSE 80
# Thu, 03 Jun 2021 22:51:40 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 02:08:50 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Jun 2021 02:08:52 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 02:08:52 GMT
ENV DRUPAL_VERSION=7.81
# Fri, 04 Jun 2021 02:08:52 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Fri, 04 Jun 2021 02:08:55 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2586fe00a043dd4a308161843ce4077416ee1eb08ebf096207b7d23f9f3b3de`  
		Last Modified: Fri, 04 Jun 2021 00:42:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e05631e0ebedf22784e28674ec126d70bafe19c18bec3031903329f3c79fe5c`  
		Last Modified: Fri, 04 Jun 2021 00:43:11 GMT  
		Size: 58.8 MB (58817851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850ed464f4dbbf5c771b2bd4ee9004e4554b1b3217e8ccaf4af0f11f7baa9cb3`  
		Last Modified: Fri, 04 Jun 2021 00:42:46 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e335f475b8f113fa030043460844251e4fc58055674a0e137a2b66dbde30fe`  
		Last Modified: Fri, 04 Jun 2021 00:44:39 GMT  
		Size: 18.0 MB (18026183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de8fa27349aadb3b3619f582ef569d38bd0735de86fb3171e4e3f7e0bd4a4e6`  
		Last Modified: Fri, 04 Jun 2021 00:44:32 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dcdf047bddbca4663a3c80f35009946585e5d15e5708473b0a061e9dc6066f`  
		Last Modified: Fri, 04 Jun 2021 00:44:32 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275591aecc011ba6df623d93406e428c30ac0db5bb47130419d58a69ab33c937`  
		Last Modified: Fri, 04 Jun 2021 00:48:15 GMT  
		Size: 10.7 MB (10681994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912ffaa8e1ffbb34e95ff268b6aee984501816405737b158c2ae2e4f7936fc5c`  
		Last Modified: Fri, 04 Jun 2021 00:48:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8f3bb8723c3b78f4d276ef16483f1eda9da096e6525914d87408c36c04f06a`  
		Last Modified: Fri, 04 Jun 2021 00:48:15 GMT  
		Size: 12.9 MB (12924753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4fa8c3cac19cbc237a797d175069111823e6a4690056ac26f5002f152fd3d5`  
		Last Modified: Fri, 04 Jun 2021 00:48:10 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299d8194b8ea699081f574c3cbe69998cac9c5b887ad4fcc0cbe2bb16a83c73`  
		Last Modified: Fri, 04 Jun 2021 00:48:10 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37201db643f98582c570ec65a0a3044f82bf8f5b27184debf09a722a5a8988a`  
		Last Modified: Fri, 04 Jun 2021 00:48:10 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f7982124bd4c960630cbd4a93f37584d7793137001b2530aa44856d278c909`  
		Last Modified: Fri, 04 Jun 2021 02:12:27 GMT  
		Size: 1.6 MB (1594873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7badce808bc84e379fc51ecd18e729511e82414016b57296627dc9ed9cf8a1e7`  
		Last Modified: Fri, 04 Jun 2021 02:12:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96df8365e8c52e185bee238cdd20a3d3f1c9fc73e6d64acd862ae2d212428419`  
		Last Modified: Fri, 04 Jun 2021 02:12:28 GMT  
		Size: 3.4 MB (3373136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; arm variant v7

```console
$ docker pull drupal@sha256:d55916f029e51388319b281f0a69af186e4d2d90cca79e3d3eafbd18e951f64a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127493667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251cf1a0f7a5b70c9cb6627ab01f48646d2cf57edbb172f85d8d160b0c194438`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 10:57:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 May 2021 10:57:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 May 2021 10:58:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 10:59:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 May 2021 10:59:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 12 May 2021 11:05:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 May 2021 11:05:22 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 May 2021 11:06:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 May 2021 11:06:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 May 2021 11:07:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 May 2021 11:07:21 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 12 May 2021 11:07:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 12 May 2021 11:07:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 11:07:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 11:07:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 May 2021 11:32:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 12 May 2021 11:32:18 GMT
ENV PHP_VERSION=7.4.19
# Wed, 12 May 2021 11:32:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.19.tar.xz.asc
# Wed, 12 May 2021 11:32:27 GMT
ENV PHP_SHA256=6c17172c4a411ccb694d9752de899bb63c72a0a3ebe5089116bc13658a1467b2
# Wed, 12 May 2021 11:33:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 May 2021 11:33:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 May 2021 11:36:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 May 2021 11:36:43 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 12 May 2021 11:37:02 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 May 2021 11:37:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 May 2021 11:37:13 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 May 2021 11:37:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 May 2021 11:37:25 GMT
WORKDIR /var/www/html
# Wed, 12 May 2021 11:37:33 GMT
EXPOSE 80
# Wed, 12 May 2021 11:37:38 GMT
CMD ["apache2-foreground"]
# Wed, 26 May 2021 22:12:16 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 May 2021 22:12:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 02 Jun 2021 19:01:25 GMT
ENV DRUPAL_VERSION=7.81
# Wed, 02 Jun 2021 19:01:26 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Wed, 02 Jun 2021 19:01:27 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22352fb7feb02278ca8a5c4cc40c987d6daaa0807aeebf04d0f7fd6491bce6b9`  
		Last Modified: Wed, 12 May 2021 12:45:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b88f898fb7f5d158ba653a177fb7020d8d49f0f041b30557db247eeae68689`  
		Last Modified: Wed, 12 May 2021 12:45:28 GMT  
		Size: 59.5 MB (59512823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625219458bf4e7cb92d11dc544dcc2efe11e4ffe7c21483dfb38a07a4727adb6`  
		Last Modified: Wed, 12 May 2021 12:45:01 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd01838a18ec9767b7c80f970388dc360e09a1eb2e98351216c084f30d90e0cb`  
		Last Modified: Wed, 12 May 2021 12:46:08 GMT  
		Size: 17.5 MB (17481766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a4c6d1d0e39bc20b64661607bc1bd0fb3f411fef0fcbd3b9846c88d2233fd`  
		Last Modified: Wed, 12 May 2021 12:45:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9313d33587d68f464ee2da208483529a1aec56f272301617410494d5f2e11386`  
		Last Modified: Wed, 12 May 2021 12:45:57 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e883c42ce932ee8409002a92c9dfc07d1d5b3bada4f075a149f258c6b7b6cc`  
		Last Modified: Wed, 12 May 2021 12:47:57 GMT  
		Size: 10.7 MB (10676687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702b680e326c5e74c7ecfdcf309b0568f514bc039c59a23e0dff836d28d11ff`  
		Last Modified: Wed, 12 May 2021 12:47:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c2be2194e88b8aaafd56db8d220813d734fd7dc147e7c17e2623c82d66167`  
		Last Modified: Wed, 12 May 2021 12:47:58 GMT  
		Size: 12.2 MB (12222348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18520224e4cd01301113e18be9c1d809475ada18168286412207b57149ac8b2c`  
		Last Modified: Wed, 12 May 2021 12:47:54 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd51ac44685e23a43631525422e40ec074e0d65c736526a5404a357515a87d6`  
		Last Modified: Wed, 12 May 2021 12:47:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812dae31c3f05d29c828c5ea35c2ddd76aae18bb910be394ee4bdc5a96fdb1f`  
		Last Modified: Wed, 12 May 2021 12:47:54 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c735d090add3329d75b5642bac123fe27c3b6d47f2228b6c3242b9eb3c7546`  
		Last Modified: Wed, 26 May 2021 22:40:27 GMT  
		Size: 1.5 MB (1474898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f98c0d7223f2b38019c6dd1153a8b08284c1b400676b28adfdfe79dad83187`  
		Last Modified: Wed, 26 May 2021 22:40:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde6f74d54f1bdcf93f4a61f4f4cc0d38091434abf5651b2270c60ca4f40f187`  
		Last Modified: Wed, 02 Jun 2021 19:13:31 GMT  
		Size: 3.4 MB (3373151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:7cb2b7745c55cad0e44bc8700715ed30ac81e1bc686b6c5f952fb07f52dca942
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144230330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a49426c4d5eb8dcc8933faed396994ebbbdac73a915ebbda72e64e16d321f2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Fri, 04 Jun 2021 00:27:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 04 Jun 2021 00:27:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 04 Jun 2021 00:27:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Jun 2021 00:27:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 04 Jun 2021 00:27:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 04 Jun 2021 00:31:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 04 Jun 2021 00:31:00 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 04 Jun 2021 00:31:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 04 Jun 2021 00:31:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 04 Jun 2021 00:31:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 04 Jun 2021 00:31:10 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 04 Jun 2021 00:31:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 04 Jun 2021 00:31:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 04 Jun 2021 00:31:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 04 Jun 2021 00:31:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 04 Jun 2021 01:04:11 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 04 Jun 2021 01:04:11 GMT
ENV PHP_VERSION=7.4.20
# Fri, 04 Jun 2021 01:04:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Fri, 04 Jun 2021 01:04:11 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Fri, 04 Jun 2021 01:04:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 01:04:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 01:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 01:06:27 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 01:06:28 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 01:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 01:06:28 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 01:06:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 01:06:28 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 01:06:29 GMT
EXPOSE 80
# Fri, 04 Jun 2021 01:06:29 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 03:06:47 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Jun 2021 03:06:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 03:14:38 GMT
ENV DRUPAL_VERSION=7.81
# Fri, 04 Jun 2021 03:14:38 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Fri, 04 Jun 2021 03:14:40 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d547f5a00c91fdfd427db81ba2de70616ba7e4b2158a2b162c846c3cd834f3`  
		Last Modified: Fri, 04 Jun 2021 02:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daebef4d8872054f7aa065e0b9f221d60fca1a45f2da4fb04536c10ac129fa23`  
		Last Modified: Fri, 04 Jun 2021 02:41:18 GMT  
		Size: 70.4 MB (70356256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f3aa932bc23c2453a034b0f74ef8b029be2d8cfb6fc7b17764d0ce0231612a`  
		Last Modified: Fri, 04 Jun 2021 02:41:06 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4719d0ede6fc5a24ae234b47a1ce1e1c1c023ba6369da6e4899e02aa6e0d1d36`  
		Last Modified: Fri, 04 Jun 2021 02:42:30 GMT  
		Size: 18.6 MB (18579971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439e17f37fd307cf02821f65c5691f8796cc80eb641d5e2c15bfc3d522079afa`  
		Last Modified: Fri, 04 Jun 2021 02:42:27 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ec9e53c285fda553d9e6373cdea8c4f731734707fd144e95d0f24b07a452d7`  
		Last Modified: Fri, 04 Jun 2021 02:42:27 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832773f46986ae1833cdc214d1cc73a58d16521502391956e69998604dd45f50`  
		Last Modified: Fri, 04 Jun 2021 02:48:00 GMT  
		Size: 10.7 MB (10682659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c9aed57499689af02a453d14b3223ef4b834677549fc392ab3190d1916a620`  
		Last Modified: Fri, 04 Jun 2021 02:47:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f7df2b795e0ec644d302466a45062d16e14beded961ab31b5c50de5ab9e626`  
		Last Modified: Fri, 04 Jun 2021 02:48:00 GMT  
		Size: 13.6 MB (13628680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b7262a50720acbe76c04f46965e8844f9b2daa98d9195927cbec603ba60a18`  
		Last Modified: Fri, 04 Jun 2021 02:47:57 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2760f08868c432eac9a4da1718c39f1a9785de72c6c667c5fcfebd830e96cc`  
		Last Modified: Fri, 04 Jun 2021 02:47:57 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157e981ceddb1647fad9472aeeb6c8ae850d34548af5c9a2c0cad1cb746401ca`  
		Last Modified: Fri, 04 Jun 2021 02:47:57 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f77e05388b60495d14f62d5a450f5058a2cff68e0558bba6c6ce941acbe6eeb`  
		Last Modified: Fri, 04 Jun 2021 03:25:17 GMT  
		Size: 1.7 MB (1692657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35541d6228c23ee283d6957d0a103b2ab799fd45bb0c9ff1235bdf3d0ec1df4`  
		Last Modified: Fri, 04 Jun 2021 03:25:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0eaeafe5114ea48aa2dd1c667fb18284e684abe81c21766d00ed83b7ec941ac`  
		Last Modified: Fri, 04 Jun 2021 03:33:16 GMT  
		Size: 3.4 MB (3373137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; 386

```console
$ docker pull drupal@sha256:e9d00618bb93aa23a05000b122dd8ba015c42b1d959415052bea763212f5584c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158162427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b72ae334f5e51a2e96abaf6bb782cc82df25a924ce4acfbeba61c7c5956755fc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 10:29:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 May 2021 10:29:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 May 2021 10:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 10:29:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 May 2021 10:29:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 12 May 2021 10:37:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 May 2021 10:37:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 May 2021 10:37:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 May 2021 10:37:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 May 2021 10:37:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 May 2021 10:37:19 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 12 May 2021 10:37:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 12 May 2021 10:37:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 10:37:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 10:37:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 May 2021 11:05:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Jun 2021 21:50:26 GMT
ENV PHP_VERSION=7.4.20
# Thu, 03 Jun 2021 21:50:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Thu, 03 Jun 2021 21:50:26 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Thu, 03 Jun 2021 21:50:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 03 Jun 2021 21:50:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:55:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Jun 2021 21:55:27 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:55:29 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Jun 2021 21:55:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Jun 2021 21:55:29 GMT
STOPSIGNAL SIGWINCH
# Thu, 03 Jun 2021 21:55:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:55:30 GMT
WORKDIR /var/www/html
# Thu, 03 Jun 2021 21:55:30 GMT
EXPOSE 80
# Thu, 03 Jun 2021 21:55:31 GMT
CMD ["apache2-foreground"]
# Thu, 03 Jun 2021 23:21:12 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 23:21:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Jun 2021 23:29:30 GMT
ENV DRUPAL_VERSION=7.81
# Thu, 03 Jun 2021 23:29:30 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Thu, 03 Jun 2021 23:29:31 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a6012e74b9298cbe4936d73f6694f467e692dfe3130410f328cc59b3de2ec6`  
		Last Modified: Wed, 12 May 2021 12:25:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b14d908cddd1fdc9c095659188c3778da604ce674953cc0ed6e25f8fecd6301`  
		Last Modified: Wed, 12 May 2021 12:26:04 GMT  
		Size: 81.2 MB (81230367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0703ccc94437b3b2b071a425e7d402955ab19778a1ad674a0ca8a21a1962e78`  
		Last Modified: Wed, 12 May 2021 12:25:37 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e6aca3d072c9f95c6d0423f61779ccfcdd2d5b0ce57000d02c5fa1c48cb1b`  
		Last Modified: Wed, 12 May 2021 12:27:15 GMT  
		Size: 19.1 MB (19114945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c556c76ca8a7a51e5d551d68a80f4c66c80ed83e36cad9e2b6ac826ed63a5db1`  
		Last Modified: Wed, 12 May 2021 12:27:10 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b1655d902066aeb6df69d60c905f98e7f5dead03fcecdd90a3355e8601a94`  
		Last Modified: Wed, 12 May 2021 12:27:10 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfd77d3682cc05ff1df8682ca76082353e9c34693593164d5788a4c639064ee`  
		Last Modified: Thu, 03 Jun 2021 23:10:45 GMT  
		Size: 10.7 MB (10683259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3aec4420cad143acf41b9e7218cc0495efac9d77493908c39398fad144246`  
		Last Modified: Thu, 03 Jun 2021 23:10:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6dae33359b26ae1569531226b62f9eacdbd9ccce88df61c2ded014ddb207f0`  
		Last Modified: Thu, 03 Jun 2021 23:10:49 GMT  
		Size: 14.2 MB (14172182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ac151e650e0e321cd992321a89a2fb30c91cb355c4c80743138ec5a981c567`  
		Last Modified: Thu, 03 Jun 2021 23:10:40 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefeea5b5d5d73c7e4c81a4ba7f89bb3fbdee1ef5ff3ef6c6147b0d2454abb2b`  
		Last Modified: Thu, 03 Jun 2021 23:10:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a5cc7153f1fc70e6b84f79257e4da229bf4108826fc50592cda91f2c36c055`  
		Last Modified: Thu, 03 Jun 2021 23:10:40 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc118c7d8b8291e82554a0e97a5770abe3a17c463680ce5fb2b050a88c5463e`  
		Last Modified: Thu, 03 Jun 2021 23:36:55 GMT  
		Size: 1.8 MB (1787738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab25dac12e67bf2894c44fdd6de83ae36a6d108c027b789bfed8182e7fee0ff1`  
		Last Modified: Thu, 03 Jun 2021 23:36:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2769d3f23bc4646f461840d5f0dd52519f76db3c46583a28604f7c4cb8f863d`  
		Last Modified: Thu, 03 Jun 2021 23:45:37 GMT  
		Size: 3.4 MB (3373138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; mips64le

```console
$ docker pull drupal@sha256:039085128c5b4bde54d2ee56133bd0a9e36f708815c42bb0c7e900a34d9e8f67
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134729092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1db3ac1f145b640aa7e720a6156597b8076c4661f1df8f1674a67a3b0ea05e00`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 10:17:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 May 2021 10:17:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 May 2021 10:18:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 10:18:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 May 2021 10:18:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 12 May 2021 10:30:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 May 2021 10:30:54 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 May 2021 10:31:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 May 2021 10:31:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 May 2021 10:31:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 May 2021 10:31:25 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 12 May 2021 10:31:26 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 12 May 2021 10:31:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 10:31:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 10:31:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 May 2021 11:19:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Jun 2021 21:16:16 GMT
ENV PHP_VERSION=7.4.20
# Thu, 03 Jun 2021 21:16:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Thu, 03 Jun 2021 21:16:17 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Thu, 03 Jun 2021 21:16:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 03 Jun 2021 21:16:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Jun 2021 21:24:30 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:24:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Jun 2021 21:24:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Jun 2021 21:24:33 GMT
STOPSIGNAL SIGWINCH
# Thu, 03 Jun 2021 21:24:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:24:33 GMT
WORKDIR /var/www/html
# Thu, 03 Jun 2021 21:24:34 GMT
EXPOSE 80
# Thu, 03 Jun 2021 21:24:34 GMT
CMD ["apache2-foreground"]
# Thu, 03 Jun 2021 22:34:05 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 22:34:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Jun 2021 22:34:07 GMT
ENV DRUPAL_VERSION=7.81
# Thu, 03 Jun 2021 22:34:08 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Thu, 03 Jun 2021 22:34:11 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f283cbfbaba47c98021eab6ee697e5defea6f86e25b0e7b8fbd34e2090cc129`  
		Last Modified: Wed, 12 May 2021 12:40:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3faf4ed12762bcc54095098c6677437ad34843514935b655a506b2a3e534769`  
		Last Modified: Wed, 12 May 2021 12:41:22 GMT  
		Size: 61.4 MB (61404028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4750f0df4fd64e45217d89e4c39e0ba64d76784691c74cd4dc027dd6656486b9`  
		Last Modified: Wed, 12 May 2021 12:40:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5dd148bfacdfa12ee384ed9c45ca5eb39bff5fb57a853569272eecf8339dfb`  
		Last Modified: Wed, 12 May 2021 12:42:30 GMT  
		Size: 18.6 MB (18611746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaea65323b38aae4718399a07820992a202b5e152881f5771c84e8fe944aa21`  
		Last Modified: Wed, 12 May 2021 12:42:17 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55bdb5d36cee74d52082160cd3d30b20e5f81c2dc01c2b7acce89682eb71015`  
		Last Modified: Wed, 12 May 2021 12:42:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71103ce54c078c6b71e33cdffdf0ec8a0d7dade3f0b6733df7aacef288d6ad`  
		Last Modified: Thu, 03 Jun 2021 21:54:00 GMT  
		Size: 10.7 MB (10681372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef19292290db57dfb1d3f070414a9569566498629c2c1df925401cce488f4d2`  
		Last Modified: Thu, 03 Jun 2021 21:53:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac14056aed544cad6410ec1fad9ed3d23075d98d950a5bc3c11403f99110f24`  
		Last Modified: Thu, 03 Jun 2021 21:54:05 GMT  
		Size: 13.1 MB (13147789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706365c8d5de1b20c1a600e4683ae25d125ae5fb9813a082d71166145d760d0e`  
		Last Modified: Thu, 03 Jun 2021 21:53:53 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1e7c7a62c703467ce329655b35daf5f41d758f5d177f0c0b6b31fff31397bd`  
		Last Modified: Thu, 03 Jun 2021 21:53:53 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6fdf0881e2404b7d11398f0785176de41d327eb82c783199f8a936e87072a2`  
		Last Modified: Thu, 03 Jun 2021 21:53:53 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dd6366e5e2d72ad4afc23d608fffd69a56ea1575d8f320e6aa76f30da71010`  
		Last Modified: Thu, 03 Jun 2021 22:37:05 GMT  
		Size: 1.7 MB (1692808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22ad9cbbac5de9d8bb4b4c9d4b01900183b23260392c649a3d206c1dda38dba`  
		Last Modified: Thu, 03 Jun 2021 22:37:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7eb703847ac4e69fa5800f0a8e0fe294c5ad9d88c596320f4f24ad0c13df34`  
		Last Modified: Thu, 03 Jun 2021 22:37:07 GMT  
		Size: 3.4 MB (3372843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; ppc64le

```console
$ docker pull drupal@sha256:af073e4cdd7b84e6decf184802a52011bcec0236a3afa969a8e2d547d6476132
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163547387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3250df9252164940db0454edccc45f71145a33d178980756aed06e01048b9ca7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:38:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 May 2021 14:39:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 May 2021 14:43:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:43:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 May 2021 14:43:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 12 May 2021 14:56:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 May 2021 14:56:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 May 2021 14:58:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 May 2021 14:58:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 May 2021 14:58:50 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 May 2021 14:58:55 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 12 May 2021 14:59:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 12 May 2021 14:59:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 14:59:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 14:59:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 May 2021 15:35:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 04 Jun 2021 00:04:19 GMT
ENV PHP_VERSION=7.4.20
# Fri, 04 Jun 2021 00:04:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Fri, 04 Jun 2021 00:04:33 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Fri, 04 Jun 2021 00:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 00:08:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:17:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 00:17:59 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:18:12 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 00:18:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 00:18:23 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 00:18:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:18:51 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 00:18:57 GMT
EXPOSE 80
# Fri, 04 Jun 2021 00:19:02 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 01:25:49 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Jun 2021 01:25:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 01:47:40 GMT
ENV DRUPAL_VERSION=7.81
# Fri, 04 Jun 2021 01:47:48 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Fri, 04 Jun 2021 01:48:12 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a14bc264585c89d8cac3708bf24a395fe650eb6722f3b4e9e8c70782fb5a4`  
		Last Modified: Wed, 12 May 2021 16:48:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077c017d1b8e5687ac5dad9953152fca3eb76d6003e9933234d2061e96bd825`  
		Last Modified: Wed, 12 May 2021 16:49:56 GMT  
		Size: 82.3 MB (82291076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea04b608bfa2044926ed943edbb39e52bbefe5d0509664702303abd8d8da7e2`  
		Last Modified: Wed, 12 May 2021 16:48:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c3367ec2f621b030af9b865d74efc201e2e1e248d8447c169c24073b5a4533`  
		Last Modified: Wed, 12 May 2021 16:51:08 GMT  
		Size: 19.8 MB (19818351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e180c2e3763e1b77caa19e2eab6b490eb6196f9bb5d530aeb31a4c5744e012cd`  
		Last Modified: Wed, 12 May 2021 16:50:51 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6fc71e2b139cac61559f5c31a52b2082da8d9ac52ba363789f8cea8e36d87`  
		Last Modified: Wed, 12 May 2021 16:50:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e2fca09acf24300313364ebcdb54b1f98beb863867d1b3487dcb269c8ba8f0`  
		Last Modified: Fri, 04 Jun 2021 01:17:33 GMT  
		Size: 10.7 MB (10684131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6f226f7c7e05acb053d0e37841930fd2d9b60988976e085af4bef029d2fd95`  
		Last Modified: Fri, 04 Jun 2021 01:17:29 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2d37bd4167fbfff135acc32c3f40f77219edce2f6674e11ce27000e43fb9ec`  
		Last Modified: Fri, 04 Jun 2021 01:17:32 GMT  
		Size: 14.9 MB (14882023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfad6d06e892ebc650dde5d9691548e315ee537cd49c6441f29704cbd320686`  
		Last Modified: Fri, 04 Jun 2021 01:17:30 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fedb58f73042e42e43d150d3ce33a27140d8ab3de34a5d4342886df93c2239`  
		Last Modified: Fri, 04 Jun 2021 01:17:29 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367739fcd6cb8cbc8f9080a3d3c29269eaf627b8d73b25fed8f2479847547ba3`  
		Last Modified: Fri, 04 Jun 2021 01:17:29 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0832c4d86946f4e36adef8a3a62349456efcc5656e29531819a7468a4e3689d3`  
		Last Modified: Fri, 04 Jun 2021 01:52:21 GMT  
		Size: 1.9 MB (1940529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80fba7c7da128fdf25958204b8d925df02a5744c2c4d1f84dc4dc542fc0d22f`  
		Last Modified: Fri, 04 Jun 2021 01:52:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61459171b3dd56e1e5ab67634540d001ad828aabc07f0fd826045133398263d`  
		Last Modified: Fri, 04 Jun 2021 02:21:40 GMT  
		Size: 3.4 MB (3373145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-apache` - linux; s390x

```console
$ docker pull drupal@sha256:ae07630cf5d28f7d15f0d32f259209b68c59ca46da3cdeaf5fb3b2f32b1ef924
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137803124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d32f9c166487133939ff1932f54fb353cb960f011ed3f2327dd34bc2cebff7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 04:39:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 May 2021 04:39:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 May 2021 04:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 04:40:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 May 2021 04:40:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 12 May 2021 04:44:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 May 2021 04:44:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 May 2021 04:45:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 May 2021 04:45:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 May 2021 04:45:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 May 2021 04:45:19 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 12 May 2021 04:45:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 12 May 2021 04:45:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 04:45:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 May 2021 04:45:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 May 2021 05:02:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Jun 2021 23:54:14 GMT
ENV PHP_VERSION=7.4.20
# Thu, 03 Jun 2021 23:54:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Thu, 03 Jun 2021 23:54:15 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Thu, 03 Jun 2021 23:54:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 03 Jun 2021 23:54:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Jun 2021 23:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Jun 2021 23:57:18 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Thu, 03 Jun 2021 23:57:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Jun 2021 23:57:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Jun 2021 23:57:21 GMT
STOPSIGNAL SIGWINCH
# Thu, 03 Jun 2021 23:57:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 03 Jun 2021 23:57:22 GMT
WORKDIR /var/www/html
# Thu, 03 Jun 2021 23:57:23 GMT
EXPOSE 80
# Thu, 03 Jun 2021 23:57:24 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 00:47:26 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Jun 2021 00:47:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 00:56:21 GMT
ENV DRUPAL_VERSION=7.81
# Fri, 04 Jun 2021 00:56:22 GMT
ENV DRUPAL_MD5=ca21e214b3de1453e71f2eb1ab182c3d
# Fri, 04 Jun 2021 00:56:23 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f858f0a7a9a17707b5c8ce7aff5e0c8177f92ad170f0fcfe34ec021cd2eecf`  
		Last Modified: Wed, 12 May 2021 05:36:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3360e595e85bb6804af9e2f0df01e74859712eba8c22a3cb2a2a5f31b389d6`  
		Last Modified: Wed, 12 May 2021 05:36:33 GMT  
		Size: 64.7 MB (64710136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2468f59807a3a09c29661c3ff01a719db4cf479d16be33ede8bae9120feae245`  
		Last Modified: Wed, 12 May 2021 05:36:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a81c4b3a8fb8986f448a9d68c61e986f5535e39ab71e32e28db5f9a80a9f3a`  
		Last Modified: Wed, 12 May 2021 05:37:00 GMT  
		Size: 18.5 MB (18525103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c031d0df465590a38b85d7e83aeab770250d709ffd5d486001b88cfbe3bba1f8`  
		Last Modified: Wed, 12 May 2021 05:36:58 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ef7a37da49dd7d88cbdd2a05a72ce8b2f168696c8746586cc509034f4a8dae`  
		Last Modified: Wed, 12 May 2021 05:36:57 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5579a09782180f5a2e53d528d3868726715c5852b19a4ba60e85116b3e074f`  
		Last Modified: Fri, 04 Jun 2021 00:43:29 GMT  
		Size: 10.7 MB (10682406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9839e70562395969783d6291a1284d818bef0f6c5f5df9ec32203f49bb0da45`  
		Last Modified: Fri, 04 Jun 2021 00:43:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0f9c8321f9fee2d7fc3bf006679bd4fabfda7370df83a07df10bab6b1b7049`  
		Last Modified: Fri, 04 Jun 2021 00:43:29 GMT  
		Size: 13.1 MB (13058278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9027834f47de02b3e1b3c79e476d764b91ecc24f23ee16525bf83b93c72323`  
		Last Modified: Fri, 04 Jun 2021 00:43:27 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280b635aa6dfb1a96407e2f7e13be0b6412b1dc8fa20f2535b280fdfa417d278`  
		Last Modified: Fri, 04 Jun 2021 00:43:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb786f96da358e313b35b584b2dd39ec10a7a4b28ae061df71747e9ddb685a5`  
		Last Modified: Fri, 04 Jun 2021 00:43:27 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7c12a5ad7b2c8e23012d7f4ee02a28fc3b382c307f4314c93e8285d0a1b1d7`  
		Last Modified: Fri, 04 Jun 2021 00:58:54 GMT  
		Size: 1.7 MB (1688154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017e1527e6f6a2f629cd92ab43616cc89f3fd037a2c32b142c099e7d04d61a12`  
		Last Modified: Fri, 04 Jun 2021 00:58:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eaec850787b12872504eb07d9e409f718ea275e182d93c569abddc0a17d4c3d`  
		Last Modified: Fri, 04 Jun 2021 01:02:30 GMT  
		Size: 3.4 MB (3373151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
