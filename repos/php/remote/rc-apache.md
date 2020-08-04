## `php:rc-apache`

```console
$ docker pull php@sha256:ff9abf77ea8e4f8c02c99247612b7d6b07dc02a319bdc13cf12ab3cc134f76b4
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

### `php:rc-apache` - linux; amd64

```console
$ docker pull php@sha256:6732465f835e7829cdd2c7ad78c3b4030737ec6ccc3455ea7ba58d4f0a2dca9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.1 MB (147089946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855864e95ab94e8b33f268319a55bdf8b1c972013cd12f0a391b9e70c669cdd8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:44:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 08:44:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 08:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:44:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 08:44:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 08:53:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 08:53:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 08:53:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 08:53:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 08:53:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:53:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:53:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 08:53:22 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jul 2020 19:26:33 GMT
ENV PHP_VERSION=8.0.0alpha3
# Thu, 23 Jul 2020 19:26:34 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Thu, 23 Jul 2020 19:26:34 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Thu, 23 Jul 2020 19:26:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jul 2020 19:26:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:35:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 23 Jul 2020 19:35:05 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:35:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jul 2020 19:35:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jul 2020 19:35:07 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jul 2020 19:35:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:35:08 GMT
WORKDIR /var/www/html
# Thu, 23 Jul 2020 19:35:09 GMT
EXPOSE 80
# Thu, 23 Jul 2020 19:35:09 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081a822af59557fab64a7e6b1f10993a1447c4565bee919c5a63f20e5d447207`  
		Last Modified: Wed, 22 Jul 2020 11:57:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5bea655fca655018e10a9078d5092b4d7d491ef2a9c380a0adf1c7ed119b88`  
		Last Modified: Wed, 22 Jul 2020 11:57:28 GMT  
		Size: 76.6 MB (76648810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d9e6a44c7084c807b3c4203ec786d5bb187a14e4344496dca2d4148030e6e`  
		Last Modified: Wed, 22 Jul 2020 11:57:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c80d726a75cac175ad1a0f31047d9b7809b93e94ee08e0ea99d1fa8b2f8229`  
		Last Modified: Wed, 22 Jul 2020 11:57:50 GMT  
		Size: 18.7 MB (18675907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f3ef5189e5c08bea0c669d2d214c7c8acc874f2b8f37bff1747483a664515c`  
		Last Modified: Wed, 22 Jul 2020 11:57:44 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a9c1efdc831a6e3cc46fd388cfac71cc76d715242b9c3a1a389dce263c3cc0`  
		Last Modified: Wed, 22 Jul 2020 11:57:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f680197a9ed46048286d0e6c958e9dff9be5d80aac3eda9aa9e42820f9af2d`  
		Last Modified: Thu, 23 Jul 2020 20:09:14 GMT  
		Size: 10.8 MB (10843653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49faeb5185bfdd6fdbfb44d0d224db5dbca76998bce0276423b0750add131a5a`  
		Last Modified: Thu, 23 Jul 2020 20:09:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07249824579529269a1e721b3ec3134773b170c548ec4e48031e9ac0add946`  
		Last Modified: Thu, 23 Jul 2020 20:09:16 GMT  
		Size: 13.8 MB (13817740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb93797f7f9eac2205b1e15d413fa727e0576dba9e3c8c567e2f0df9030ed0e7`  
		Last Modified: Thu, 23 Jul 2020 20:09:13 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bf65e5eb92070c530e9d6daf3d8851e5204389ee077ddc737161f473a4c81`  
		Last Modified: Thu, 23 Jul 2020 20:09:13 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54e085fec922b72ad1889f1dbed8bacf8f210727638b6078e045d3f972a7324`  
		Last Modified: Thu, 23 Jul 2020 20:09:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; arm variant v5

```console
$ docker pull php@sha256:82961a56d4acf51a1232901da104b4f6908b687f602e5f5f7cc43c6c227e4bd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125124364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0349c45a1fb700dbe142f0f7e2226648708a64d00ca1263f490d2ba98fe5137c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:45:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 07:45:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 07:46:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:46:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 07:46:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 07:53:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 07:54:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 07:54:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 07:55:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 07:56:04 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 07:56:10 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 07:56:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 07:56:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 07:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 07:56:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 07:56:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 04 Aug 2020 07:56:53 GMT
ENV PHP_VERSION=8.0.0alpha3
# Tue, 04 Aug 2020 07:56:59 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Tue, 04 Aug 2020 07:57:05 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Tue, 04 Aug 2020 07:57:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 07:58:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 08:02:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Tue, 04 Aug 2020 08:02:43 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 08:03:06 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 08:03:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 08:03:25 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 08:03:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 08:03:50 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 08:03:55 GMT
EXPOSE 80
# Tue, 04 Aug 2020 08:04:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e3ffbe19b2a2bfeeacbbe19ebc723555226e6a7355497496d611651ff34e41`  
		Last Modified: Tue, 04 Aug 2020 10:50:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a88a51e2ecb1ee8af7ea0cc9d09e9f9a11e5d54d3cf6e1bc97010e846b3a30`  
		Last Modified: Tue, 04 Aug 2020 10:51:20 GMT  
		Size: 58.8 MB (58801130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4bf35e560813a772e4257c4ed0d74c43a55e1ec64e7d07c030bf6d56a4f2f3`  
		Last Modified: Tue, 04 Aug 2020 10:50:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f69fcc5374b782b2c16b64c06ff731b1e9d02708bb5aa4444ba6384cf77b93`  
		Last Modified: Tue, 04 Aug 2020 10:51:57 GMT  
		Size: 18.0 MB (18024847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740994c3c41b9e36247528c6cfea221a46cf2708b61b1548007b88f3b966eb45`  
		Last Modified: Tue, 04 Aug 2020 10:51:51 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c342cccfcc7f66b658549dba33de7d85fb3be0d4dbc8a097d7683f135d3042d3`  
		Last Modified: Tue, 04 Aug 2020 10:51:51 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc6f01764132381fc5f398ca5aef956b061794f7e5157c6e42c26a028fa6739`  
		Last Modified: Tue, 04 Aug 2020 10:51:52 GMT  
		Size: 10.8 MB (10841324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b22a2a7dd99d452d90c43847a06ba30242c662555cb7945ecf374b8dba0236f`  
		Last Modified: Tue, 04 Aug 2020 10:51:49 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcd93d9652e99ba8113822880cef68459817a170f8e85c15066062228d4289a`  
		Last Modified: Tue, 04 Aug 2020 10:51:54 GMT  
		Size: 12.6 MB (12615581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7101085f1706d0167bc4f7cb370ed2a2d435d4458fc3484b886b7615e6dc4e4b`  
		Last Modified: Tue, 04 Aug 2020 10:51:49 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11102bf76a7b99f5c10492896dcd548c51e8d1904c6ba8429fd513c3f550c89`  
		Last Modified: Tue, 04 Aug 2020 10:51:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efdaff66e3f1abefaa2476ecddf9b8ad78869e63e98bedb9eb44707db80e0e7`  
		Last Modified: Tue, 04 Aug 2020 10:51:49 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; arm variant v7

```console
$ docker pull php@sha256:750132e1ff8a7e04f1e615ad22609de1b64fd5e5f112d7d62812f7b56372055f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122446948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8182dce2e6e0950043d9adcb7f79a464eebaf3d1efda24b8d085aa1859738aea`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 09:31:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 09:32:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:32:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 09:32:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 09:35:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 09:35:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 09:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 09:36:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 09:36:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 09:36:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 09:36:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 09:36:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 09:36:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 09:36:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 09:36:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jul 2020 19:12:33 GMT
ENV PHP_VERSION=8.0.0alpha3
# Thu, 23 Jul 2020 19:12:34 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Thu, 23 Jul 2020 19:12:36 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Thu, 23 Jul 2020 19:12:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jul 2020 19:12:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:16:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 23 Jul 2020 19:16:29 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:16:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jul 2020 19:16:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jul 2020 19:16:39 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jul 2020 19:16:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:16:43 GMT
WORKDIR /var/www/html
# Thu, 23 Jul 2020 19:16:45 GMT
EXPOSE 80
# Thu, 23 Jul 2020 19:16:46 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a476362b835810ad6f6eaecc2a497b4302f2b8ac196c911884fe753f3be0c`  
		Last Modified: Wed, 22 Jul 2020 11:54:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbec70860f5643fca4a35066a02be7aab2ad53c776daa74f2b6d2bc97ad9f9f3`  
		Last Modified: Wed, 22 Jul 2020 11:55:12 GMT  
		Size: 59.5 MB (59505456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f7b8f25575d1efc6595391f7314710b2d0187564386d0cf3a81a74c4278d6`  
		Last Modified: Wed, 22 Jul 2020 11:54:53 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b46f8661c634c6b6f0f1a6e45a3452a8731b0d139678e65fe2c43eb310e9162`  
		Last Modified: Wed, 22 Jul 2020 11:55:47 GMT  
		Size: 17.5 MB (17481960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f081e3e7911001e5da489b54d64f3752a6e5faf47b5181166f0270fa9fdd0ee`  
		Last Modified: Wed, 22 Jul 2020 11:55:42 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5aae3a57b1751f2cc89b35efb321ebaed34df66f7f7db8713b8b4c93af3685d`  
		Last Modified: Wed, 22 Jul 2020 11:55:42 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe98afaa1a901eea3679e8a976599f70b85657d212f4d8fd09b2bb9c8567186`  
		Last Modified: Thu, 23 Jul 2020 19:41:58 GMT  
		Size: 10.8 MB (10841352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8b3f0e8cff975d55626d9c344a74a6295364670efbc814b36a5a52e4ee8316`  
		Last Modified: Thu, 23 Jul 2020 19:41:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c95315f8af184557cf7e1715a8c4645a56536cc61a0cfe1c13c0bc1712bd2d5`  
		Last Modified: Thu, 23 Jul 2020 19:41:59 GMT  
		Size: 11.9 MB (11906855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba0501c15cd5be0ae704ab22a8a004b85a635d723f02f1f33eba1a889ae7f58`  
		Last Modified: Thu, 23 Jul 2020 19:41:55 GMT  
		Size: 2.3 KB (2287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef41fb4b33dc3a9c39996cc91a8d57b4bb033d25cd4dfd20118d40fcaf2daa9a`  
		Last Modified: Thu, 23 Jul 2020 19:41:55 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a2031b439a07d94e0db08d7f2dca631635d1c0ea61dc62b763d2cad859f6dc`  
		Last Modified: Thu, 23 Jul 2020 19:41:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; arm64 variant v8

```console
$ docker pull php@sha256:de1c9461ba788e5490302f31fe03bc7597759a18c9857a3ecbe730c9a6937f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138908946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ce355f5f2ec2e47994c82c4bf2512465fa4236b7a4fd4c98ff8ba722ca0f87`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:19:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 11:19:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 11:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:20:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 11:21:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 11:25:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 11:25:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 11:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 11:26:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 11:26:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 11:26:19 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 11:26:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 11:26:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:26:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:26:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 11:26:33 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jul 2020 19:49:03 GMT
ENV PHP_VERSION=8.0.0alpha3
# Thu, 23 Jul 2020 19:49:04 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Thu, 23 Jul 2020 19:49:04 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Thu, 23 Jul 2020 19:49:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jul 2020 19:49:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:53:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 23 Jul 2020 19:53:08 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:53:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jul 2020 19:53:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jul 2020 19:53:23 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jul 2020 19:53:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:53:25 GMT
WORKDIR /var/www/html
# Thu, 23 Jul 2020 19:53:26 GMT
EXPOSE 80
# Thu, 23 Jul 2020 19:53:27 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d0ba90fa18020ed9569da0e936f2c6d545f48231f27020a883d5de88d96a10`  
		Last Modified: Wed, 22 Jul 2020 13:32:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a37699742587260a77a7c676da89681dc8ca92dd2db86faee3dcc77109ccea`  
		Last Modified: Wed, 22 Jul 2020 13:33:12 GMT  
		Size: 70.3 MB (70337912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f6e19fa909b49d726f813175349e7ea4dcaa9589076b04108e40eda3f792b4`  
		Last Modified: Wed, 22 Jul 2020 13:32:49 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec0a9b64ab8386df6bf5d945a5b1c5712c549bca9f1a0d3808138b57fa607e`  
		Last Modified: Wed, 22 Jul 2020 13:34:15 GMT  
		Size: 18.6 MB (18579398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6462f70cfa9f8b1238b00624079f1dbfe0cd6c85d195dacf4fab20d812a1d26c`  
		Last Modified: Wed, 22 Jul 2020 13:34:10 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bad882d5dcc21edad5bd6842a791c6a838844f61872200feff6f162c8d1d7e1`  
		Last Modified: Wed, 22 Jul 2020 13:34:07 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060b035a483231c780c2d03587d3f544c36e78b351076b4ac98887cc097a8b6f`  
		Last Modified: Thu, 23 Jul 2020 20:16:51 GMT  
		Size: 10.8 MB (10842265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d314a9510b85b6fc8cd164150c62ddb64f1bb6afb1d53fd8577fb2cb8c9c5e3b`  
		Last Modified: Thu, 23 Jul 2020 20:16:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e5f5746becff05a3104b826a0f6388f14e32c20eeb8ded7f9bd5c8a2e51e5`  
		Last Modified: Thu, 23 Jul 2020 20:16:52 GMT  
		Size: 13.3 MB (13286137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdec056f6aeb5cc7cea9b01e07270758ada4ab5d34382ea3af89a081054468ff`  
		Last Modified: Thu, 23 Jul 2020 20:16:48 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678de9af1a389cc2458bb6f540766722a8ec50641478ae5aa64b42c29c58ff89`  
		Last Modified: Thu, 23 Jul 2020 20:16:48 GMT  
		Size: 253.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde5049e801c263ad491004b18e5bbddf2b91639feae5b9e1cfcef6cc824eab4`  
		Last Modified: Thu, 23 Jul 2020 20:16:48 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; 386

```console
$ docker pull php@sha256:be23e38b09269dcd430605bbbc45c156bef6732f8f22aadd898070f06112a775
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152781202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1018f88e26817af01c8d8fec66bfeef75e2ad020c2fb40f6ea1546389f7e881f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:42:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 08:42:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 08:43:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:43:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 08:43:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 08:51:38 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 08:51:38 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 08:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 08:51:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 08:51:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 08:51:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 08:51:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 08:51:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 08:52:00 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 23 Jul 2020 19:08:08 GMT
ENV PHP_VERSION=8.0.0alpha3
# Thu, 23 Jul 2020 19:08:08 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Thu, 23 Jul 2020 19:08:08 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Thu, 23 Jul 2020 19:08:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jul 2020 19:08:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:14:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Thu, 23 Jul 2020 19:14:06 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:14:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jul 2020 19:14:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jul 2020 19:14:08 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jul 2020 19:14:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jul 2020 19:14:08 GMT
WORKDIR /var/www/html
# Thu, 23 Jul 2020 19:14:08 GMT
EXPOSE 80
# Thu, 23 Jul 2020 19:14:08 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dac354b7d13e3bb52269c5c4afdb82d013431213a5c1abd2bcdbe7c8746143b`  
		Last Modified: Wed, 22 Jul 2020 12:01:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3244890340b96c338e5649236ef464c2002d7f8034b40bf205bcfb8303fd8`  
		Last Modified: Wed, 22 Jul 2020 12:02:07 GMT  
		Size: 81.2 MB (81195189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c2b96264b3ad05aacda736bbf4212e47ab5aa547d7838b399eb4c1bc6237e4`  
		Last Modified: Wed, 22 Jul 2020 12:01:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228dec6ce1b76c8a5be878e7aed5fff883303810056be0bf4be3a58dc1f0a8ce`  
		Last Modified: Wed, 22 Jul 2020 12:02:27 GMT  
		Size: 19.1 MB (19112759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94ed7311e87846e439b9cacb6c5f52a5f74b8f02af21ce4fdc78b69517dbd30`  
		Last Modified: Wed, 22 Jul 2020 12:02:19 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f1ef047159981233219d747b72ed47196a5229833cc54978ba380a3dd8ad91`  
		Last Modified: Wed, 22 Jul 2020 12:02:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d8a6ec00392b9176e769084e1af99c856660ef831b15fb97ec72924a240e9d`  
		Last Modified: Thu, 23 Jul 2020 19:56:10 GMT  
		Size: 10.8 MB (10842871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a148d054f9a2179e7f2de21e1f3304a2c8424a9429408ad1df711a167c8bfb`  
		Last Modified: Thu, 23 Jul 2020 19:56:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c11ccdaf7a31bedc2a6a763f4a31cfb6c14e1e3b73b2036d70a20c7c058c1`  
		Last Modified: Thu, 23 Jul 2020 19:56:15 GMT  
		Size: 13.9 MB (13870189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1ca7fba245e0646417ab70d470de8a273952dd49ff5e52bb42985c58e5dacd`  
		Last Modified: Thu, 23 Jul 2020 19:56:06 GMT  
		Size: 2.3 KB (2281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355710029ee21f28ee1fd66f37158f24c8b4615ed9d35d7aa33f053369546928`  
		Last Modified: Thu, 23 Jul 2020 19:56:07 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca547033168f355f24eda467c5c04a32f60d5fcbb45a4c7546b07ddf4c4d11`  
		Last Modified: Thu, 23 Jul 2020 19:56:07 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; mips64le

```console
$ docker pull php@sha256:591ad6382226cf1166cb955c8e51d562e23a0d34a3c27f5e45024f0d57f4d8a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129443913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c27c176417c94afa8e2fa64f1d5790c84b4a39d36f22d1f1f133cd1d64fdae`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:20:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 11:20:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 11:21:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:21:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 11:21:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 11:34:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 11:34:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 11:34:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 11:34:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 11:34:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 11:34:42 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 11:34:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 11:34:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 11:34:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 11:34:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 11:34:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 04 Aug 2020 11:34:44 GMT
ENV PHP_VERSION=8.0.0alpha3
# Tue, 04 Aug 2020 11:34:44 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Tue, 04 Aug 2020 11:34:44 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Tue, 04 Aug 2020 11:35:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 11:35:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:46:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Tue, 04 Aug 2020 11:46:49 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:46:51 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 11:46:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 11:46:51 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 11:46:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:46:52 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 11:46:52 GMT
EXPOSE 80
# Tue, 04 Aug 2020 11:46:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03d05372daa08e1d710fd41190c6bd10c94993ffd335b298d436793eb9773ea`  
		Last Modified: Tue, 04 Aug 2020 13:52:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b7547fc35288caef4bc14b45970f142023a3e6aa26b31327cf7ae42769166`  
		Last Modified: Tue, 04 Aug 2020 13:53:11 GMT  
		Size: 61.4 MB (61389262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb15645eb91acb34562718b3a59bcdce3b9b0b0e82bf672f3dd46c0a8a609b`  
		Last Modified: Tue, 04 Aug 2020 13:52:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e048d09c42e36fbe868a7791022f377ddc38e339cb19eb0c9088e460423c0d88`  
		Last Modified: Tue, 04 Aug 2020 13:54:02 GMT  
		Size: 18.6 MB (18606100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393c52063a6d6a12ace80d1494b85099cd2ea098326418dddb3729bdca2c6e32`  
		Last Modified: Tue, 04 Aug 2020 13:53:50 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444651384ab14107b743dbb3edfd2a685a4b7d5e3bccc9737b8cec6de409d5d0`  
		Last Modified: Tue, 04 Aug 2020 13:53:49 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cab54a663b8d92e04da2c1b771954e58dc681c3c686e41aa4e9b4552620a19`  
		Last Modified: Tue, 04 Aug 2020 13:53:53 GMT  
		Size: 10.8 MB (10840435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6658da40ca55e5ec22adc5e5a4167ffa49486c4cd1f47806907fa755556dae1`  
		Last Modified: Tue, 04 Aug 2020 13:53:47 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7484edc1a6c984ef881fc9278380c72b62ee7bb0e3d81b7144e7c3b9532abd5`  
		Last Modified: Tue, 04 Aug 2020 13:53:58 GMT  
		Size: 12.8 MB (12840083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4386f003a7760088e4cd94d5d29cf4be095b28c4f89eb631b87637b092695bb`  
		Last Modified: Tue, 04 Aug 2020 13:53:47 GMT  
		Size: 2.3 KB (2287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e463abb06940c5754391c211c302c8ad35088900779dd1d69093c48cbc2fb3`  
		Last Modified: Tue, 04 Aug 2020 13:53:47 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8220baa5becb90b645c3f9ae67d34e098ca38ce352455e23ff74141e994a536`  
		Last Modified: Tue, 04 Aug 2020 13:53:47 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; ppc64le

```console
$ docker pull php@sha256:313ee7503e06e5c6868b031fd3aeb127dd13c4c992da60206dbd5019bcf685da
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (158019612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30a79269a7517674c10fc2d2233aae201816d126f78506023f6ae343ffb0503e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:23:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 10:23:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 10:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:28:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 10:28:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 10:36:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 10:37:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 10:39:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 10:39:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 10:39:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 10:39:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 10:39:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 10:39:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 10:40:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 10:40:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 10:40:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 04 Aug 2020 10:40:16 GMT
ENV PHP_VERSION=8.0.0alpha3
# Tue, 04 Aug 2020 10:40:20 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Tue, 04 Aug 2020 10:40:24 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Tue, 04 Aug 2020 10:42:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 10:42:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 10:52:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Tue, 04 Aug 2020 10:52:38 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 10:52:48 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 10:52:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 10:52:55 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 10:52:56 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 10:52:57 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 10:53:00 GMT
EXPOSE 80
# Tue, 04 Aug 2020 10:53:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1638f5ca01b7c06ee35198f1b1e561696585b3539fbe344ccb8f1bb06499339`  
		Last Modified: Tue, 04 Aug 2020 12:35:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03053d6310ef37b9abff0a3d2fdb20a475147b623840f2c4cfe6905564ab8ac5`  
		Last Modified: Tue, 04 Aug 2020 12:35:49 GMT  
		Size: 82.3 MB (82260396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf846775f1d1a2dd29b33ef5b154abc1f5ecc19a2aeb8d2b83e56ef2ce5a428`  
		Last Modified: Tue, 04 Aug 2020 12:35:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feae99d1acb4fb8cc7aea0a40e892cf5156bceec266cd2ebe5303893fe63cafd`  
		Last Modified: Tue, 04 Aug 2020 12:36:34 GMT  
		Size: 19.8 MB (19812786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cd922f9821aebf5814f8d052f9dc4f7375f247e3c8fb4ea6fa401efcff4cb9`  
		Last Modified: Tue, 04 Aug 2020 12:36:28 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f91e3733853fecd191a2b14027843e9189b97caed5dbc4803de26a493efbbc1`  
		Last Modified: Tue, 04 Aug 2020 12:36:27 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb1fc6814aa261f38eb533f5b15b8c5c1cfeda6756812aec8d74b76effe69b`  
		Last Modified: Tue, 04 Aug 2020 12:36:28 GMT  
		Size: 10.8 MB (10843619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30bac5ff9026d6b7b7743eb07bf156f80ea76c48808470e587e183a151bb99c`  
		Last Modified: Tue, 04 Aug 2020 12:36:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de2d62976c3d84e57f6b395c6719c2cb5882262d0066a0d5f75aaabe0bf3e01`  
		Last Modified: Tue, 04 Aug 2020 12:36:28 GMT  
		Size: 14.6 MB (14579548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc45daa0d8ed2c5b6048d65f40551327f37d30065cfbd85588d3ae268d7e797`  
		Last Modified: Tue, 04 Aug 2020 12:36:24 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707794ca74aa0040b53cb80154b0c62411f765c9319a73260e5c446034ed4db`  
		Last Modified: Tue, 04 Aug 2020 12:36:24 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5880dcf25e58a47820716e8978a5a643efccea889b2a506362d049ccfbfc375`  
		Last Modified: Tue, 04 Aug 2020 12:36:25 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:rc-apache` - linux; s390x

```console
$ docker pull php@sha256:b8b513e25cf6c0d442eaf6d022a5c6a9ce8af1736f40c1f3b075b699086a0960
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132543835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb0b4a0e8a2a827b44817f339164225913d0c84e76da59af105ce7a60c4f576`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:17:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 03:17:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 03:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 03:18:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 03:18:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 03:20:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 03:20:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 03:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 03:20:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 03:20:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:20:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 03:20:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 04 Aug 2020 03:20:30 GMT
ENV PHP_VERSION=8.0.0alpha3
# Tue, 04 Aug 2020 03:20:30 GMT
ENV PHP_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz PHP_ASC_URL=https://downloads.php.net/~carusogabriel/php-8.0.0alpha3.tar.xz.asc
# Tue, 04 Aug 2020 03:20:30 GMT
ENV PHP_SHA256=83dac88c90bf47fad89bb2425d76243fa0356e462954d652893d05b9593ac6d0 PHP_MD5=
# Tue, 04 Aug 2020 03:20:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 03:20:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:22:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version
# Tue, 04 Aug 2020 03:22:26 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:22:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 03:22:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 03:22:27 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 03:22:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:22:27 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 03:22:28 GMT
EXPOSE 80
# Tue, 04 Aug 2020 03:22:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f8604b15b40b87c7c78f35c952be34d77e22c70a7a3d634af952bed77df82a`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c79c3a25fa505e04cf025f8485f429f891ecf1609983c99d0f0b81a99aa8f54`  
		Last Modified: Tue, 04 Aug 2020 03:56:16 GMT  
		Size: 64.7 MB (64706546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007fcb88e4f44656bd1669c15b17ec295337d9d3a8ac3764848b6130f737ac05`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef93b86f4a7b3b0359b5f145a6f9cfa99af8cbc9e23a11458d496d3d4902854`  
		Last Modified: Tue, 04 Aug 2020 03:56:35 GMT  
		Size: 18.5 MB (18522609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03de6a7739c46b225f487b15c9e4745f8a3360dc4d59e0c81b5659e6e209e9e`  
		Last Modified: Tue, 04 Aug 2020 03:56:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16499546079fb354707b57f0646a75ded183022339942a95fe84bcfa606be992`  
		Last Modified: Tue, 04 Aug 2020 03:56:32 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8465d91342b796d54785c426ba45d4f42d58c5b697e1495112dba0b09de5d20`  
		Last Modified: Tue, 04 Aug 2020 03:56:32 GMT  
		Size: 10.8 MB (10841655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e9ea635c9984e6f5ed8175d29fb18cc14c5e6397f439c7d26d8920787b6462`  
		Last Modified: Tue, 04 Aug 2020 03:56:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f11ff3762c7c0d1de62d538531973ae42c8e221f800f244bd13a8d60835e4a3`  
		Last Modified: Tue, 04 Aug 2020 03:56:32 GMT  
		Size: 12.8 MB (12759985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d2b22d40ead7677b5a6a10611aaca3fa289fb438d1cfa57d1722ae6669fe73`  
		Last Modified: Tue, 04 Aug 2020 03:56:30 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a89e0b0902f6a0d12ffbadeced955e1fcffd7ab3b633462821ecbdc2106849`  
		Last Modified: Tue, 04 Aug 2020 03:56:30 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236059b77aeec16a8ab4817f724d6c4ae1c27271221a510c5490d5492b6c03b8`  
		Last Modified: Tue, 04 Aug 2020 03:56:30 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
