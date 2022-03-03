## `postfixadmin:3-apache`

```console
$ docker pull postfixadmin@sha256:61b047c887a790db738eef55cdb270e8da5d2e9d4682a55074195d33ffa432af
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

### `postfixadmin:3-apache` - linux; amd64

```console
$ docker pull postfixadmin@sha256:e1285da81a5d46a73af6e010972005c6dfbc311b126f23411b031e2aaa8038ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.4 MB (171371844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bacd9ef1b3ac224956d9861d4dc59b3d611b02b08af6070a6b133de39a25908`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:17:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 16:17:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 16:18:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:18:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 16:18:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 16:27:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 16:27:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 16:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 16:27:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 16:27:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 16:27:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 16:27:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 16:27:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 18:09:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 18:26:23 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 18:26:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 18:26:23 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 18:27:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Feb 2022 18:27:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Feb 2022 18:30:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Feb 2022 18:30:25 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 17 Feb 2022 18:30:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Feb 2022 18:30:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Feb 2022 18:30:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 17 Feb 2022 18:30:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 17 Feb 2022 18:30:27 GMT
WORKDIR /var/www/html
# Thu, 17 Feb 2022 18:30:27 GMT
EXPOSE 80
# Thu, 17 Feb 2022 18:30:27 GMT
CMD ["apache2-foreground"]
# Thu, 17 Feb 2022 22:47:14 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 17 Feb 2022 22:47:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Feb 2022 22:47:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Feb 2022 22:47:51 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 17 Feb 2022 22:47:51 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 17 Feb 2022 22:47:52 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 17 Feb 2022 22:47:52 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 17 Feb 2022 22:47:52 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 17 Feb 2022 22:47:53 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 17 Feb 2022 22:47:55 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 17 Feb 2022 22:47:55 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 17 Feb 2022 22:47:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 17 Feb 2022 22:47:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1ad84cf10194e2130f05599fcf95721234f2e72aeb9b2c7341719a0a736e41`  
		Last Modified: Wed, 26 Jan 2022 19:09:25 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c937dadeb7e3e4f156ed8bf156bc07d09c18d255475f602ae6e7c94ad0efc5`  
		Last Modified: Wed, 26 Jan 2022 19:09:41 GMT  
		Size: 91.6 MB (91604421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2f1dc96e597c811b3e8c3d0332b71dd64989ff1f972ffbc477edbc479062f7`  
		Last Modified: Wed, 26 Jan 2022 19:09:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c3f82c39d441d1987e11925e9cda5f1f9aba52ad1d3c341e9c4e7f1efe42c0`  
		Last Modified: Wed, 26 Jan 2022 19:10:41 GMT  
		Size: 19.2 MB (19245845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc6462bd8e4fa3a65fff11c70bd270c8f59545a093c6d3124a426036e3880a`  
		Last Modified: Wed, 26 Jan 2022 19:10:37 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c670d99116c951149bb76403284f5a63b99c3788e7088cf4278364322ba777ac`  
		Last Modified: Wed, 26 Jan 2022 19:10:37 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b5d4e23f0388efaf57b5f2e27bc92b9dc24163681658e2a32172b619f86e5b`  
		Last Modified: Thu, 17 Feb 2022 21:02:25 GMT  
		Size: 10.8 MB (10758158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2a6d8c1af31afa548177cc8b0b3c5ccb590ab2e16c6a7233ad9efe7d04d304`  
		Last Modified: Thu, 17 Feb 2022 21:02:22 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597ec12098727268dc3e7243dae87b159c943a351ef3e62fd891609412efd499`  
		Last Modified: Thu, 17 Feb 2022 21:02:25 GMT  
		Size: 14.0 MB (14046693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe74968caee05911c6adb08f769568e0dead55eb5732442733aed653e4e022c9`  
		Last Modified: Thu, 17 Feb 2022 21:02:22 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51e1df1e33fc9be5094b4ac9eb9ffb8eed2ede2e934f094c9425e1842654e90`  
		Last Modified: Thu, 17 Feb 2022 21:02:22 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b82a1163e0161389b7bd2607a6b9510767534ea1f41f8a53271a876f3b2605`  
		Last Modified: Thu, 17 Feb 2022 21:02:22 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66138b20463e0df4188a19eab626104973ef2300cea700f0c5010fe1922188cf`  
		Last Modified: Thu, 17 Feb 2022 22:50:02 GMT  
		Size: 1.3 MB (1284068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6ad04c597cc68131ac7609fa131091cf0f75bebc7cd314524ee91c4e8551e`  
		Last Modified: Thu, 17 Feb 2022 22:50:03 GMT  
		Size: 1.2 MB (1186304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11514742b0293129982e5ce94663a9144c819bae3473ebe2ddcfa05d6f9c16ea`  
		Last Modified: Thu, 17 Feb 2022 22:50:02 GMT  
		Size: 8.2 KB (8224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925fa9d517b67752ea3d8d765b42bd8ec92b01b06a485d5cc294953490eca747`  
		Last Modified: Thu, 17 Feb 2022 22:50:02 GMT  
		Size: 1.9 MB (1864836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50570a672b89d6570c143a230db3ddd700a8283fdbb8871243ff17e3f8ad62d`  
		Last Modified: Thu, 17 Feb 2022 22:50:02 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; arm variant v5

```console
$ docker pull postfixadmin@sha256:8645d7e1e2de4c164e2a5a00e775987e2d03d0554e76ee29989afdaa362e16a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.1 MB (149111926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954d7527b4411e9be54683e18ce832007173d9c63122e676c162d94ca5498e34`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:53 GMT
ADD file:eb61ee802e5118b26e1fec2c7fc58e34de0de54a5fd47dc6318c11a039ef528f in / 
# Tue, 01 Mar 2022 02:02:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:18:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 13:18:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 13:18:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:18:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 13:18:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 13:25:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 13:25:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 13:25:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 13:25:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 13:25:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 13:25:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:25:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:25:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 14:58:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Mar 2022 14:58:19 GMT
ENV PHP_VERSION=7.4.28
# Tue, 01 Mar 2022 14:58:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 01 Mar 2022 14:58:20 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 01 Mar 2022 14:58:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 14:58:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Mar 2022 15:03:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Mar 2022 15:03:04 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Tue, 01 Mar 2022 15:03:06 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Mar 2022 15:03:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Mar 2022 15:03:06 GMT
STOPSIGNAL SIGWINCH
# Tue, 01 Mar 2022 15:03:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 01 Mar 2022 15:03:08 GMT
WORKDIR /var/www/html
# Tue, 01 Mar 2022 15:03:08 GMT
EXPOSE 80
# Tue, 01 Mar 2022 15:03:08 GMT
CMD ["apache2-foreground"]
# Wed, 02 Mar 2022 11:39:50 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Wed, 02 Mar 2022 11:40:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 11:41:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 11:41:50 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Wed, 02 Mar 2022 11:41:51 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Wed, 02 Mar 2022 11:41:51 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Wed, 02 Mar 2022 11:41:52 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Wed, 02 Mar 2022 11:41:52 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Wed, 02 Mar 2022 11:41:54 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Wed, 02 Mar 2022 11:41:57 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Wed, 02 Mar 2022 11:41:57 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Wed, 02 Mar 2022 11:41:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 02 Mar 2022 11:41:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4aa6e26b4dfdac27e5b5e15b7ebf4366149755a79dd653a5b68d9d93dd94c695`  
		Last Modified: Tue, 01 Mar 2022 02:18:33 GMT  
		Size: 28.9 MB (28909528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdad6916f037c9d7d3da52a99d3452d403d5845deeb12407caed60f3503c379`  
		Last Modified: Tue, 01 Mar 2022 16:26:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64502c70688d4183009eb799afb394a7ffc43bc7abfab2e2dd3fc4f8a30b268`  
		Last Modified: Tue, 01 Mar 2022 16:26:57 GMT  
		Size: 73.7 MB (73684127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467221c05730cce61a7bc60465100a949657a85c508404a806ab9b6d86305497`  
		Last Modified: Tue, 01 Mar 2022 16:26:08 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4525a06a0af94fa8b0f9979073e5ffc1ec56f221d37672bc337c8b52534205d9`  
		Last Modified: Tue, 01 Mar 2022 16:28:18 GMT  
		Size: 18.5 MB (18539852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c3b85f9dc3e90460dbba216997c21bbde27bb7897c1f0ec891bbcbc7506d1e`  
		Last Modified: Tue, 01 Mar 2022 16:28:07 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13c089110614b490507597cebb1d849dde0ae7772aa8c597867f0b01d0d6b32`  
		Last Modified: Tue, 01 Mar 2022 16:28:07 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754992199451d1a809d80dc0f47e291f3b69c6e5420c031669faea780ad026b2`  
		Last Modified: Tue, 01 Mar 2022 16:39:54 GMT  
		Size: 10.8 MB (10756808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e43d9299761ee54a9f27fa52f3c9f5f0f8ef43b843ab8e28c7a92f1afcd993c`  
		Last Modified: Tue, 01 Mar 2022 16:39:49 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2fa80a33a114b78879a7e1d0b0c53aaf1f4623b950330a8bbbb6a316ddae72`  
		Last Modified: Tue, 01 Mar 2022 16:39:58 GMT  
		Size: 13.0 MB (12982060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bff17aaff5d7729133d1bc0b6df2c9ab5c49a0c880f9e2f8d5e5fec5815e4`  
		Last Modified: Tue, 01 Mar 2022 16:39:49 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27a74aa6aaf363660e3d00045148dfd82e620b74ef13e800de9e41353e4d96e`  
		Last Modified: Tue, 01 Mar 2022 16:39:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d25aad064ea2aac039bbdf5fb17480b02a0e0de22961fa374b6323b0a8ceaf`  
		Last Modified: Tue, 01 Mar 2022 16:39:49 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725b2777df570e7f94131c936ffbf9bac23915dc00ad5e0a9cc83b76da6cf282`  
		Last Modified: Wed, 02 Mar 2022 11:45:28 GMT  
		Size: 1.2 MB (1229965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc18ea813d4d1a7216b6a1983502340a19e3ad9246504ea21ef414f78b1f7e1`  
		Last Modified: Wed, 02 Mar 2022 11:45:28 GMT  
		Size: 1.1 MB (1129520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66204dcd1f94a5863a26491d0dee757f7c556b038bb3a28fcd3ec5fefd0059fc`  
		Last Modified: Wed, 02 Mar 2022 11:45:27 GMT  
		Size: 8.2 KB (8222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca27ef1aff03866d031c1a6574aa5b6262a07a327e6ffef56ea80c69d3cedffe`  
		Last Modified: Wed, 02 Mar 2022 11:45:29 GMT  
		Size: 1.9 MB (1864818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fad5ad1d29a46b7c043bee87c77b53ff5a9f8b21ec111b580038e96496f861`  
		Last Modified: Wed, 02 Mar 2022 11:45:27 GMT  
		Size: 1.6 KB (1595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:05c281d844ebbb35c196bf95b188567d6f72b3bd6c5fe8b57d66e5a6e1dee94d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141199054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd006a6d3fe1cfe7e2db0a501e672f125a5ca68d361e030fb35f41a6777b262`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:27:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 03:27:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:28:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 03:28:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 03:34:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 03:34:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 03:34:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 03:34:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 03:34:50 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 03:34:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:34:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 03:34:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 05:02:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 19:14:46 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 19:14:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 19:14:47 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 19:15:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Feb 2022 19:15:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Feb 2022 19:19:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Feb 2022 19:19:17 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 17 Feb 2022 19:19:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Feb 2022 19:19:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Feb 2022 19:19:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 17 Feb 2022 19:19:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 17 Feb 2022 19:19:21 GMT
WORKDIR /var/www/html
# Thu, 17 Feb 2022 19:19:21 GMT
EXPOSE 80
# Thu, 17 Feb 2022 19:19:22 GMT
CMD ["apache2-foreground"]
# Fri, 18 Feb 2022 03:34:20 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 18 Feb 2022 03:34:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Feb 2022 03:36:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Feb 2022 03:36:12 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 18 Feb 2022 03:36:13 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 18 Feb 2022 03:36:13 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 18 Feb 2022 03:36:14 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 18 Feb 2022 03:36:14 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 18 Feb 2022 03:36:16 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 18 Feb 2022 03:36:19 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 18 Feb 2022 03:36:20 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Fri, 18 Feb 2022 03:36:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 18 Feb 2022 03:36:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc9a20cd165cc34bba0c0bab277b6fbf5b727eb38c1b902e577a6f91bdd4980`  
		Last Modified: Wed, 26 Jan 2022 06:36:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e7063615e6e2b8aee21d5be918dc091b1ed4a0792197b96205dcb419f7115b`  
		Last Modified: Wed, 26 Jan 2022 06:37:29 GMT  
		Size: 69.3 MB (69315436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed49ea1bd88a9bbfafb4155619fe90383f2f713205f8bb810a75902408f0d1de`  
		Last Modified: Wed, 26 Jan 2022 06:36:46 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22e82e5b1bd524afe0d900329ad1f0e1dcb427a3ff6c5e37accd58d6780ff1b`  
		Last Modified: Wed, 26 Jan 2022 08:19:17 GMT  
		Size: 18.0 MB (17993026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65de72f6bd09c20a231d7a2cf455eed5327c561f4b52e2fb20a6ca99b7c75e`  
		Last Modified: Wed, 26 Jan 2022 08:19:07 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292027d35ecb573bb5871e1fe35b5fdde0c782984668e9658d3e3936dda27b7`  
		Last Modified: Wed, 26 Jan 2022 08:19:07 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c327725381c590dd0355d55812fd476bb419a7ba32b152e86fc857e1d9fbfc`  
		Last Modified: Thu, 17 Feb 2022 20:52:23 GMT  
		Size: 10.8 MB (10756911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3397db8ca65e8724cfb8d8bf5fc147f01a3f8d63ad9f1b92dec7af8d054ddb01`  
		Last Modified: Thu, 17 Feb 2022 20:52:18 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33422b5b4fcdfb802cf283ae0603693f9c9b211ce9cb5f4fee999cbd940a3aef`  
		Last Modified: Thu, 17 Feb 2022 20:52:27 GMT  
		Size: 12.4 MB (12384149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a516764556336b50ea83b3f77b55b435506f40092210983b21fcfc49f52e8667`  
		Last Modified: Thu, 17 Feb 2022 20:52:18 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348d649f47445b7022140c67ae29189013222ee92df6aecaae9c24933c04699d`  
		Last Modified: Thu, 17 Feb 2022 20:52:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4c95c4194f3ffff35410a4415334b155ebd010d42ef4564d7fbf4cd9fc9b2f`  
		Last Modified: Thu, 17 Feb 2022 20:52:18 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40303472be7e5eb7a7a6d951f907e6a6978ae2a86b75e9db7776715e222fc37`  
		Last Modified: Fri, 18 Feb 2022 03:42:01 GMT  
		Size: 1.2 MB (1224496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570be1c7ab5bb98a4c2a113877b930fe27706123fc31328848ed37599f6e8ae2`  
		Last Modified: Fri, 18 Feb 2022 03:42:01 GMT  
		Size: 1.1 MB (1079984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2405ceffece256c2557d12ed86c198ce626955725b1a049609fd9426f350d126`  
		Last Modified: Fri, 18 Feb 2022 03:42:00 GMT  
		Size: 8.2 KB (8224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69044b2ec45967849290aa97916f682f30fdd36c4e001a9b769dcf4003bab59f`  
		Last Modified: Fri, 18 Feb 2022 03:42:02 GMT  
		Size: 1.9 MB (1864845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d068ab1451b9c4bdb8d3cb1c39983b9e4d96f67566e3260a1aed73ec4dfb94b0`  
		Last Modified: Fri, 18 Feb 2022 03:42:00 GMT  
		Size: 1.6 KB (1599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:b3e9225632b077f255e98a76865a376fb92f6b0e493397b210beb0de6248914e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.3 MB (160294471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e712dea1ed644c715a7f133c42e85564dcf33907410a2573ef3a276eb8d5de`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 16:21:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 16:21:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 16:21:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 16:21:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 16:21:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 16:28:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 16:28:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 16:28:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 16:28:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 16:28:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 16:28:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 16:28:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 16:28:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 17:30:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Mar 2022 17:30:30 GMT
ENV PHP_VERSION=7.4.28
# Tue, 01 Mar 2022 17:30:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 01 Mar 2022 17:30:32 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 01 Mar 2022 17:31:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 17:31:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:54:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 21:54:06 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:54:06 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 21:54:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 21:54:08 GMT
STOPSIGNAL SIGWINCH
# Wed, 02 Mar 2022 21:54:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:54:10 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 21:54:11 GMT
EXPOSE 80
# Wed, 02 Mar 2022 21:54:12 GMT
CMD ["apache2-foreground"]
# Thu, 03 Mar 2022 01:40:48 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 03 Mar 2022 01:40:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 01:41:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 01:41:25 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Thu, 03 Mar 2022 01:41:26 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 03 Mar 2022 01:41:27 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Thu, 03 Mar 2022 01:41:28 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 03 Mar 2022 01:41:29 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 03 Mar 2022 01:41:30 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 03 Mar 2022 01:41:33 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 03 Mar 2022 01:41:34 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 03 Mar 2022 01:41:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 03 Mar 2022 01:41:35 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33762069c180ac7a2bd850df459df42f7dac21d9a3ca6d6b138bd972ceb3b2`  
		Last Modified: Tue, 01 Mar 2022 18:17:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94fc40547e2c4be338f062fc29bcd2c7f19345badf0ff429726978f764df45e`  
		Last Modified: Tue, 01 Mar 2022 18:17:39 GMT  
		Size: 86.9 MB (86920736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63844f2b3ed82fda7e922caee6208b748ab2244bc614e0c7e140f8d6401b15e6`  
		Last Modified: Tue, 01 Mar 2022 18:17:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d266bd1762c9e1f8829e89d2afbe0a50182d933749c48d8f4520629ae6f10`  
		Last Modified: Tue, 01 Mar 2022 18:18:41 GMT  
		Size: 18.9 MB (18943623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f752ab6d43690a94880d9ce2a919e6496b56011b1a02849267f3edd5f8f4ab4f`  
		Last Modified: Tue, 01 Mar 2022 18:18:39 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a2301cb0006dfb0af21fd521a8d25be1a4174abdc5942f9fe1666ae5742542`  
		Last Modified: Tue, 01 Mar 2022 18:18:39 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb1d14bc09e07e2b325ee9b24a086da679af6de81d744115b91faf75a1b19fb`  
		Last Modified: Tue, 01 Mar 2022 18:26:44 GMT  
		Size: 10.5 MB (10541968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8d3af31136d32d4b46989c34d5b9dcf64f462ef3ab4d95a17fc3d79beb6f2f`  
		Last Modified: Tue, 01 Mar 2022 18:26:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7d30c4cc2a81bd113b9d67551da6b2d669d2faffb8abf1ce3bb6909d536f45`  
		Last Modified: Wed, 02 Mar 2022 23:25:46 GMT  
		Size: 10.0 MB (9998224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8f97cd022b3e5e5a6f7341459a6eed5e16a91157fd0e0399a472a3de956f8c`  
		Last Modified: Wed, 02 Mar 2022 23:25:44 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee15129365a8ea8890bc479fef3b85ec90f26c79d6e263b70ace46c2e0a148f`  
		Last Modified: Wed, 02 Mar 2022 23:25:44 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3214c714844e3e9a0931ef2c1fe026cb800f3fc2a31d7aaa052df9089c39da`  
		Last Modified: Wed, 02 Mar 2022 23:25:44 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ed0fbb1d6a10d5baf3c1a0c20b10b04e4a3959ea87731e1ca455cba883bdaa`  
		Last Modified: Thu, 03 Mar 2022 01:43:55 GMT  
		Size: 991.5 KB (991456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8923abba6a15bf1f9ccc54b4f2717c8fe2ef28cfc03d7d1dca29711bd09b678c`  
		Last Modified: Thu, 03 Mar 2022 01:43:55 GMT  
		Size: 961.4 KB (961356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3330409cf76bca6b5c99596d8e862d09f0e083d3019e2890c8868e0f1afd1d`  
		Last Modified: Thu, 03 Mar 2022 01:43:54 GMT  
		Size: 8.2 KB (8218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6253e0187d25713924efec016bca71fe146633f74c60275ea0c19d968cae406b`  
		Last Modified: Thu, 03 Mar 2022 01:43:55 GMT  
		Size: 1.9 MB (1864985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ebf1bec532410b6bdd414aac116e02d9c925bbb7444640d9e1cf231573048f`  
		Last Modified: Thu, 03 Mar 2022 01:43:55 GMT  
		Size: 1.6 KB (1595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; 386

```console
$ docker pull postfixadmin@sha256:8d99c2959487097cf4e7464c48d845e1d1ea29743259d43c4e866a3c1c020bd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.3 MB (170336089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab367be3a5829ea5ae928c6905f8477f4801964f7d261cf7edabd9de723cbddf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 15:11:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 15:11:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 15:11:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:11:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 15:11:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 15:21:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 15:21:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 15:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 15:21:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 15:21:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 15:21:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 15:21:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 15:21:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 17:40:32 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Mar 2022 17:40:32 GMT
ENV PHP_VERSION=7.4.28
# Tue, 01 Mar 2022 17:40:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 01 Mar 2022 17:40:32 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 01 Mar 2022 17:41:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 17:41:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 22:08:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 22:08:37 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 02 Mar 2022 22:08:37 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 22:08:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 22:08:38 GMT
STOPSIGNAL SIGWINCH
# Wed, 02 Mar 2022 22:08:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 02 Mar 2022 22:08:38 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 22:08:38 GMT
EXPOSE 80
# Wed, 02 Mar 2022 22:08:38 GMT
CMD ["apache2-foreground"]
# Thu, 03 Mar 2022 01:01:01 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 03 Mar 2022 01:01:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 01:01:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 01:01:44 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Thu, 03 Mar 2022 01:01:44 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 03 Mar 2022 01:01:44 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Thu, 03 Mar 2022 01:01:45 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 03 Mar 2022 01:01:45 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 03 Mar 2022 01:01:46 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 03 Mar 2022 01:01:47 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 03 Mar 2022 01:01:48 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 03 Mar 2022 01:01:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 03 Mar 2022 01:01:48 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaee34f3c6a532588cab5618c0c2cd27d4fbc713824ae1017b96cf8655c5c4e`  
		Last Modified: Tue, 01 Mar 2022 19:19:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab7419028c0335ca5652ae1b7b0d6a245a1880f3f0db3ee2e7f52c6699c7320`  
		Last Modified: Tue, 01 Mar 2022 19:20:15 GMT  
		Size: 92.7 MB (92716709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3d0b6ac083a10e9db01232c45dd11a397351a30082762071adc6f4e398a4bc`  
		Last Modified: Tue, 01 Mar 2022 19:19:52 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3860ef1b54af78c1119ed2246557e2d6bdcbd064475d9a9f6a371ca269a7a7`  
		Last Modified: Tue, 01 Mar 2022 19:21:30 GMT  
		Size: 19.7 MB (19714254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa7aa1d76ef078062230dd8b6e5e69f34636eeeaae9dc7452f371012327e977`  
		Last Modified: Tue, 01 Mar 2022 19:21:24 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1ba670bbaf2b18ece3f4313dfcb5c2fda57a31224bcf51030d591a33126adb`  
		Last Modified: Tue, 01 Mar 2022 19:21:24 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea2c3130160b2025f80bac6385fe6d89d9182f2e0c92de0e2a149f61c61c270`  
		Last Modified: Tue, 01 Mar 2022 19:32:24 GMT  
		Size: 10.8 MB (10757441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29a11d4a1e9744bf2b2bb375409dd0b5bf0e823c146ca96915b8afbff422760`  
		Last Modified: Tue, 01 Mar 2022 19:32:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d81d9131d458f9e70f871f6795169278f76f6112d7b67f208b39b19d574a03`  
		Last Modified: Thu, 03 Mar 2022 00:38:53 GMT  
		Size: 10.4 MB (10443086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b180d46b9df86371809fbead8ea88a565d00f950c9b51e58f7d96ea9dce9d847`  
		Last Modified: Thu, 03 Mar 2022 00:38:50 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f25cd9c02c879134e2ea608b7882ad11c067076393e204420c8491d6a8c768d`  
		Last Modified: Thu, 03 Mar 2022 00:38:50 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90afb76127aad1cd565f3322409fd3141b6c700c2d2e1fe1e2c196e43793b9f7`  
		Last Modified: Thu, 03 Mar 2022 00:38:50 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37ab5887209517c111aa86fdeb4d829b5329eef866846e14b7793234e35043`  
		Last Modified: Thu, 03 Mar 2022 01:04:20 GMT  
		Size: 1.2 MB (1243254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd91980326a49dcd7cc158df09eeda7c961ca6ad45e1ee71571c9b0e0d4ab38`  
		Last Modified: Thu, 03 Mar 2022 01:04:20 GMT  
		Size: 1.2 MB (1203605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5bb2fe88bb99c2c6127fc14b29dac24d06e9b2ab2293b1c08198843747cb92`  
		Last Modified: Thu, 03 Mar 2022 01:04:19 GMT  
		Size: 8.2 KB (8218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54fdd2d7dc2872ead55c77de6996c5415c4094aa87851d8de2598bc5984293a`  
		Last Modified: Thu, 03 Mar 2022 01:04:20 GMT  
		Size: 1.9 MB (1865104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46297bf8af849e1f83da5392a8efb56d9dafdef1295857e0c26ab792a1614cac`  
		Last Modified: Thu, 03 Mar 2022 01:04:19 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; mips64le

```console
$ docker pull postfixadmin@sha256:e902a26a2b91b34b572c13f52baab99118127271e0833543675d4e00aa28c6a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.1 MB (149082367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26cf7121231a57746c5edf0fd3cc38feb521bfd8d79c31bc19c6ad0f0b0d6ed0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 12:25:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 12:25:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 12:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 12:26:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 12:26:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 12:39:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 12:39:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 12:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 12:40:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 12:40:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 12:40:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 12:40:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 12:40:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 16:05:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 19:18:08 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 19:18:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 19:18:09 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 19:18:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Feb 2022 19:18:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Feb 2022 19:26:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Feb 2022 19:26:24 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 17 Feb 2022 19:26:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Feb 2022 19:26:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Feb 2022 19:26:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 17 Feb 2022 19:26:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 17 Feb 2022 19:26:27 GMT
WORKDIR /var/www/html
# Thu, 17 Feb 2022 19:26:28 GMT
EXPOSE 80
# Thu, 17 Feb 2022 19:26:28 GMT
CMD ["apache2-foreground"]
# Thu, 17 Feb 2022 22:34:50 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 17 Feb 2022 22:35:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Feb 2022 22:36:58 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Feb 2022 22:36:58 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 17 Feb 2022 22:36:58 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 17 Feb 2022 22:36:59 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 17 Feb 2022 22:36:59 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 17 Feb 2022 22:36:59 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 17 Feb 2022 22:37:01 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 17 Feb 2022 22:37:05 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 17 Feb 2022 22:37:06 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 17 Feb 2022 22:37:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 17 Feb 2022 22:37:06 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191e94952e609ddcd788e8b84a0c6e52cb8d70b72fc1ecdf09671b8b97c8ae88`  
		Last Modified: Wed, 26 Jan 2022 18:35:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a20e2dcd1bfa855631549301d1b32d7018e8471fd65e4172a12ade76c981de`  
		Last Modified: Wed, 26 Jan 2022 18:36:05 GMT  
		Size: 72.0 MB (72013491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1dc62c31c14b2b41b143b779c94633e090e9b781c749c205f379a4a404e4ef`  
		Last Modified: Wed, 26 Jan 2022 18:35:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa51c2bcf42e9b3ec702bec52c0b36b70bf365f6fa4fa1908b7261a112c1dd2c`  
		Last Modified: Wed, 26 Jan 2022 18:37:13 GMT  
		Size: 19.1 MB (19145545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d0161a75ed794ace7404c46755af243b6f1b5f40277f8e34adb69a84b23cce`  
		Last Modified: Wed, 26 Jan 2022 18:36:59 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7bc9abc811886cd43346551116f915ee9670ac9db88c80df0a08c457f94545`  
		Last Modified: Wed, 26 Jan 2022 18:36:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa750875ada5b080a253dd437e234f332970743a2adc0b30ecd918d838410278`  
		Last Modified: Thu, 17 Feb 2022 20:30:47 GMT  
		Size: 10.8 MB (10756229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5195d83f8fe50efbe70829ed22e7502249a7322902129735c94c7df1745cd2`  
		Last Modified: Thu, 17 Feb 2022 20:30:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b0174df0c2ddfa247d6329cd725873b0763ed85f8278696219e52e5a7653fd`  
		Last Modified: Thu, 17 Feb 2022 20:30:53 GMT  
		Size: 13.3 MB (13340776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0ade321d1d3b50fde8527ea02531280868a5cad4a488fe40502557a192d839`  
		Last Modified: Thu, 17 Feb 2022 20:30:42 GMT  
		Size: 2.3 KB (2318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471cd2e2e06e98508a0e2e6b50639c610394048b21b2be20c5b7696e80e70daa`  
		Last Modified: Thu, 17 Feb 2022 20:30:42 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765007d7baa6246d9028224bfe7a0d037a167094649a351056fce0e72d57f4f6`  
		Last Modified: Thu, 17 Feb 2022 20:30:42 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f81742c9ea7c5c8cd606475d73f7b3833c06370915194b6f414a2c9df317609`  
		Last Modified: Thu, 17 Feb 2022 22:39:47 GMT  
		Size: 1.2 MB (1160342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f72031c1f4a6272ec4e6704ffdab16d80c8a76d1ed3f7bbd54274de306afb2f`  
		Last Modified: Thu, 17 Feb 2022 22:39:47 GMT  
		Size: 1.2 MB (1153198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e68914e673bb76e9486db82c4ca2b69daa163f83647fd28e869a942219d5f66`  
		Last Modified: Thu, 17 Feb 2022 22:39:45 GMT  
		Size: 8.2 KB (8223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229e65c36b02e9bf59c9188200449bbced2ecb4eed52f8f6185a94cb96311ac5`  
		Last Modified: Thu, 17 Feb 2022 22:39:47 GMT  
		Size: 1.9 MB (1864794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f08abde78eba2e5afd4a31c59eae12d47727b9591b392f679f0d3b14037136c`  
		Last Modified: Thu, 17 Feb 2022 22:39:45 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:db3ec92bd74d66233cdbc093d9c41721639c660a254e3ed6fb387411892f6729
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172567442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399c879c3178b95eead03e04385171eea93ac307288587823a3876577785889b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:29:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 10:29:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 10:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 10:31:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 10:31:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 10:40:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 10:40:14 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 10:41:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 10:41:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 10:41:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 10:41:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 10:41:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 10:41:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 12:25:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 18:31:06 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 18:31:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 18:31:11 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 18:33:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Feb 2022 18:33:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Feb 2022 18:38:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Feb 2022 18:38:38 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 17 Feb 2022 18:38:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Feb 2022 18:38:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Feb 2022 18:38:55 GMT
STOPSIGNAL SIGWINCH
# Thu, 17 Feb 2022 18:38:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 17 Feb 2022 18:39:00 GMT
WORKDIR /var/www/html
# Thu, 17 Feb 2022 18:39:05 GMT
EXPOSE 80
# Thu, 17 Feb 2022 18:39:08 GMT
CMD ["apache2-foreground"]
# Thu, 17 Feb 2022 22:45:57 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 17 Feb 2022 22:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Feb 2022 22:48:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Feb 2022 22:48:05 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 17 Feb 2022 22:48:07 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 17 Feb 2022 22:48:13 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 17 Feb 2022 22:48:18 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 17 Feb 2022 22:48:22 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 17 Feb 2022 22:48:33 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 17 Feb 2022 22:48:42 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 17 Feb 2022 22:48:47 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 17 Feb 2022 22:48:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 17 Feb 2022 22:48:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6353566d57126497241a2d1359b8e40a4aa82b31a4fb89b70b71f25028296b7d`  
		Last Modified: Wed, 26 Jan 2022 13:46:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1c3a5c5a3593cebdd72b812ae7ebe3522a05b2d5522abf096556c638af718`  
		Last Modified: Wed, 26 Jan 2022 13:47:18 GMT  
		Size: 86.6 MB (86624458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824b5fa25d786f0ce5c69716c3b8b6ed693840142dbc489273cfd54b9bf7cd3`  
		Last Modified: Wed, 26 Jan 2022 13:46:29 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de019d08f1c17354d8643f0d49cdb41e9b7e26614ba5a7436b782ea079171078`  
		Last Modified: Wed, 26 Jan 2022 13:48:35 GMT  
		Size: 20.5 MB (20451239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3fedf8071a108e2c69f4f313a0851b4de8cf56294204dcd4a0600b599ebef5`  
		Last Modified: Wed, 26 Jan 2022 13:48:24 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b34bae6208b08ced06055ea40bc35cd69a6258050e1fa7a2f84b88e95f5b16`  
		Last Modified: Wed, 26 Jan 2022 13:48:23 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b01165a0df2147f3288c2f61276f8d62f5fc547bc47c48e95245412723bde6`  
		Last Modified: Thu, 17 Feb 2022 20:07:05 GMT  
		Size: 10.8 MB (10758422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536495dc91b2df92b85fdcb9318a7aec588d61c9593ccb2b4825e823ae8a55e`  
		Last Modified: Thu, 17 Feb 2022 20:07:02 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92223817ba49f61d565b5f8d132d792f733b59413a724e1601d42ecc47aad66f`  
		Last Modified: Thu, 17 Feb 2022 20:07:05 GMT  
		Size: 15.1 MB (15072067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee829ed620109332646b7c4ba12f6a0427121852356f8ee4099fb7e722ca1f0`  
		Last Modified: Thu, 17 Feb 2022 20:07:02 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56435856a053da3e484fbe4bb389cf3e4e6bc1ce5ad3f6e2dcb209a587c570e8`  
		Last Modified: Thu, 17 Feb 2022 20:07:02 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500c75a5c21cd5e86c81445de5ed30ef5d82085188bfea49ce0c3d01f12d6b15`  
		Last Modified: Thu, 17 Feb 2022 20:07:02 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f04a0bcad40dadb31447fef15fa439ed48734874f2902fd9ebcbb2f74a1db77`  
		Last Modified: Thu, 17 Feb 2022 22:54:29 GMT  
		Size: 1.2 MB (1186735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be095121a6e1090ca9cbfb1865f8fd629688f79fc0ff3f0f7e77e33fe024d4f`  
		Last Modified: Thu, 17 Feb 2022 22:54:31 GMT  
		Size: 1.3 MB (1321381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6e2f9399e5e6d1a5e0634f7c202938013277de88141ffe015779c8386d500a`  
		Last Modified: Thu, 17 Feb 2022 22:54:28 GMT  
		Size: 8.2 KB (8224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2155a80e145ce7b36104bb8314ccbc3c73a4378a9ea4fcd26f8da3ecdb8647ee`  
		Last Modified: Thu, 17 Feb 2022 22:54:31 GMT  
		Size: 1.9 MB (1864831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19862cf47ac44f415a6fec8bf94e9d5eb675c6d88fa93ee9f9c75c6a142ee964`  
		Last Modified: Thu, 17 Feb 2022 22:54:28 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-apache` - linux; s390x

```console
$ docker pull postfixadmin@sha256:6661d67fe911f73b87bb9cd30bb245446f36a6e27ef00f78104b9daf27ce943d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.1 MB (145070610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23522f78420a0e60540b58b3e13da8b25a8ae4372d52a9692bcbbe6bc642a913`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:33:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 13:33:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 13:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:34:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 13:34:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 13:38:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 13:38:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 13:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 13:38:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 13:38:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 13:38:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:38:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 13:38:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 14:25:12 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Mar 2022 14:25:13 GMT
ENV PHP_VERSION=7.4.28
# Tue, 01 Mar 2022 14:25:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 01 Mar 2022 14:25:13 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 01 Mar 2022 14:26:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 14:26:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 20:46:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 20:46:29 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 02 Mar 2022 20:46:29 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 20:46:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 20:46:30 GMT
STOPSIGNAL SIGWINCH
# Wed, 02 Mar 2022 20:46:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 02 Mar 2022 20:46:30 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 20:46:30 GMT
EXPOSE 80
# Wed, 02 Mar 2022 20:46:30 GMT
CMD ["apache2-foreground"]
# Thu, 03 Mar 2022 01:22:32 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 03 Mar 2022 01:22:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 01:22:56 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 01:22:56 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Thu, 03 Mar 2022 01:22:56 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 03 Mar 2022 01:22:56 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Thu, 03 Mar 2022 01:22:56 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 03 Mar 2022 01:22:56 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 03 Mar 2022 01:22:57 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 03 Mar 2022 01:22:58 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 03 Mar 2022 01:22:58 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 03 Mar 2022 01:22:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 03 Mar 2022 01:22:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e36e768b2f62ca9db79fc8204f94fabef165bdb7951c4ecdc3161e42c72b599`  
		Last Modified: Tue, 01 Mar 2022 15:09:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33e437f967c6f0d1b201253e1e22ce9112d55070778d806c5e693166688bfc7`  
		Last Modified: Tue, 01 Mar 2022 15:09:45 GMT  
		Size: 71.6 MB (71618545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9901cb4d6a8d6e06176baa29aea61892e9441218ce09d660d1bf74bbbf2821`  
		Last Modified: Tue, 01 Mar 2022 15:09:35 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72000d6dbd55db9891a9bdf73316a6f38c08738434fa5e9e9538eaebcf2ea70d`  
		Last Modified: Tue, 01 Mar 2022 15:10:46 GMT  
		Size: 19.1 MB (19053282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c4812e3690c565829cdfa5f82031285c5615e6db793eaaafc46553a13c30b`  
		Last Modified: Tue, 01 Mar 2022 15:10:43 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92dcb478c8b8955a505a5bb6b5e945ea59de406f2ba01069497a50797d9c12`  
		Last Modified: Tue, 01 Mar 2022 15:10:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5169f58b2b797f7abf062613e4b29ed7858e84efc0387e10815ab7835a9d208`  
		Last Modified: Tue, 01 Mar 2022 15:16:02 GMT  
		Size: 10.8 MB (10757135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27fb49be7613decee09bad0c9a905802e949196c1c571c784cbb94dcbe068e76`  
		Last Modified: Tue, 01 Mar 2022 15:16:00 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7901c7c5cd431f4339f8c8a61bad531303ada1d5703e7c3a3ae896268cfc216f`  
		Last Modified: Wed, 02 Mar 2022 22:02:41 GMT  
		Size: 9.7 MB (9687410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f0a842499523d36b9c040f784f95218c8566b827e897f214f0c217294b5c1c`  
		Last Modified: Wed, 02 Mar 2022 22:02:39 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0788341dc2845306aef4029283660a1b162ac2b7d915bd1f4c4ffe8f9e834`  
		Last Modified: Wed, 02 Mar 2022 22:02:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac2af456bae72edaae053ae089986b8b09bcff14eeea6d73f3bebbb4a4928e1`  
		Last Modified: Wed, 02 Mar 2022 22:02:39 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8f0571127fd76f1d2d320335899c2eadc046e6059cca6a1bcda66fa2eeca57`  
		Last Modified: Thu, 03 Mar 2022 01:24:45 GMT  
		Size: 1.2 MB (1245387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b14e537f21bc1535010929965b2de0c319951d27fb7862fbbf557f5fcc5a3e`  
		Last Modified: Thu, 03 Mar 2022 01:24:45 GMT  
		Size: 1.2 MB (1181380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968deb01fac168020fd4506c6c7a927a1f9e7cb1982de66eca4f95df750ee736`  
		Last Modified: Thu, 03 Mar 2022 01:24:45 GMT  
		Size: 8.2 KB (8218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6229d7c90ae84719f75aa25a7c7f74ff91beacb7001f55580547ff948b2cffde`  
		Last Modified: Thu, 03 Mar 2022 01:24:45 GMT  
		Size: 1.9 MB (1865106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b647125ba59c98cf26fb143689438d74981f2994a149ea64149e4d3e81af6b8e`  
		Last Modified: Thu, 03 Mar 2022 01:24:45 GMT  
		Size: 1.6 KB (1598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
