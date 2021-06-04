## `yourls:1-apache`

```console
$ docker pull yourls@sha256:743c479d4fc96b08e389399c4ba98b4660bf1ed52c3efb04028c67d572d99d6a
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

### `yourls:1-apache` - linux; amd64

```console
$ docker pull yourls@sha256:f47c62d7debc99a5c5e2a40e41837a1f90081a3af6a0b43f80122a8204b54822
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151374807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fccb9a3d377abe4d945e688a747dafe6dd8e2f8dba1e475b593fcfed51d4ac6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 12 May 2021 12:48:33 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 18:35:45 GMT
ENV PHP_VERSION=8.0.7
# Fri, 04 Jun 2021 18:35:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Fri, 04 Jun 2021 18:35:46 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Fri, 04 Jun 2021 18:35:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 18:35:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 18:40:24 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:40:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 18:40:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 18:40:26 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 18:40:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:40:27 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 18:40:27 GMT
EXPOSE 80
# Fri, 04 Jun 2021 18:40:27 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 20:51:42 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 20:51:43 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 20:51:44 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 20:51:44 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 20:51:44 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 20:51:46 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 20:51:47 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 20:51:47 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 20:51:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 20:51:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 20:51:47 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:519598d7b82587666cbe28db2f4fdc07e27afedeb143a4b25c57665588401b5e`  
		Last Modified: Fri, 04 Jun 2021 19:37:35 GMT  
		Size: 11.1 MB (11107187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86127afe9afbf63f3442521612d91faf4039bf1a1b3f5fc0355babde3a4ab8a`  
		Last Modified: Fri, 04 Jun 2021 19:37:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3ecbff81fa432cf75a3204247b49ee0305e1fdaace32e37c523af3e85989c0`  
		Last Modified: Fri, 04 Jun 2021 19:37:35 GMT  
		Size: 14.5 MB (14490867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182b59a9cacba1a7ee7135b9711c99b3313a02bd9ae16a96915060f1406e6058`  
		Last Modified: Fri, 04 Jun 2021 19:37:31 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91763d383b593a765d25f38f3c35476b1eb7bf7a538110f0a0fbb7893cb5a2fd`  
		Last Modified: Fri, 04 Jun 2021 19:37:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea724594135ee66d8d2fbc40d7f47f5ba1571b1da5f6be6485dad8afc98111b`  
		Last Modified: Fri, 04 Jun 2021 19:37:31 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096be7d4c8288d7a36af67cd095dc321cb7900a516b9d9683b5e5eb4488e8d7`  
		Last Modified: Fri, 04 Jun 2021 20:54:44 GMT  
		Size: 690.3 KB (690304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d6eda8a24713954d546929b81ad215b4dff1efe52c70509fa813ceef466e8c`  
		Last Modified: Fri, 04 Jun 2021 20:54:44 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d786a375194343cb6a6d557a54451827ff11f52007a7204a0e4f8f578d911db9`  
		Last Modified: Fri, 04 Jun 2021 20:54:41 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001aa1f913ad81bfafdb09811047112869d3fab2a629ec134ae05205feadc803`  
		Last Modified: Fri, 04 Jun 2021 20:54:42 GMT  
		Size: 2.6 MB (2572148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d503dc8f139f03505e7a51ba21b85567daa9ec716df9b466c4dff69f85d5a44`  
		Last Modified: Fri, 04 Jun 2021 20:54:41 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ce29a61437f91d6fa2a8157612da628288ac58e7da35e9acc3b1809f309338`  
		Last Modified: Fri, 04 Jun 2021 20:54:41 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325e29fdf92a04e4ab8d2762c07c5aa3ae359f9bdcb0212056dc6c511e1070da`  
		Last Modified: Fri, 04 Jun 2021 20:54:41 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:bf66485aec3d963e42d9d535880c9428d8e5c3a1baec4537a6f197c714410443
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128955992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b9815d00b5ccc72aa7c56856e3ac811cc07ad125692ae963a437bc3c50a590`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Thu, 03 Jun 2021 22:01:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 18:53:21 GMT
ENV PHP_VERSION=8.0.7
# Fri, 04 Jun 2021 18:53:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Fri, 04 Jun 2021 18:53:22 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Fri, 04 Jun 2021 18:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 18:53:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:57:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 18:57:32 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:57:33 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 18:57:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 18:57:34 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 18:57:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:57:34 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 18:57:34 GMT
EXPOSE 80
# Fri, 04 Jun 2021 18:57:34 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 20:23:48 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 20:23:49 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 20:23:50 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 20:23:50 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 20:23:50 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 20:23:52 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 20:23:52 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 20:23:52 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 20:23:52 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 20:23:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 20:23:53 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:2b64a343b2678830f2d4ef8af99fe2abdcef1bbcdf886aff50131ee8b664844c`  
		Last Modified: Fri, 04 Jun 2021 19:20:01 GMT  
		Size: 11.1 MB (11104996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bda359c226069751602f5450ef9002b4cbc09ae145954b4a5fb4d81a12c733`  
		Last Modified: Fri, 04 Jun 2021 19:19:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf3826b5451880bf4649a3ba79ed966327f566430af2de3a02e2edafaedf0e`  
		Last Modified: Fri, 04 Jun 2021 19:20:01 GMT  
		Size: 13.2 MB (13205274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044e045c64f9af496eb1970d16a37407113bd5ddcc41082e474df74f1807ef43`  
		Last Modified: Fri, 04 Jun 2021 19:19:56 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0ac39174c6bb7a4dd7c5645c0bd12ada7700d8cd71b4a8fac1d122519e091f`  
		Last Modified: Fri, 04 Jun 2021 19:19:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a048a9861f84b91a2d03a49031792deba25c58fa99a734e85991d79aeca9f05`  
		Last Modified: Fri, 04 Jun 2021 19:19:57 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c6c00219a6e377612672f3d7b05479b46661e4eff249cdc312c95ca387867`  
		Last Modified: Fri, 04 Jun 2021 20:25:30 GMT  
		Size: 340.3 KB (340298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fbb05f31476d20f3e4625f5209ae9f48aab42d85ce19add4a4b43796748bd`  
		Last Modified: Fri, 04 Jun 2021 20:25:29 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf8622d8560dfe25a3c67c79844348d33a0305566fabd478def0b5bd17d441`  
		Last Modified: Fri, 04 Jun 2021 20:25:27 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bdfbf1daea6f0a6f120be2c89b013545eed9265182fa87ed8b2305cb741d80`  
		Last Modified: Fri, 04 Jun 2021 20:25:28 GMT  
		Size: 2.6 MB (2572152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ff6ce0205fd0b0175c3ed5a86bd4d9a96ef7ae828103c84e7141d1a39d1122`  
		Last Modified: Fri, 04 Jun 2021 20:25:27 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10bfd9edf9e11978051ba3a10de2073bec4aa4ef378a41d20cb5de481ba5d86`  
		Last Modified: Fri, 04 Jun 2021 20:25:28 GMT  
		Size: 2.0 KB (2043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17adf98427678721b87490bb1bcceef780ff696c894263d128be55240505b104`  
		Last Modified: Fri, 04 Jun 2021 20:25:27 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:d5dbf2d9bcaf899358b0d5ced7669a62625191d48d145e1b28f2f6cf6b946f5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126231079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f81b47df0a65ff0ab0c73393d10fe1fd047ce1017296faffdc7b492cd2e3f0cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Fri, 04 Jun 2021 02:52:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 04 Jun 2021 02:52:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 04 Jun 2021 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Jun 2021 02:53:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 04 Jun 2021 02:53:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 04 Jun 2021 02:57:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 04 Jun 2021 02:57:59 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 04 Jun 2021 02:58:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 04 Jun 2021 02:58:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 04 Jun 2021 02:58:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 04 Jun 2021 02:58:11 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 04 Jun 2021 02:58:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 04 Jun 2021 02:58:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 04 Jun 2021 02:58:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 04 Jun 2021 02:58:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 04 Jun 2021 02:58:12 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 02:58:12 GMT
ENV PHP_VERSION=8.0.6
# Fri, 04 Jun 2021 02:58:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 04 Jun 2021 02:58:12 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 04 Jun 2021 02:58:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 02:58:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 03:02:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 03:02:37 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 03:02:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 03:02:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 03:02:38 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 03:02:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 03:02:39 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 03:02:39 GMT
EXPOSE 80
# Fri, 04 Jun 2021 03:02:39 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 11:19:57 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 11:19:58 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 11:19:59 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 11:19:59 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 11:19:59 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 11:20:06 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 11:20:06 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 11:20:07 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 11:20:07 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 11:20:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 11:20:07 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171c90793ddc5dae10b5c09628ea9b2b65ce602c0cad3408f3fda800f5aec8db`  
		Last Modified: Fri, 04 Jun 2021 06:25:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd764830a721fbbba2d34b9d434e911649e4dda208d2aedf658b0241ebbd20bb`  
		Last Modified: Fri, 04 Jun 2021 06:25:14 GMT  
		Size: 59.5 MB (59512543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562a2feae8887f32895169b8cfd6656dd3348f84304c15d0c88de4571663a9a`  
		Last Modified: Fri, 04 Jun 2021 06:25:00 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacabafa2c464cd565f7b99d5b1ba54abcb62c63dc9f18f10c205174a1f400ec`  
		Last Modified: Fri, 04 Jun 2021 06:26:37 GMT  
		Size: 17.5 MB (17481699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0feab867e145045d2c3a7d4e52160982c31abba933728157de7f6ce445dd5`  
		Last Modified: Fri, 04 Jun 2021 06:26:29 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec4e0f87c2b982419d3d121057425a4093273669bcac10622e3982e5cc1b44`  
		Last Modified: Fri, 04 Jun 2021 06:26:28 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04439bafeae14743dde8017d393cd4220960805120184f368df487b080f24bb`  
		Last Modified: Fri, 04 Jun 2021 06:26:29 GMT  
		Size: 11.1 MB (11100513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547fb1b32d0d3b4b807673f92128b2d4c1bce6954233e08f6d32c168be953a4a`  
		Last Modified: Fri, 04 Jun 2021 06:26:26 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac5c678b9b3f0f07cbad4bfe125f66c33f057f468b7d5562cf85854a1d0d275`  
		Last Modified: Fri, 04 Jun 2021 06:26:30 GMT  
		Size: 12.5 MB (12501428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edcd27f9183227d629c9e6c43767c849d0e4f9cd2fd25a1aa01aa62ba8b768`  
		Last Modified: Fri, 04 Jun 2021 06:26:26 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee4050bf578f99d2c79f092f167acac58f631df1c8ad9f8444d5b1cdb1e32ff`  
		Last Modified: Fri, 04 Jun 2021 06:26:26 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c74f7e4c84090c42c3142890e502d44a021168237c97e06b7843df7df0828`  
		Last Modified: Fri, 04 Jun 2021 06:26:26 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c3cf335f27bc1f38fa700dc6ece446169f046a144b72fc7b773dbf8d0c239`  
		Last Modified: Fri, 04 Jun 2021 11:22:34 GMT  
		Size: 306.9 KB (306858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fe791d4594ca9d14a66da3ff0c57dea03960de971210ee1ceb8081df1a5aed`  
		Last Modified: Fri, 04 Jun 2021 11:22:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd89be200e62667d59bf70c9103ae5419b641d0fc931349330fc634d112d57f`  
		Last Modified: Fri, 04 Jun 2021 11:22:31 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7046cc201bcd34357c69dc1fa4b3a8528e8224f0cdb4f012f8ec6fdea1a2e52b`  
		Last Modified: Fri, 04 Jun 2021 11:22:32 GMT  
		Size: 2.6 MB (2572151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a9698c1550f0d43c68278a378290a1d1a2ee12ed84b474505c4877e8425b`  
		Last Modified: Fri, 04 Jun 2021 11:22:31 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf398dc7304e85ed9f0995ac97a233fd6780fed9825ab767db59ec8490b2e2`  
		Last Modified: Fri, 04 Jun 2021 11:22:31 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89f24e377be0385d3a5a8f037c300d84852d85632b5e76cb3614a167f35cf9d`  
		Last Modified: Fri, 04 Jun 2021 11:22:31 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:1cbee11aa418bfab1cf7b41f5f69a996cde8fc7e74064e3132450ca656589b2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142807193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7a4b8b6b2d49735b1c6665c18b67534a3ca890aa299a5605a0a3b272be7387`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Fri, 04 Jun 2021 00:31:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 00:31:11 GMT
ENV PHP_VERSION=8.0.6
# Fri, 04 Jun 2021 00:31:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 04 Jun 2021 00:31:12 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 04 Jun 2021 00:31:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 00:31:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:34:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 00:34:36 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:34:37 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 00:34:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 00:34:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 00:34:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 00:34:38 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 00:34:38 GMT
EXPOSE 80
# Fri, 04 Jun 2021 00:34:38 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 06:53:33 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 06:53:34 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 06:53:35 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 06:53:35 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 06:53:35 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 06:53:37 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 06:53:37 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 06:53:37 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 06:53:37 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 06:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 06:53:38 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:bcacc040b1492d7e22a474325175954e529751f79b2b853ad8f60c69d767786e`  
		Last Modified: Fri, 04 Jun 2021 02:42:28 GMT  
		Size: 11.1 MB (11101175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068a8271d3cc7fa4ac50bff80e9a8e9269d35b941ad45fb3de5dd9e0e187b7f`  
		Last Modified: Fri, 04 Jun 2021 02:42:24 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d985bf1145352a2ced842076e58babf601cc78b09ff053a9662daac4120dc`  
		Last Modified: Fri, 04 Jun 2021 02:42:27 GMT  
		Size: 13.9 MB (13923855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f04cb1486ac2700117e321e6cbf55bb5e2c2ff0468ec3b0b223c6a97b7af864`  
		Last Modified: Fri, 04 Jun 2021 02:42:24 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4077c8912286e105ab081c6cac91c70ad10c6fed3dc290adcebee5536f6324`  
		Last Modified: Fri, 04 Jun 2021 02:42:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5bea2a002070442bd0731758c9acb89e15b830de17b4e9b7ea929233849a0c`  
		Last Modified: Fri, 04 Jun 2021 02:42:24 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6b836099ee3550b8e56627179e706931e9873ee87efcaca000ed79c33c398a`  
		Last Modified: Fri, 04 Jun 2021 06:55:41 GMT  
		Size: 352.9 KB (352907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c8444b85d184860cbbacf3bd65fa943840416946515a4293c802858ba6aba`  
		Last Modified: Fri, 04 Jun 2021 06:55:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca4e6da265ed9d1728559a0a4afa2b854e71d5761ec7f65a131ef8c2a9da137`  
		Last Modified: Fri, 04 Jun 2021 06:55:38 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f2472ec2581b9c92846301acdc5d1729d26dafd6530fe06183468b1f7f4f7e`  
		Last Modified: Fri, 04 Jun 2021 06:55:39 GMT  
		Size: 2.6 MB (2572153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce71af311a3914af8321dec956c0472a750c77c75456c0935232b5b05bd421bc`  
		Last Modified: Fri, 04 Jun 2021 06:55:38 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3fc92750e29b00441b4197ef810b0f6240279bf76db3d5449c03bcef1e4cb4`  
		Last Modified: Fri, 04 Jun 2021 06:55:38 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a835096511b15eb34da9a52d4e82a2f06e4d62df8934d7c4273977b93760a6`  
		Last Modified: Fri, 04 Jun 2021 06:55:38 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; 386

```console
$ docker pull yourls@sha256:ddcbe714d1faa901c15236048a85aef0d8d4916af2878ae345ffa88318e6481b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.7 MB (156675761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574b1a21db04e1440b88045085168d845da04ab8da81f1f7d540623d249def5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 12 May 2021 10:37:20 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 12 May 2021 10:37:20 GMT
ENV PHP_VERSION=8.0.6
# Wed, 12 May 2021 10:37:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Wed, 12 May 2021 10:37:21 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Wed, 12 May 2021 10:37:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 May 2021 10:37:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 May 2021 10:44:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 May 2021 10:44:35 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 12 May 2021 10:44:37 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 May 2021 10:44:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 May 2021 10:44:37 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 May 2021 10:44:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 May 2021 10:44:38 GMT
WORKDIR /var/www/html
# Wed, 12 May 2021 10:44:38 GMT
EXPOSE 80
# Wed, 12 May 2021 10:44:38 GMT
CMD ["apache2-foreground"]
# Wed, 12 May 2021 22:07:04 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 May 2021 22:07:05 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 May 2021 22:07:06 GMT
RUN a2enmod rewrite expires
# Wed, 12 May 2021 22:07:06 GMT
ENV YOURLS_VERSION=1.8.1
# Wed, 12 May 2021 22:07:07 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Wed, 12 May 2021 22:07:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 May 2021 22:07:09 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Wed, 12 May 2021 22:07:09 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Wed, 12 May 2021 22:07:09 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 12 May 2021 22:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 22:07:10 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:c4f17e8b2fac815bb78259262fe7fb98ba8b61dd50d61e89d98b3a2f6d923c4f`  
		Last Modified: Wed, 12 May 2021 12:27:12 GMT  
		Size: 11.1 MB (11101743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746e0fd7bd284fae3c5af49f1cc74f616b749eecc7bda2470ed01745c2e2006d`  
		Last Modified: Wed, 12 May 2021 12:27:08 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77847a893d3a2b7075d6d491f4462c133092522067ebbace3e38fa62e13b5ebe`  
		Last Modified: Wed, 12 May 2021 12:27:13 GMT  
		Size: 14.5 MB (14479248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780aa56639e0330c27467bdd8cf3efc3a32d29d4ae84e8540bfe9930d304ed36`  
		Last Modified: Wed, 12 May 2021 12:27:08 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40578ac3d60e54fdd75968f8ab486de676e679eaffc5cf78610a3de173f8058f`  
		Last Modified: Wed, 12 May 2021 12:27:08 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14646fb478fe44be6cfd8323332a72e771a1ad969f386bbfad13adc2d4447fc`  
		Last Modified: Wed, 12 May 2021 12:27:08 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a57bcff1ea28bd6c5808ca4fcbd293917c51603d3e4a8a6eab55177f13b9f6`  
		Last Modified: Wed, 12 May 2021 22:09:59 GMT  
		Size: 372.6 KB (372599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f60df8b4c7ec9510b0a6d4ffaff8359385681690df58bc67ad35fc454509f`  
		Last Modified: Wed, 12 May 2021 22:09:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf36fe774023decec98f7fcf7b6adbbe543a8383737b150cff28a725faebec7f`  
		Last Modified: Wed, 12 May 2021 22:09:56 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac59fbefd106c0f0bb7b971a8cef32bd9189db9fbb36b0e59a7d375aaf21cd`  
		Last Modified: Wed, 12 May 2021 22:09:57 GMT  
		Size: 2.6 MB (2572153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b758bb956b95dd1e5d84b2296102d15a561785b7db98736407ae4caa7bf54d1`  
		Last Modified: Wed, 12 May 2021 22:09:56 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4649c44ef7811f16b604564f42afb7c25db3c986c23ac8bf5c1a35f61d8fe1be`  
		Last Modified: Wed, 12 May 2021 22:09:56 GMT  
		Size: 2.0 KB (2044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6619168ef1ee6d85db8dd2f000357f97aeb4b46170a083715be9ab42d9dcbef2`  
		Last Modified: Wed, 12 May 2021 22:09:56 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; mips64le

```console
$ docker pull yourls@sha256:e9b6f52588f93aee9b7f9b98513ab5cc5e080beb0fa751ed5bd05e925120a20a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133294421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d459107495425a03923006dba1817b7d487c951f4d2250aab8e2655033941110`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 12 May 2021 10:31:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 19:20:20 GMT
ENV PHP_VERSION=8.0.7
# Fri, 04 Jun 2021 19:20:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Fri, 04 Jun 2021 19:20:20 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Fri, 04 Jun 2021 19:20:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 19:20:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 19:32:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 19:32:52 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 19:32:54 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 19:32:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 19:32:54 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 19:32:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 19:32:55 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 19:32:55 GMT
EXPOSE 80
# Fri, 04 Jun 2021 19:32:56 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 20:38:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 20:38:16 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 20:38:18 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 20:38:18 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 20:38:19 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 20:38:22 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 20:38:23 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 20:38:23 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 20:38:24 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 20:38:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 20:38:24 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:41fe46bf9a78fccb66bf61214460f84173fd3ab2c155618dc81b7be903b5259d`  
		Last Modified: Fri, 04 Jun 2021 20:02:26 GMT  
		Size: 11.1 MB (11104288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf37639066f27b211965a152a66beccac73ac262259ab4c72f5e783bdd54595`  
		Last Modified: Fri, 04 Jun 2021 20:02:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f192ee753c4227fc452dc1dbacd8319f24fe56c8f149d4a7bbbe19af40b7eaf1`  
		Last Modified: Fri, 04 Jun 2021 20:02:31 GMT  
		Size: 13.4 MB (13430879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21efd4c6e326bba7c6eaf5707424a488206ce792b2403433ebd793479851c9e9`  
		Last Modified: Fri, 04 Jun 2021 20:02:19 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06aa93b923b47309c656b249a1112ae4b05b2b54292312300fbaed596951281a`  
		Last Modified: Fri, 04 Jun 2021 20:02:20 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db519a70b4dfb83ff6040ae49cfaf117aedea64ef4aaae630899a9db347c8a14`  
		Last Modified: Fri, 04 Jun 2021 20:02:20 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5ef147585f8e5dc6547815ef6a135a88ddcde74920bb0bb594b4947ac913fb`  
		Last Modified: Fri, 04 Jun 2021 20:40:36 GMT  
		Size: 348.9 KB (348931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713492e6fbe5827976d7c786b3bb2673a12c8c25aa57ab1deae7824e8ab35bba`  
		Last Modified: Fri, 04 Jun 2021 20:40:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcc1423d1e598989be1878b4869b254e9a726c4902377c7d5861aa50a729d1b`  
		Last Modified: Fri, 04 Jun 2021 20:40:33 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf28fbee23fb204133873a047623391099c700de0dd3b4b35736d3cadf79f75`  
		Last Modified: Fri, 04 Jun 2021 20:40:35 GMT  
		Size: 2.6 MB (2572126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803e61368de4edd43d3cff9e8919de4294cd0d660119843aab1dacab2438447c`  
		Last Modified: Fri, 04 Jun 2021 20:40:33 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c5b36c4a879284ac2b0df4657153eff5ca6d9d79f572da070862f17c3d91a`  
		Last Modified: Fri, 04 Jun 2021 20:40:33 GMT  
		Size: 2.0 KB (2044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc352605d91a339339cc3000d1f3a40a40b8002367466d9ddbe20a4fdba4f05`  
		Last Modified: Fri, 04 Jun 2021 20:40:33 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:25677ff02c7b273bc051265e8d867298537991202081342449d26bcfd9844eae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (161963132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100685714ce6a532af7a84da9ffa85818587480470b823bee06c0e070fdb08e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 12 May 2021 14:59:50 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 18:26:10 GMT
ENV PHP_VERSION=8.0.7
# Fri, 04 Jun 2021 18:26:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Fri, 04 Jun 2021 18:26:23 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Fri, 04 Jun 2021 18:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 18:28:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:35:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 18:35:16 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:35:26 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 18:35:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 18:35:36 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 18:35:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:35:47 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 18:35:53 GMT
EXPOSE 80
# Fri, 04 Jun 2021 18:36:03 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 20:15:45 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 20:15:59 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 20:16:11 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 20:16:15 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 20:16:21 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 20:16:40 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 20:16:42 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 20:16:44 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 20:16:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 20:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 20:16:58 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:d72cd19bc639393c875c5125ed109d94174a78a9da2e471eb6d4d1f4a61e09d0`  
		Last Modified: Fri, 04 Jun 2021 19:21:36 GMT  
		Size: 11.1 MB (11107175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66371bc2621d2b115aa59dc5e8d0f7688fa939a67e3181c23635956c14be685`  
		Last Modified: Fri, 04 Jun 2021 19:21:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fa1c9c98eef9c024a546dff2ae5ec31297cb737423a49374c5f281b9be276`  
		Last Modified: Fri, 04 Jun 2021 19:21:34 GMT  
		Size: 15.2 MB (15210908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d4b0051e99aca2975df554d03a60b428f6e5f84fb337942220ceaff7864a83`  
		Last Modified: Fri, 04 Jun 2021 19:21:30 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3a34242642814bca7ad7e9b1496ed96c17cc5a3ddafdc5d386477fba18a96`  
		Last Modified: Fri, 04 Jun 2021 19:21:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c7fb86cdf0114858bec4787978cae2ec24a697d2d0dfd95295e5268f50e077`  
		Last Modified: Fri, 04 Jun 2021 19:21:31 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671782211ba2b17b6a7805b530c441a4427a094279899f851eae4c8284a6cb00`  
		Last Modified: Fri, 04 Jun 2021 20:22:06 GMT  
		Size: 401.4 KB (401438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35426b47ec981034652282158f042b19152ff998166b405c03ab19be20a99a82`  
		Last Modified: Fri, 04 Jun 2021 20:22:05 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e88cb02fb510258d08c2446dc91352dedc950ac01d99a92f0ae79a2f67b166`  
		Last Modified: Fri, 04 Jun 2021 20:22:02 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961739b2dad65d9e6a1511b6119c3ee16fcae7060a9906c8144381333aed87a3`  
		Last Modified: Fri, 04 Jun 2021 20:22:02 GMT  
		Size: 2.6 MB (2572152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a033aee1c3f762f5bab3999c2ae09d78fd240cedaeffd8eb6858c7e3a5ce43`  
		Last Modified: Fri, 04 Jun 2021 20:22:01 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc727097fa4b411f4f3038f05b06263580605eaa9a86244017ba07b5072a249`  
		Last Modified: Fri, 04 Jun 2021 20:22:01 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9379e06b7e3a6b0a3b92eb5600d8408bd5ddb6368bb66fec46b450ec01cf3884`  
		Last Modified: Fri, 04 Jun 2021 20:22:02 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; s390x

```console
$ docker pull yourls@sha256:ecce1096f54b2388c03d8bc8c5b20fa2843aa7c0c875d79422ac84a8235d43ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136393881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:853ccd6b0c03cf3e22d127fe945900c2713248d31e6b69028bda7a302d29f712`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 12 May 2021 04:45:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 18:50:05 GMT
ENV PHP_VERSION=8.0.7
# Fri, 04 Jun 2021 18:50:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Fri, 04 Jun 2021 18:50:06 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Fri, 04 Jun 2021 18:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Jun 2021 18:50:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:54:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 18:54:41 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:54:43 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 18:54:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 18:54:44 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Jun 2021 18:54:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Jun 2021 18:54:46 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 18:54:46 GMT
EXPOSE 80
# Fri, 04 Jun 2021 18:54:47 GMT
CMD ["apache2-foreground"]
# Fri, 04 Jun 2021 20:03:40 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 04 Jun 2021 20:03:42 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Jun 2021 20:03:43 GMT
RUN a2enmod rewrite expires
# Fri, 04 Jun 2021 20:03:44 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 04 Jun 2021 20:03:45 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 04 Jun 2021 20:03:48 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 04 Jun 2021 20:03:49 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 04 Jun 2021 20:03:49 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 04 Jun 2021 20:03:49 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 04 Jun 2021 20:03:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Jun 2021 20:03:50 GMT
CMD ["apache2-foreground"]
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
	-	`sha256:b1e014e668c2792b82a55f60f5660702f4b3fe5630d2a45ae45b9d6faec01d81`  
		Last Modified: Fri, 04 Jun 2021 19:30:04 GMT  
		Size: 11.1 MB (11105453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e074f7d48acee495e9a3584ea183ab00630bf09de0351992d2e5394e5bee22`  
		Last Modified: Fri, 04 Jun 2021 19:29:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c721c56df01ebde81e36b02a4436da9de3daa5f1705273a7a860a9be2e1073f`  
		Last Modified: Fri, 04 Jun 2021 19:29:59 GMT  
		Size: 13.4 MB (13360566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381ecff87a029a209adce54e1d0de3d1d60450854fbc319aef679784dfb6903`  
		Last Modified: Fri, 04 Jun 2021 19:29:56 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088d4f58e8a7697d384d0d8710bc73a80226e19263af6976b836e256be0b7d7a`  
		Last Modified: Fri, 04 Jun 2021 19:29:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4988f1ca8dca64d338acb84f14bd707d55863296d7fe7bdaafe9ba28f33ce74`  
		Last Modified: Fri, 04 Jun 2021 19:29:56 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd91daf3284c0bc05b497460652404c878f69113893720d28d4a5483c1bb507`  
		Last Modified: Fri, 04 Jun 2021 20:06:45 GMT  
		Size: 350.7 KB (350667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39bcf9f3122765bdd05694ac5757132b3a5fe3063117aedd96d44ecdad7766a`  
		Last Modified: Fri, 04 Jun 2021 20:06:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddd72a18dc13821f92b3bb59e0ab60744ca4b810a014deab166b157c43d6a4`  
		Last Modified: Fri, 04 Jun 2021 20:06:43 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7134bdf64a60fb1f67015ffd68e13547056ead04aaa288ed18c72f4e51d414`  
		Last Modified: Fri, 04 Jun 2021 20:06:44 GMT  
		Size: 2.6 MB (2572151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79928cee3b56113727fbb26f19752e427f7bbbd17782239600192b342e5514f7`  
		Last Modified: Fri, 04 Jun 2021 20:06:43 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e8e857ca0b1acfb4e4cd2e57e7abc2899cd29b14b31df0e0de64e85bbbfade`  
		Last Modified: Fri, 04 Jun 2021 20:06:43 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac112472304d7bf1aad273e854ac0d0fba0918c684b8627c923fffac90b8f85a`  
		Last Modified: Fri, 04 Jun 2021 20:06:43 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
