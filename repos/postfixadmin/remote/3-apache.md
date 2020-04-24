## `postfixadmin:3-apache`

```console
$ docker pull postfixadmin@sha256:e4ee21477bdde1399c924a8026b3a92cfc41deac3a504651931aff8169426561
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postfixadmin:3-apache` - linux; amd64

```console
$ docker pull postfixadmin@sha256:f4f2f090cc289486958744ecca7a41185759e37b7cc4479cc260707c78e5935c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.9 MB (150937971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc26d686adbb182375858cf420915fe9b94cb1ac3e03e94c7ad207de12fedaab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:34:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 16:34:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 16:34:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 16:34:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 16:34:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 16:41:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 16:41:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 16:41:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 16:41:26 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 16:41:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 16:41:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 16:41:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 16:41:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 16:41:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 16:41:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 17:07:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Apr 2020 17:07:32 GMT
ENV PHP_VERSION=7.3.17
# Thu, 23 Apr 2020 17:07:33 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 17:07:33 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 23 Apr 2020 17:07:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 17:07:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:11:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 17:11:29 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:11:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 17:11:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 17:11:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 17:11:31 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 17:11:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:11:31 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 17:11:32 GMT
EXPOSE 80
# Thu, 23 Apr 2020 17:11:32 GMT
CMD ["apache2-foreground"]
# Fri, 24 Apr 2020 12:19:58 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 24 Apr 2020 12:20:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:20:32 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 12:20:32 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 12:20:32 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 12:20:32 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 12:20:32 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 24 Apr 2020 12:20:33 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 24 Apr 2020 12:20:34 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 24 Apr 2020 12:20:35 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:20:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:20:35 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4504446071184d4707bc1b754311b73a078008c3d1c64b7c3603e062f9e826`  
		Last Modified: Thu, 23 Apr 2020 18:46:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d55b89827dff29b49f86cebc978eddb06ffdf89e9675cc9e43e76939a1a3cd`  
		Last Modified: Thu, 23 Apr 2020 18:46:38 GMT  
		Size: 76.7 MB (76651558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf7f8bea876f55a2bbbf9e69e2190755e54d4dfc340c16418a66593e8f0cc61`  
		Last Modified: Thu, 23 Apr 2020 18:46:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ecb6839daa3e8fbc774a09c24e2895ec6e34909e6fc23b8807ac17d8b9eeae`  
		Last Modified: Thu, 23 Apr 2020 18:46:57 GMT  
		Size: 18.7 MB (18675941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94884188472ce2d3b20f61af5dbca21045fed141f0ba1871e57d6f80c813cd8a`  
		Last Modified: Thu, 23 Apr 2020 18:46:53 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3e02b2816773a41431e9fab79ae0e94b8e44c701685d52e89174d0ebe70842`  
		Last Modified: Thu, 23 Apr 2020 18:46:53 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24da3148e7e6cb50dcebfad092cbe7ab9abdafaf4b2f91b92999a8b8318f888c`  
		Last Modified: Thu, 23 Apr 2020 18:48:19 GMT  
		Size: 12.5 MB (12454682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b41fad541f40cec4dd53a77922fa1b6a8c5e0b6226a37bfb0305f6eb41f23a8`  
		Last Modified: Thu, 23 Apr 2020 18:48:17 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf4d822b25e881858974ef05d5237438ea75e79629228030993e01d8685cf3a`  
		Last Modified: Thu, 23 Apr 2020 18:48:20 GMT  
		Size: 14.1 MB (14057004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e69fc8086e416fa935d708d5196b6b9ffca7356ce0ffb52a644a14260c1a391`  
		Last Modified: Thu, 23 Apr 2020 18:48:16 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f2bc770a9534802c12c23068fe04d04b7b84b7ed4ebdd62b2ece80e09cc02f`  
		Last Modified: Thu, 23 Apr 2020 18:48:16 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c38040e6c74036e61689bf9d60353a9abee8bb7e7b6dec86b59614773f0b44e`  
		Last Modified: Thu, 23 Apr 2020 18:48:17 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c94a258a01539abbb713e675bcf397e02201832c7be08b9b96da243c958a548`  
		Last Modified: Thu, 23 Apr 2020 18:48:17 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0b2bd87342b5082fccd7ebe9e79fac92174948f064854b6514c8d5732385a2`  
		Last Modified: Fri, 24 Apr 2020 12:21:34 GMT  
		Size: 650.9 KB (650902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945dcf3ebaafcf03230fa6fd1fbbc8b6f8934939fadd4a1e040080a96ddab0c6`  
		Last Modified: Fri, 24 Apr 2020 12:21:33 GMT  
		Size: 8.2 KB (8227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cda67a02181f6062bc780eab8de872c865d00de6d4c1fc408acd2789e8fa54`  
		Last Modified: Fri, 24 Apr 2020 12:21:34 GMT  
		Size: 1.3 MB (1334614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce1f3b82d8841cd4ffdca5f91bcec53cbf56c775b638f123f4d129dc8ebae8a`  
		Last Modified: Fri, 24 Apr 2020 12:21:34 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; arm variant v5

```console
$ docker pull postfixadmin@sha256:c9dbc6dcd45e07c4582138067093a08ca2737d231d20a483c36eb26dbed8293d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129148184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7b77441b45d39bc1370f71ff42b88008f2f0f53d0e8f7b3b6b33f5cfd52c00`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 05:05:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 05:05:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 05:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 05:06:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 05:06:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 05:10:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 05:10:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 05:10:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 05:10:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 05:10:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 05:10:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 05:10:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 05:11:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 05:11:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 05:11:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 05:27:22 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Apr 2020 05:27:23 GMT
ENV PHP_VERSION=7.3.17
# Thu, 23 Apr 2020 05:27:23 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 05:27:25 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 23 Apr 2020 05:27:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 05:27:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 05:30:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 05:31:01 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 05:31:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 05:31:07 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 05:31:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 05:31:09 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 05:31:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 05:31:12 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 05:31:13 GMT
EXPOSE 80
# Thu, 23 Apr 2020 05:31:14 GMT
CMD ["apache2-foreground"]
# Thu, 23 Apr 2020 12:07:48 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 23 Apr 2020 12:09:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 12:09:08 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Thu, 23 Apr 2020 12:09:09 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 23 Apr 2020 12:09:09 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Thu, 23 Apr 2020 12:09:10 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 23 Apr 2020 12:09:11 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 23 Apr 2020 12:09:13 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 23 Apr 2020 12:09:16 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 23 Apr 2020 12:09:17 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Thu, 23 Apr 2020 12:09:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 23 Apr 2020 12:09:19 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a265de7879713459cf6e6045e802665b84c49dcb7194d42e80f713168a926d4`  
		Last Modified: Thu, 23 Apr 2020 06:32:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710cdb8f85f5abf4fda742431a0310421e7bd540337a4d831a04c9da4f000b2e`  
		Last Modified: Thu, 23 Apr 2020 06:33:06 GMT  
		Size: 58.8 MB (58799213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36a8c43726552051e04d6641b87a0c8dd7104c18f21f0b0a2f06ed6d5e03377`  
		Last Modified: Thu, 23 Apr 2020 06:32:43 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47e3b4a8efcd60aaee6d37992bab4f13d460aaf38b73cdd30a6d76f99d21c8`  
		Last Modified: Thu, 23 Apr 2020 06:34:02 GMT  
		Size: 18.0 MB (18024804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc537d4bdd514646a167fc552d70b3fc62700d1466708f49dd826723aefb151`  
		Last Modified: Thu, 23 Apr 2020 06:33:55 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74bd7696ab34d6970527a338bbceeea2763f61f021062e941a73a963ce26e45`  
		Last Modified: Thu, 23 Apr 2020 06:33:56 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937832f18ee06437073e86d6402655e9ee89331546b1d769f778b024d390e3b`  
		Last Modified: Thu, 23 Apr 2020 06:36:20 GMT  
		Size: 12.5 MB (12452845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3031835778e053ea7e9c35bdfaf09002513f8abeea109524ce20b4042d3958b4`  
		Last Modified: Thu, 23 Apr 2020 06:36:16 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e162ba77749c0b6e66f08b006e636bb4a8a17c4a090b0a8faf27c74f1baffbc6`  
		Last Modified: Thu, 23 Apr 2020 06:36:19 GMT  
		Size: 13.1 MB (13070793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fabe289bcbdb6303697cbc5c53913a0525c7ecb3d78fc8254471c3814bd982d`  
		Last Modified: Thu, 23 Apr 2020 06:36:14 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba635d81e8b70f75294a69d06fffb394472037e3887d7754cf11ebcde905ca`  
		Last Modified: Thu, 23 Apr 2020 06:36:14 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6243cbad5739fc59d0361fc5265c82da559a45aec5d8f34ed8520882fd419b23`  
		Last Modified: Thu, 23 Apr 2020 06:36:14 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af320f8e5849dc24b58a58122e5a1761b21e0d137ac7e78346e76463af39c2f9`  
		Last Modified: Thu, 23 Apr 2020 06:36:14 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14754fc7684d461a20652ea7bc7cfbc975ca8c100ffe1e7af7119875ce7ac68`  
		Last Modified: Thu, 23 Apr 2020 12:11:17 GMT  
		Size: 614.4 KB (614426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dda19618a4e95a316fc9c8013d61930c4059f49ec53f32359146db1f38522c`  
		Last Modified: Thu, 23 Apr 2020 12:11:17 GMT  
		Size: 8.2 KB (8226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab4e233750026b36a472cffffc91112489f154c8e033fc9e7e0a46f2195f20b`  
		Last Modified: Thu, 23 Apr 2020 12:11:17 GMT  
		Size: 1.3 MB (1334644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d5810b09084c2c02c3d6f2e94790a20c422adb453e565b1aeaccd7a5088fed`  
		Last Modified: Thu, 23 Apr 2020 12:11:17 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:6683d41da9b56c004ce12470e08e1d1988fecb0f21e627aa3e4f9d7c6cc4c77f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126460842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a439aa1c60b34ada4bf3d6b6d90574d0913395c50bdecb05841cf91b6c6634e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Fri, 24 Apr 2020 08:57:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 24 Apr 2020 08:57:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 24 Apr 2020 08:57:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 08:57:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 08:57:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 09:01:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 24 Apr 2020 09:01:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 24 Apr 2020 09:01:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 24 Apr 2020 09:02:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 24 Apr 2020 09:02:05 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 24 Apr 2020 09:02:05 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 24 Apr 2020 09:02:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 24 Apr 2020 09:02:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 09:02:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 09:02:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 09:34:25 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 24 Apr 2020 09:34:25 GMT
ENV PHP_VERSION=7.3.17
# Fri, 24 Apr 2020 09:34:26 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Fri, 24 Apr 2020 09:34:27 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Fri, 24 Apr 2020 09:34:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Apr 2020 09:34:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:37:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Apr 2020 09:37:33 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:37:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Apr 2020 09:37:39 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 24 Apr 2020 09:37:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Apr 2020 09:37:40 GMT
STOPSIGNAL SIGWINCH
# Fri, 24 Apr 2020 09:37:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:37:41 GMT
WORKDIR /var/www/html
# Fri, 24 Apr 2020 09:37:42 GMT
EXPOSE 80
# Fri, 24 Apr 2020 09:37:42 GMT
CMD ["apache2-foreground"]
# Fri, 24 Apr 2020 19:13:36 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 24 Apr 2020 19:14:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 19:14:38 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 19:14:39 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 19:14:39 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 19:14:40 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 19:14:41 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 24 Apr 2020 19:14:43 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 24 Apr 2020 19:14:46 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 24 Apr 2020 19:14:47 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:14:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:14:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f226b25862554006e56e97824faf9ba02bccdf2ecc2fdd30bb5b7f4619213354`  
		Last Modified: Fri, 24 Apr 2020 11:13:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d00b13e2f95b0ce7abb5b67c563d0ff2829359ecfa094f0fda731c40da1e`  
		Last Modified: Fri, 24 Apr 2020 11:13:57 GMT  
		Size: 59.5 MB (59501349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe33b7ba1f364ebeff5d799606435019145f125dd9f627718c2526f5c08726b0`  
		Last Modified: Fri, 24 Apr 2020 11:13:39 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f073aea4e3b1432422f06c950086e5f496493222ed92a187e1129dc20a00a172`  
		Last Modified: Fri, 24 Apr 2020 11:14:51 GMT  
		Size: 17.5 MB (17482036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fef6916908e53031c15629ad04ebc4adac43babef20008079fa1c18c00d8f47`  
		Last Modified: Fri, 24 Apr 2020 11:14:46 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09acc7ff9bc72c3ed202cd5b5a9ea606aff1b84967aa950e8ee58eadfedb0ff3`  
		Last Modified: Fri, 24 Apr 2020 11:14:45 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5634f291e53874d85cfd77cf79d494f6a16a784e095be12cf2f840062357342`  
		Last Modified: Fri, 24 Apr 2020 11:20:00 GMT  
		Size: 12.5 MB (12452870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498bcc507fedefb94a9cc1a4187e7198cd38c274b3cf779aa3e7ecf18f17c2cb`  
		Last Modified: Fri, 24 Apr 2020 11:19:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee207636376737e916a8b3f913fb9d50ec6930f800bf7c3679320dc50705a5b0`  
		Last Modified: Fri, 24 Apr 2020 11:19:59 GMT  
		Size: 12.4 MB (12370883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7dfcbbfc36cd1c2b3caa08a37eb12b9a0cd4864745cf8679e085af77f7ad8d`  
		Last Modified: Fri, 24 Apr 2020 11:19:56 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0441f801761a063de2281c8d0250f9b138833295536273805f2c2d18ddfcbd`  
		Last Modified: Fri, 24 Apr 2020 11:19:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b0bd4d0b36ec79a3f834209a4b814ef0ebf3e85e4bc4acb7331cb5f051a110`  
		Last Modified: Fri, 24 Apr 2020 11:19:55 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7035e4d2c092cc87b5facbb5ef8fc1fccc0e4d76ef34beaa89e599df42bb866`  
		Last Modified: Fri, 24 Apr 2020 11:19:56 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a215ada8ea2e3491f5c644cc8793233e7f8f489c51e123307c937470988d1734`  
		Last Modified: Fri, 24 Apr 2020 19:17:43 GMT  
		Size: 598.6 KB (598554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fce88c21d63dc4684a4b3cf5aae0c8f550fa91ab03f8dc4a9efa150c7ab5d25`  
		Last Modified: Fri, 24 Apr 2020 19:17:43 GMT  
		Size: 8.2 KB (8227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896a41c11506382895e652fa9b855ce83bc4e8f7606786863d59648375fa435`  
		Last Modified: Fri, 24 Apr 2020 19:17:43 GMT  
		Size: 1.3 MB (1334648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7271c7c20c8697b66ed0002ad26a00441165c414a354c0eefcaea8aaca5522`  
		Last Modified: Fri, 24 Apr 2020 19:17:43 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:845f243c34342b8d41ede8f472765d51c07077b72226c7ffddececed5f0c49fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (142958204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5ecb3ae7c1cb2f6b4e9d252b366cf08f854049e0be0dcc4ec6326baf37a0e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:09:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 16:09:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 16:10:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 16:10:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 16:10:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 16:16:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 16:16:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 16:16:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 16:16:48 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 16:16:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 16:16:53 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 16:16:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 16:16:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 16:16:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 16:16:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 16:42:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Apr 2020 16:42:34 GMT
ENV PHP_VERSION=7.3.17
# Thu, 23 Apr 2020 16:42:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 16:42:36 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 23 Apr 2020 16:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 16:42:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:47:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 16:47:33 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:47:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 16:47:38 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 16:47:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 16:47:40 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 16:47:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:47:41 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 16:47:41 GMT
EXPOSE 80
# Thu, 23 Apr 2020 16:47:42 GMT
CMD ["apache2-foreground"]
# Fri, 24 Apr 2020 02:24:06 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 24 Apr 2020 02:25:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 02:25:22 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 02:25:23 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 02:25:24 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 02:25:25 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 02:25:26 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 24 Apr 2020 02:25:29 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 24 Apr 2020 02:25:33 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 24 Apr 2020 02:25:34 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:25:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:25:36 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00aeccd126509e0b42d6cba92126cce7c342206083cc40a285bd447cf1f2d46`  
		Last Modified: Thu, 23 Apr 2020 17:51:33 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103463f158e3c7f91314c099c5524db53fd97efd35b7502a2991750063630384`  
		Last Modified: Thu, 23 Apr 2020 17:51:55 GMT  
		Size: 70.3 MB (70334752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c968fd52774e9a63a8ca1cd66b708fb02df8fdc207dc98e23a8682010b0047`  
		Last Modified: Thu, 23 Apr 2020 17:51:33 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cf3850d2505684647002e52f9e280c1cf6a30b8c49dddd6017ee83798bbb7`  
		Last Modified: Thu, 23 Apr 2020 17:52:43 GMT  
		Size: 18.6 MB (18579535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a2d85f3606b4622b9b2a90e8d654227e9f0ebd232876fe876afc91896d24b7`  
		Last Modified: Thu, 23 Apr 2020 17:52:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48169ea54a2577041dac811d298ab9e023a176fdc6dcb8c95c5cf41ebb9e378b`  
		Last Modified: Thu, 23 Apr 2020 17:52:34 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c5f90b05191d914ec993158e073730aa073d6c6035e66b61a9acf58cc1ecbc`  
		Last Modified: Thu, 23 Apr 2020 17:54:39 GMT  
		Size: 12.5 MB (12453558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396b3ffa930129ef6e71819652772db7e1196fb39b2b93edf4804993d22915a1`  
		Last Modified: Thu, 23 Apr 2020 17:54:36 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86a98663676269fd6dec230e4f42cc9c2b2fe2a3cccaa1d770a59fe3bedb31e`  
		Last Modified: Thu, 23 Apr 2020 17:54:38 GMT  
		Size: 13.7 MB (13739953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1773479e9c673bfa2ffab9d0e76f0205a4ba8ed4b20b28d95effd15cccb59f68`  
		Last Modified: Thu, 23 Apr 2020 17:54:35 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a4d9366080c0097860dd594eed6c2fadc4307a349bf2e236e7859bde8e48d`  
		Last Modified: Thu, 23 Apr 2020 17:54:35 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4537795cb57d50107dfe32d8cd244f802e688eaebc301cac5b258820e8abdd20`  
		Last Modified: Thu, 23 Apr 2020 17:54:35 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1550f75df887d89398c00ebdd3e9b46bd06b9356710adf7c3fc68ec3dd169985`  
		Last Modified: Thu, 23 Apr 2020 17:54:35 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d5a991c65cfac01901d9f765270a4345ca768e6a4fbe92645659d7d3eb29d1`  
		Last Modified: Fri, 24 Apr 2020 02:27:45 GMT  
		Size: 642.8 KB (642820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5fa2e0b6c665f58e6cfdeb858995baefad23feb25572b2ecfa3367a8a95a5`  
		Last Modified: Fri, 24 Apr 2020 02:27:45 GMT  
		Size: 8.2 KB (8227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38963aea7b9a20fdd983a0798e9af11c03c77670b7dc4fe53790db0923cf0e7c`  
		Last Modified: Fri, 24 Apr 2020 02:27:45 GMT  
		Size: 1.3 MB (1334644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c1f0d306dd6465eb515bfbed685d45f2b28fc0b195f7bcb9ba86aa38c966a1`  
		Last Modified: Fri, 24 Apr 2020 02:27:45 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; 386

```console
$ docker pull postfixadmin@sha256:8cd0c8d815bf167829df0bb98c987f9cd052e652f29e374496480546874f9f55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156909755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d4e30530e05b42ee64d9591f3599a34442a25db95e7d7d5f5eb55b8489365b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:58:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 11:58:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 11:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 11:58:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 11:58:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 12:06:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 12:06:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 12:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 12:06:50 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 12:06:51 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 12:06:52 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 12:06:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 12:06:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 12:06:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 12:06:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 12:36:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Apr 2020 12:36:50 GMT
ENV PHP_VERSION=7.3.17
# Thu, 23 Apr 2020 12:36:50 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 12:36:50 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 23 Apr 2020 12:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 12:37:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 12:42:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 12:42:22 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 12:42:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 12:42:24 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 12:42:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 12:42:24 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 12:42:25 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 12:42:25 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 12:42:25 GMT
EXPOSE 80
# Thu, 23 Apr 2020 12:42:25 GMT
CMD ["apache2-foreground"]
# Thu, 23 Apr 2020 20:36:01 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 23 Apr 2020 20:36:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 20:36:52 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Thu, 23 Apr 2020 20:36:52 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 23 Apr 2020 20:36:52 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Thu, 23 Apr 2020 20:36:53 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 23 Apr 2020 20:36:53 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 23 Apr 2020 20:36:54 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 23 Apr 2020 20:36:55 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 23 Apr 2020 20:36:55 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Thu, 23 Apr 2020 20:36:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 23 Apr 2020 20:36:56 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b6f6109ad6afc6066a9a9b19c9903065b90dc4ecb232ad312a50d2a3af7c20`  
		Last Modified: Thu, 23 Apr 2020 14:14:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b8d4220a9dc78cfb17d7518deddaa4957545b12088485de215374ec8cd5fcd`  
		Last Modified: Thu, 23 Apr 2020 14:14:26 GMT  
		Size: 81.2 MB (81198126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd893e354bac0fa6072eb200ef4c28c499dce07f2bf148816b9b04550dc27082`  
		Last Modified: Thu, 23 Apr 2020 14:14:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a71342deb67ff65b123b84dec7f6dd3772d7418cab3b8f1c9b05d2ed015c00a`  
		Last Modified: Thu, 23 Apr 2020 14:14:52 GMT  
		Size: 19.1 MB (19112697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69b5a5b87d25a9b0d974f78ef0902be086f49e7e4a97921db839b9e6882d06c`  
		Last Modified: Thu, 23 Apr 2020 14:14:46 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbd15ab6153d2103bf3572f753d9ca318b71e50d3a5808c0919f3cbed98c806`  
		Last Modified: Thu, 23 Apr 2020 14:14:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaa1758bc336e2c5876403e11e0e935427f0aa18345e01fb64072f43d958abc`  
		Last Modified: Thu, 23 Apr 2020 14:16:32 GMT  
		Size: 12.5 MB (12454031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4f746d43cb405201ae02ee1b214ef317f8b7f51cf9d51dc94c333c5f1efb6e`  
		Last Modified: Thu, 23 Apr 2020 14:16:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ebe8850627f71338deea3aac79acc66902df243242709edd4c731c5067c591`  
		Last Modified: Thu, 23 Apr 2020 14:16:35 GMT  
		Size: 14.4 MB (14375998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ca8f57a27212526ac2539a199b5bffa914f076e2cd7cd192dbee0c4a2454e4`  
		Last Modified: Thu, 23 Apr 2020 14:16:29 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553e0aee9799bff334b9883fa1cabce63e4f71882bc38b3524b48f07446a5e47`  
		Last Modified: Thu, 23 Apr 2020 14:16:29 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8217d2fb7e0230791f379cfac74d39f148b11c32b0b3d919c3c8dab57fb664e9`  
		Last Modified: Thu, 23 Apr 2020 14:16:29 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea5864b08357fb6bdfcff952ea76b8dfd93998f46536eb48f263636cbcac3d8`  
		Last Modified: Thu, 23 Apr 2020 14:16:29 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc280059014159f05c7197dc6ecb7c7252a2b66936d6e733c4347741413ba7`  
		Last Modified: Thu, 23 Apr 2020 20:38:12 GMT  
		Size: 665.3 KB (665311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580e8af4f58510631e69e7699c95e9b1be8dc309075263a8958b9160fd9e9018`  
		Last Modified: Thu, 23 Apr 2020 20:38:12 GMT  
		Size: 8.2 KB (8221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6f1b1919f0a75f8345a3c7615b54a2a5b7ace7a1f89519c4427322545d90`  
		Last Modified: Thu, 23 Apr 2020 20:38:13 GMT  
		Size: 1.3 MB (1334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b47aeabc99a087572154f0903227768c3048e6581fb391650e25ac831966eb`  
		Last Modified: Thu, 23 Apr 2020 20:38:12 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:2451b86a6bfac5833e679022dbafb8edc4108b8e91cb8db42de8ad8ad9defaf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162192497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f49918728ddff2e8797bdcc13ca7b4b8720279ae751b41fede48852fdccbede`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 14:58:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 14:58:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 15:00:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:01:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 15:01:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 15:07:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 15:08:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 15:09:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 15:09:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 15:09:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 15:09:28 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 15:09:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 15:09:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 15:09:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 15:09:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 15:33:23 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Apr 2020 15:33:29 GMT
ENV PHP_VERSION=7.3.17
# Thu, 23 Apr 2020 15:33:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 15:33:35 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 23 Apr 2020 15:34:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 15:34:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:39:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 15:39:40 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:39:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 15:39:51 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 15:39:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 15:39:57 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 15:39:58 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:40:01 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 15:40:03 GMT
EXPOSE 80
# Thu, 23 Apr 2020 15:40:07 GMT
CMD ["apache2-foreground"]
# Fri, 24 Apr 2020 00:06:21 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 24 Apr 2020 00:07:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:07:24 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 00:07:26 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 00:07:28 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 24 Apr 2020 00:07:30 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 24 Apr 2020 00:07:32 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 24 Apr 2020 00:07:37 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 24 Apr 2020 00:07:41 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 24 Apr 2020 00:07:43 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 24 Apr 2020 00:07:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 24 Apr 2020 00:07:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b755a3bf05f4bf7425e586a874481ea765f886765d68e5e3973f9ac727187c6c`  
		Last Modified: Thu, 23 Apr 2020 17:16:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81edbd0a9383cf9bc58dcb07cb9b0cc6454030497e3a606ae400db6a3b6a1962`  
		Last Modified: Thu, 23 Apr 2020 17:17:15 GMT  
		Size: 82.3 MB (82259619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947531f183613e1f7fca563adeccbc3242cda14370ed376901fbf634af0264c3`  
		Last Modified: Thu, 23 Apr 2020 17:16:20 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a95e79fe710527d52bde3f306bfd30c4fd804fa4ef236e53a0bcf240504c8aa`  
		Last Modified: Thu, 23 Apr 2020 17:18:21 GMT  
		Size: 19.8 MB (19812607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de97ec0f6e96230894adec6eadf7a2f8cc7608e6dd5b441dfe99cac9ac85357`  
		Last Modified: Thu, 23 Apr 2020 17:18:12 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8347f80ea17e906c812e85500251d7c276e9380aeb01c0326b9026631d2b09b`  
		Last Modified: Thu, 23 Apr 2020 17:18:08 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d280b61c80ce6ed18df7fc295ece65cf8d023f5d792b68c8575ec070cc5b58`  
		Last Modified: Thu, 23 Apr 2020 17:21:06 GMT  
		Size: 12.5 MB (12454463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7f5b9eaa6c41153c0fbfe843a44797b9cd0a41337a3593529550233f61ec58`  
		Last Modified: Thu, 23 Apr 2020 17:21:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a845579e71a37bff92aff492f4ab18e713b68b6c3b02174110a4d2fdaa833a06`  
		Last Modified: Thu, 23 Apr 2020 17:21:11 GMT  
		Size: 15.1 MB (15094382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82f19362e23f22ab6f2d07666fa3e199b0c1af4f3810088622cce61c4d73db`  
		Last Modified: Thu, 23 Apr 2020 17:21:01 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e697af043186fbfd20c3186cbbf1684604b8f16a862f99b809f9b50bf40db`  
		Last Modified: Thu, 23 Apr 2020 17:21:00 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a2ee3f400bdbae56b5de4a4884395e182adc42179d676c3df85dbfd48c2444`  
		Last Modified: Thu, 23 Apr 2020 17:21:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6a666916a5f6021166907db55d337838e504497859fca1dfbc61f262d05e1c`  
		Last Modified: Thu, 23 Apr 2020 17:21:00 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acef7de99f584554b23530f7ed4c6842f2c633e0aa2dda497d8de5bde142e9e7`  
		Last Modified: Fri, 24 Apr 2020 00:09:37 GMT  
		Size: 697.0 KB (697012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72b758aa2eb05893edc579a62b543226c386696349c6752ed8127e1b82e9407`  
		Last Modified: Fri, 24 Apr 2020 00:09:37 GMT  
		Size: 8.2 KB (8222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d289809627f33dc6eeaeb491dafa505e09f7f4403f197d9ab0adb761f30d93f`  
		Last Modified: Fri, 24 Apr 2020 00:09:38 GMT  
		Size: 1.3 MB (1334645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34f49a691206f3645a62043454682967f63e649472b4f73c2bb9bf99f2490c`  
		Last Modified: Fri, 24 Apr 2020 00:09:37 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; s390x

```console
$ docker pull postfixadmin@sha256:bc9c663df3f295bb822a873ea7ce4cbb1c160197c3dd848095e2465b305a49b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136666319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dd5c53bbd0291ff94b0877733990b923d9246e4dad4a1191c5612dec2d42f1d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 07:06:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 07:06:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 07:07:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 07:07:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 07:07:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 07:10:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 07:10:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 07:10:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 07:10:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 07:10:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 07:10:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 07:10:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 07:10:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 07:10:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 07:10:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 07:20:58 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Apr 2020 07:20:58 GMT
ENV PHP_VERSION=7.3.17
# Thu, 23 Apr 2020 07:20:58 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 07:20:58 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 23 Apr 2020 07:21:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 07:21:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:22:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 07:22:42 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:22:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 07:22:44 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 07:22:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 07:22:44 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 07:22:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:22:45 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 07:22:45 GMT
EXPOSE 80
# Thu, 23 Apr 2020 07:22:45 GMT
CMD ["apache2-foreground"]
# Thu, 23 Apr 2020 16:05:48 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 23 Apr 2020 16:06:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 16:06:38 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Thu, 23 Apr 2020 16:06:39 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 23 Apr 2020 16:06:39 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Thu, 23 Apr 2020 16:06:40 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 23 Apr 2020 16:06:41 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 23 Apr 2020 16:06:42 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 23 Apr 2020 16:06:46 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 23 Apr 2020 16:06:46 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:06:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:06:48 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08bde6b0b1d4817b549715812249f566ebbdb1c81c26581d3a34e9f0646ac7`  
		Last Modified: Thu, 23 Apr 2020 08:06:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb184ae545a538a5e99fa27bf76f21aeb7324f061ae0e6ed7ab6003f8ec8d861`  
		Last Modified: Thu, 23 Apr 2020 08:06:57 GMT  
		Size: 64.7 MB (64698982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bff96336b89f3c42d3c1ca154c9bee84597dd2e1776952a82e47e94dac6e5c`  
		Last Modified: Thu, 23 Apr 2020 08:06:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2101c4a938d8b8d63ad7e9e67ce5e8f648130174093f07c2dba57707145c46e4`  
		Last Modified: Thu, 23 Apr 2020 08:07:42 GMT  
		Size: 18.5 MB (18522444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98988af543b5301ceb878cb0da958a05b2d1ba052efd8780bcbe589b82bcbe1`  
		Last Modified: Thu, 23 Apr 2020 08:07:39 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd3c6a14b8cb1d6330e59c568e4a5aa3c4035eedd019b1b06b7f9aded5e4e66`  
		Last Modified: Thu, 23 Apr 2020 08:07:37 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fc84539a1fbb471cbb5ccfa0a447f70bf5fca81dcbb9638bc91f72adcd1843`  
		Last Modified: Thu, 23 Apr 2020 08:09:21 GMT  
		Size: 12.5 MB (12453140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e784e0f7faff7880bd1b4475c505f2dd2559068f777af6664b62b48edc141e`  
		Last Modified: Thu, 23 Apr 2020 08:09:18 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115a6b68f5abeb50de445814a1bcd77c1793f5aeb881d5ee69086665923927c3`  
		Last Modified: Thu, 23 Apr 2020 08:09:20 GMT  
		Size: 13.3 MB (13286023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a293f9ef172f817ffe2493185e3425f40459cd14795366131476fe87f6a83c4f`  
		Last Modified: Thu, 23 Apr 2020 08:09:16 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ba80c5e48efe4a8c2b3cb861b473c1f699e68263b56c1b8c4ab2f46fbff661`  
		Last Modified: Thu, 23 Apr 2020 08:09:17 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e588c7e6b4007b71c67e4f12d45091f06c881933d42227156aa11d0242cef0c6`  
		Last Modified: Thu, 23 Apr 2020 08:09:16 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633ac3880d459f3f8fc7f339b19f0c0107eb8e46d84180d4b2b531999747a2c0`  
		Last Modified: Thu, 23 Apr 2020 08:09:17 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a241d17722d780d3787f4330cbe8a2fa8d733820816b6277d310ddf05ca87e0`  
		Last Modified: Thu, 23 Apr 2020 16:08:16 GMT  
		Size: 643.9 KB (643852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2981f71e5afbba34b22692d69cdb7db7fd8d038130f5d1d5c184af2c44ddde0a`  
		Last Modified: Thu, 23 Apr 2020 16:08:16 GMT  
		Size: 8.2 KB (8225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d64c0717e66669004c79aaff452f3b8950b0dec72d1b24a3315d0024d0b4814`  
		Last Modified: Thu, 23 Apr 2020 16:08:22 GMT  
		Size: 1.3 MB (1334646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bef30287cf00edc9cda1115eb5bedc6c1ab89241e5d30a99a4374e8661b069`  
		Last Modified: Thu, 23 Apr 2020 16:08:16 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
